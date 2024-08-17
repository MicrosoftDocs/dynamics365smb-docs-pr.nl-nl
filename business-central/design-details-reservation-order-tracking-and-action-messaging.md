---
title: 'Ontwerpdetails - reservering, ordertracking en actieberichten | Microsoft Docs'
description: Het reserveringssysteem is uitgebreid en omvat de onderling verbonden en parallelle functies van Order Tracking en Action Messaging.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'design, replenishment, reordering'
ms.date: 08/06/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="design-details-reservation-order-tracking-and-action-messaging"></a>Ontwerpdetails: reservering, ordertracering en planningsboodschappen

Het uitgebreide reserveringssysteem omvat de onderling verbonden en parallelle functies van Order Tracking en Action Messaging.  

De kern van het reserveringssysteem is de koppeling van een vraaginvoer en een bijbehorende aanbodinvoer, hetzij via reservering of ordertracking. Een reservering is een door de gebruiker gegenereerde koppeling en een ordertraceringsrecord is een door het systeem gegenereerde koppeling. Een artikelhoeveelheid die in het reserveringssysteem is ingevoerd, wordt óf gereserveerd óf de order gevolgd, maar niet beide tegelijkertijd. Hoe de systemen met een item omgaan, hangt af van de manier waarop het item is ingesteld.  

Het reserveringssysteem communiceert met het planningssysteem door planningsboodschappen op planningsregels te maken tijdens uitgevoerde planningen. Een planningsboodschap kan als een aanhangsel van een ordertraceringsrecord worden beschouwd. Planningsboodschappen, hetzij dynamisch gemaakt in ordertracering of tijdens de planning, bieden een handig hulpmiddel voor efficiënte voorraadplanning.  

> [!NOTE]  
> Gereserveerde aantallen worden genegeerd door het planningsysteem. Dit betekent dat de vaste koppeling tussen voorziening en vraag niet kan worden gewijzigd via de planning.  

 Het reserveringssysteem vormt ook de structurele basis voor het artikeltraceringsysteem. Ga voor meer informatie naar  [Ontwerpdetails: Itemtracering](design-details-item-tracking.md).  

 <!--For more detailed information about how the reservation system works, see the _Reservation Entry Table_ white paper on [PartnerSource](https://go.microsoft.com/fwlink/?LinkId=258348).  -->
<!--
> [!NOTE]
> [!INCLUDE [locations-cronus](includes/locations-cronus.md)]
-->

## <a name="reservation"></a>Reservering

 Een reservering is een vaste koppeling die bepaalde vraag en een bepaald aanbod aan elkaar koppelt. Deze koppeling heeft rechtstreeks invloed op de verdere voorraadtransactie en zorgt voor de juiste vereffening van artikelposten voor waarderingsdoeleinden. Een reservering overschrijft de standaardwaarderingsmethode van een artikel. Ga voor meer informatie naar  [Ontwerpdetails: Itemtracering](design-details-item-tracking.md).  

 De  **Reserveringspagina**  is toegankelijk vanaf alle orderregels van zowel vraag- als aanbodtypes. Op deze pagina kan de gebruiker aangeven voor welke vraag- of aanbodpost een reservering koppelen moet worden aangemaakt. De reservering bestaat uit een paar records dat hetzelfde volgnummer deelt. Eén record heeft een negatief teken en verwijst naar de vraag. De andere record heeft een positief teken en wijst naar de voorziening. Deze records worden opgeslagen in de tabel  *Reserveringsinvoer*  met de statuswaarde  *Reservering*. De gebruiker kan alle reserveringen bekijken op de pagina **Reserveringsposten**.  

### <a name="offsetting-in-reservations"></a>Compenseren in reserveringen

 Reserveringen worden gemaakt op basis van beschikbare artikelaantallen. Artikelbeschikbaarheid wordt in het kort als volgt berekend:  

 `available quantity = inventory + scheduled receipts - gross requirements`

 De volgende tabel toont de gegevens van de ordernetwerkentiteiten die deel uitmaken van de beschikbaarheidsberekening.  

||Veld in T27 Item|Brontabel|Tabelfilter|Bronveld|  
|-|------------------|------------------|------------------|------------------|  
|**Voorraad**|Voorraad|Artikelpost|N.v.t.|Aantal|  
|**Geplande ontvangsten**|Vast gepl. orderontv. (Aantal)|Prod.-orderregel|=Vast gepland|Resterend aantal (Basis)|  
|**Geplande ontvangsten**|Vrijgeg. orderontv. (Aantal)|Prod.-orderregel|=Vrijgegeven|Resterend aantal (Basis)|  
|**Geplande ontvangsten**|Aant. op assemblageorder|Assemblagekop|=Volgorde|Resterend aantal (Basis)|  
|**Geplande ontvangsten**|Aantal in inkooporders|Inkoopregel|=Volgorde|Openstaand aantal (Basis)|  
|**Geplande ontvangsten**|Transferorderontv. (Aantal)|Transferregel|N.v.t.|Openstaand aantal|  
|**Brutobehoeften**|Aantal in verkooporders|Verkoopregel|=Volgorde|Openstaand aantal (Basis)|  
|**Brutobehoeften**|Geplande behoefte (Aantal)|Materiaalregel|<>Gesimuleerd|Resterend aantal (Basis)|  
|**Brutobehoeften**|Aant. op assemblagecomponent|Assemblagelijn|=Volgorde|Resterend aantal (Basis)|  
|**Brutobehoeften**|Transferorderverz. (Aantal)|Transferregel|N.v.t.|Openstaand aantal|  

 Ga voor meer informatie naar [Ontwerpdetails: Beschikbaarheid in het magazijn](design-details-availability-in-the-warehouse.md).  

### <a name="manual-reservation"></a>Handmatige reservering

Wanneer een gebruiker opzettelijk een reservering maakt, verkrijgt de gebruiker volledig eigendom van en verantwoordelijkheid voor deze artikelen. Dit betekent dat de gebruiker een reservering ook handmatig moet wijzigen of annuleren. Dergelijke handmatige wijzigingen kunnen leiden tot automatische aanpassing van de betrokken reserveringen.  

De volgende tabel laat zien wanneer en welke wijzigingen kunnen optreden:  

|Gebruikersactie|Systeemreactie|  
|-----------------|---------------------|  
|Het gereserveerde aantal verlagen|De gerelateerde aantalvelden worden bijgewerkt.|  
|Datumvelden wijzigen|De gerelateerde datumvelden worden bijgewerkt.<br /><br /> **Opmerking:** als de vervaldatum van een vraag wordt veranderd en vóór de verzenddatum of de vervaldatum van de voorziening komt te liggen, wordt de reservering geannuleerd.|  
|De order verwijderen|De reservering is geannuleerd.|  
|Vestiging, opslaglocatie, variant, serienummer of lotnummer wijzigen|De reservering is geannuleerd.|  

> [!NOTE]  
> Met de functie voor late binding kunnen ook reserveringen worden gewijzigd zonder de gebruiker te informeren, door niet-specifieke reserveringen van serie- of lotnummers te wisselen. Ga voor meer informatie naar [Ontwerpdetails: Itemtracering en reserveringen](design-details-item-tracking-and-reservations.md).  

### <a name="automatic-reservations"></a>Automatische reserveringen

Het artikel kaart kan zo worden ingesteld dat artikelen automatisch worden gereserveerd op basis van vraag, zoals verkooporders. In dat geval wordt de reservering gedaan op basis van voorraad, inkooporders, assemblageorders en productieorders. Als de voorraad onvoldoende is, ontvangt u een waarschuwing.  

Daarnaast zorgen diverse planningsfuncties ervoor dat artikelen automatisch worden gereserveerd, zodat vraag en aanbod aan elkaar gekoppeld blijven. De ordertracking-items voor dergelijke planningskoppelingen bevatten **Reservering** in het veld **Reserveringsstatus** in de tabel *Reserveringsitem* . Automatische reserveringen worden gemaakt in de volgende situaties:  

- Een productieorder met meerdere niveaus waarvoor het veld **Productiebeleid** van het bovenliggende artikel en de onderliggende artikelen is ingesteld op **Op order produceren**. Het planningssysteem maakt reserveringen tussen de productieorder bovenliggend en de onderliggende productieorder om ervoor te zorgen dat ze gelijktijdig worden verwerkt. Deze reserveringsbinding overschrijft de standaardkostenberekening en toepassingsmethode van het artikel.  

- Een productie, assemblage of inkooporder waarvoor het veld **Bestelbeleid** van het betreffende artikel is ingesteld op **Order**. Het planningssysteem maakt reserveringen tussen de vraag en de geplande voorziening om te zorgen dat de specifieke voorziening wordt gemaakt. Ga voor meer informatie naar  [Bestellen](design-details-handling-reordering-policies.md#order).  

- Er wordt een productieorder gemaakt van een verkooporder met de functie **Verkooporderplanning** en met een automatische reservering aan de verkooporder gekoppeld.  

- Een assemblageorder die automatisch wordt aangemaakt voor een verkooporderregel om de hoeveelheid in het veld  **Aantal voor assemblage op order** te leveren. Deze automatische reservering koppelt de verkoopvraag en de assemblagevoorziening, zodat de verkooporderverwerkers de component rechtstreeks kunnen aanpassen en aan de klant kunnen toezeggen. Bovendien koppelt de reservering de assemblage-uitvoer aan de verkooporderregel door middel van de verzendactiviteit die voldoet aan de order van de klant.  

Voor vraag of aanbod dat niet is toegewezen, wijst het planningssysteem automatisch een reserveringsstatus  **Overschot** toe. Dit kan resulteren uit vraag die het gevolg is van voorspelde aantallen of door de gebruiker ingevoerde planningsparameters. Dit is een legitiem overschot, dat door het systeem wordt herkend en dat geen aanleiding geeft tot actie. Het overschot kan ook een daadwerkelijke overmaat aan aanbod of vraag zijn die niet wordt bijgehouden. Dit is een aanduiding om aan te geven dat het ordernetwerk niet in evenwicht is, waardoor het systeem planningsboodschappen verzendt. Een planningsboodschap die een wijziging van aantal voorstelt, verwijst altijd naar de soort **Overschot**. Ga voor meer informatie naar het gedeelte  [Voorbeeld: Ordertracering in verkoop, productie en overdrachten](#example-order-tracking-in-sales-production-and-transfers)  in dit artikel.  

Automatische reserveringen die tijdens de geplande run worden gemaakt, worden op de volgende manieren verwerkt:  

- Ze zijn van toepassing op de artikelhoeveelheden die zijn opgenomen in de beschikbaarheidsberekening,.Net als handmatige reserveringen. Ga voor meer informatie naar het gedeelte 'Compensatie in reserveringen' in dit artikel.  

- In tegenstelling tot handmatig gereserveerde items worden ze opgenomen en mogelijk gewijzigd in latere planningsruns.  

## <a name="order-tracking"></a>Ordertracering

Ordertracering helpt de planner een geldig leveringsplan te onderhouden door een overzicht te geven van de compensatie tussen vraag en aanbod in het ordernetwerk. De ordertraceringsrecords dienen als basis voor het maken van dynamische planningsboodschappen en planningsregelvoorstellen tijdens uitgevoerde planningen.  

> [!NOTE]  
> Het ordertraceringssysteem compenseert beschikbare voorraad wanneer orders in het ordernetwerk worden ingevoerd. Dit geeft aan dat het systeem geen prioriteit geeft aan orders die mogelijk urgenter zijn op basis van de vervaldatum. Het is daarom aan de logica van het planningssysteem of de wijsheid van de planner om deze prioriteiten op een zinnige manier te ordenen.  

> [!NOTE]  
> Het ordertrackingbeleid en de functie Actieberichten ophalen zijn niet geïntegreerd met projecten. Dit betekent dat de vraag met betrekking tot een project niet automatisch wordt getraceerd. Omdat het niet wordt getraceerd, kan hierdoor het gebruik van een bestaande aanvulling met projectinformatie worden getraceerd naar een andere vraag, bijvoorbeeld een verkooporder. Hierdoor kan het voorkomen dat uw informatie over de beschikbare voorraad niet meer klopt.  

### <a name="the-order-network"></a>Het ordernetwerk

Het ordervolgsysteem is gebaseerd op het principe dat het ordernetwerk altijd in evenwicht moet zijn, zodat elke vraag die het systeem binnenkomt, wordt gecompenseerd door een overeenkomstig aanbod en vice versa. Het systeem verzorgt dit door logische koppelingen tussen alle vraag- en voorzieningsposten in het ordernetwerk te identificeren.  

Dit principe geeft aan dat een wijziging in de vraagresultaten ertoe leidt dat de voorzieningenzijde van het ordernetwerk niet meer in evenwicht is. Andersom leidt een wijziging in voorzieningenresultaten tot een corresponderende onbalans aan de vraagzijde van het ordernetwerk. In werkelijkheid bevindt het ordernetwerk zich in een constante stroom terwijl gebruikers orders invoeren, wijzigen en verwijderen. Tijdens ordertracering worden orders dynamisch verwerkt, in reactie op elke wijziging op het moment dat deze het systeem binnenkomt en onderdeel wordt van het ordernetwerk. Zodra nieuwe ordertraceringsrecords worden gemaakt, is het ordernetwerk in balans, maar slechts tot de volgende wijziging zich voordoet.  

Om de transparantie te verhogen van berekeningen in het planningssysteem, worden op de pagina **Niet-getraceerde planningselementen** niet-getraceerde aantallen weergegeven, die het verschil in aantal aangeven tussen bekende vraag en voorgestelde voorziening. Elke regel op de pagina verwijst naar de oorzaak van het bovenmatige aantal, bijvoorbeeld **Raamcontract**, **Veiligheidsvoorraadniveau**, **Vast bestelaantal**, **Min. bestelaantal**, **Afronding** of **Demping**.  

### <a name="offsetting-in-order-tracking"></a>Compenseren in ordertracering

In tegenstelling tot reserveringen, die alleen kunnen worden gedaan op basis van beschikbare artikelaantallen, is ordertracering mogelijk op basis van alle ordernetwerkentiteiten die deel uitmaken van de berekening van nettovereisten van het planningssysteem. De nettobehoeften worden als volgt berekend:  

`net requirements = gross requirements + reorder point - scheduled receipts - planned receipts - projected available balance`  

> [!NOTE]  
> Vraag die is gerelateerd aan prognoses of planningsparameters is niet ordergetraceerd.  

### <a name="example-order-tracking-in-sales-production-and-transfers"></a>Voorbeeld: Ordertracering in verkoop, productie en transfers

In het volgende scenario ziet u welke ordertrackingposten in de tabel  *Reserveringspost* worden aangemaakt als gevolg van verschillende wijzigingen in het ordernetwerk.  

Stel dat er de volgende gegevens zijn voor twee artikelen die zijn ingesteld voor ordertracering.  

|Artikel|Parameter|Details|
|-|-|-|
|Artikel 1|Naam|Component|
||Beschikbaarheid|100 eenheden op EAST-vestiging<br /><br />- 30 eenheden van LOTA<br />- 70 eenheden van LOTB|  
|Artikel 2|Naam|Geproduceerd item|
||Productiestuklijst|1 hoeveelheid per component|  
||Vraag|Verkoop voor 100 eenheden op WEST-locatie|  
||Voorraad|Vrijgegeven productieorder (gegenereerd met de functie  *Sales Order Planning* voor de verkoop van 100 eenheden)|  

Op de pagina  **productie-instellingen** is het veld  **Componenten op locatie**  ingesteld op  *OOST*.

De volgende ordertrackingposten zijn aanwezig in de tabel  *Reserveringspost* op basis van de gegevens in de tabel.  

<!--![First example of order tracking entries in Reservation Entry table.](media/supply_planning_RTAM_1.png "supply_planning_RTAM_1")  -->
**Reserveringsinschrijvingen**

|Postnr.|Positief|Artikelnr.|Vestigingscode|Hoeveelheid|Status reservering|Omschrijving|Partijnr.|Type bron|Voor id|Binding|  
|--------|--------|--------|-------------|--------|------------------|-----------|-------|-----------|---------|-------| 
|8|-|ONDERDEEL|OOST|-70|Tracering|Component|-|5407|101004|-|
|8|Ja|ONDERDEEL|OOST|70|Tracering|Component|LOTB|32|-|-| 
|9|-|ONDERDEEL|OOST|-30|Tracering|Component|-|5407|1001004|-| 
|9|Ja|ONDERDEEL|OOST|30|Tracering|Component|LOTA|32|-|-| 
|10|-|GEPRODUCEERD ARTIKEL|WEST|-100|Reservering|Geproduceerd item|-|37|1001|Order-op-order|
|10|Ja|GEPRODUCEERD ARTIKEL|WEST|100|Reservering|Geproduceerd item|-|5406|101004|Order-op-order|


#### <a name="entry-numbers-8-and-9"></a>Volgnummers 8 en 9

Voor de componentbehoefte voor respectievelijk LOTA en LOTB worden ordertrackingkoppelingen gemaakt van de vraag in tabel 5407, *Prod. Order Component*, naar de levering in tabel 32, *Item Ledger Entry*. Het veld  **Reserveringsstatus** bevat *Tracking* om aan te geven dat deze vermeldingen dynamische koppelingen voor ordertracking zijn tussen vraag en aanbod.  

> [!NOTE]  
> Het veld  **Lotnr.** is leeg op de vraagregels omdat de lotnummers niet zijn gespecificeerd op de componentregels van de vrijgegeven productieorder.  

#### <a name="entry-number-10"></a>Volgnummer 10

Uit de verkoopvraag in tabel 37, *Verkooplijnen*, een order tracking koppelen wordt aangemaakt voor de levering in tabel 5406, *Prod. Orderregel*. De **Reserveringsstatus**  veld bevat *Reservering*, en de **Verbindend**  veld bevat *Bestelling-op-bestelling*. Dit komt doordat de vrijgegeven productieorder specifiek voor de verkooporder is gegenereerd en gekoppeld moet blijven, in tegenstelling tot ordertrackingkoppelingen met de reserveringsstatus Tracking, die dynamisch worden aangemaakt en gewijzigd. Voor meer informatie, ga naar de [Automatische reserveringen](#automatic-reservations)  sectie in dit artikel.  

 Bij deze aanwijzen in het scenario worden de 100 eenheden van LOTA en LOTB via een overdrachtsorder overgebracht naar de WEST-locatie.  

> [!NOTE]  
> Alleen de transferorderverzending wordt op dit moment geboekt, niet de ontvangst.  

 Nu bestaan de volgende ordertracking-items in de *Reservering toegang*  tafel.  

<!-- ![Second example of order tracking entries in Reservation Entry table.](media/supply_planning_RTAM_2.png "supply_planning_RTAM_2")  -->
**Reserveringsinschrijvingen**

|Postnr.|Positief|Artikelnr.|Vestigingscode|Hoeveelheid|Status reservering|Omschrijving|Partijnr.|Type bron|Voor id|Binding|  
|---------|--------|--------|-------------|--------|------------------|-----------|-------|-----------|---------|-------| 
|9|-|ONDERDEEL|OOST|-30|Overschot|Component|-|5407|1001004|-| 
|10|-|GEPRODUCEERD ARTIKEL|WEST|-100|Reservering|Geproduceerd item|-|37|1001|Order-op-order|
|10|Ja|GEPRODUCEERD ARTIKEL|WEST|100|Reservering|Geproduceerd item|-|5406|101004|Order-op-order|
|12|Ja|ONDERDEEL|WEST|70|Overschot|Component|LOTB|5741|1011|-| 
|14|Ja|ONDERDEEL|WEST|30|Overschot|Component|LOTA|5741|1011|-| 
|15|Ja|ONDERDEEL|UIT.LOG.|70|Overschot|Component|LOTB|32|-|-| 
|16|Ja|ONDERDEEL|UIT.LOG.|30|Overschot|Component|LOTA|32|-|-| 

#### <a name="entry-numbers-8-and-9-1"></a>Volgnummers 8 en 9

De ordertrackingposten voor de twee partijen van het onderdeel dat de vraag in tabel 5407 weerspiegelt, zijn gewijzigd van een reserveringsstatus van *Tracking* naar *Overschot*. De reden hiervoor is dat de leveringen die eerder in tabel 32 zijn gekoppeld, worden gebruikt bij de verzending van de overdrachtsorder.  

Werkelijk overschot, zoals in dit geval, is een reflectie van bovenmatig aanbod of vraag die niet-getraceerd blijft. Het is een indicatie van een onevenwicht in het ordernetwerk. Als het niet dynamisch wordt opgelost, genereert het planningssysteem een actiemelding.  

#### <a name="entry-numbers-12-to-16"></a>Volgnummers 12 tot 16

Omdat de twee partijen van het onderdeel op de overdrachtsorder zijn geboekt als verzonden maar nog niet ontvangen, zijn alle gerelateerde positieve ordertraceringsposten van het reserveringstype  *Overschot*, wat aangeeft dat ze niet aan enige vraag zijn toegewezen. Voor elk lotnummer heeft één post betrekking op tabel 5741,  *Transferregel*, en één post heeft betrekking op de artikelpost op de in-transitlocatie waar de artikelen zich nu bevinden.  

Bij deze aanwijzen in het scenario wordt de overdrachtsvolgorde van de componenten van de locatie  *OOST* naar *WEST* geboekt als ontvangen.  

Nu bestaan de volgende ordertracking-items in de *Reservering toegang*  tafel.  

<!-- ![Third example of order tracking entries in Reservation Entry table.](media/supply_planning_RTAM_3.png "supply_planning_RTAM_3") -->
 **Reserveringsinschrijvingen**

|Postnr.|Positief|Artikelnr.|Vestigingscode|Hoeveelheid|Status reservering|Omschrijving|Partijnr.|Type bron|Voor id|Binding|  
|---------|--------|--------|-------------|--------|------------------|-----------|-------|-----------|---------|-------| 
|8|-|ONDERDEEL|OOST|-70|Overschot|Component|-|5407|101004|-| 
|9|-|ONDERDEEL|OOST|-30|Overschot|Component|-|5407|1001004|-|
|10|-|GEPRODUCEERD ARTIKEL|WEST|-100|Reservering|Geproduceerd item|-|37|1001|Order-op-order|
|10|Ja|GEPRODUCEERD ARTIKEL|WEST|100|Reservering|Geproduceerd item|-|5406|101004|Order-op-order|
|17|Ja|ONDERDEEL|WEST|70|Overschot|Component|LOTB|32|-|-| 
|18|Ja|ONDERDEEL|WEST|30|Overschot|Component|LOTA|32|-|-| 

De ordertracking-vermeldingen lijken nu op de eerste aanwijzen in het scenario voordat de overdrachtsorder werd geboekt als alleen verzonden, behalve dat de vermeldingen voor het onderdeel nu de reserveringsstatus  *Overschot* hebben. Dit komt doordat de componentbehoefte zich nog steeds op de locatie  *OOST* bevindt, wat aangeeft dat het veld  **Locatiecode** op de componentregel van de productieorder  *OOST* bevat zoals ingesteld in het veld  **Componenten op locatie** . De levering die eerder aan deze vraag was toegewezen, is overgebracht naar de  *WEST* locatie en kan niet volledig worden getraceerd, tenzij de componentbehoefte op de productieorderregel wordt gewijzigd naar de  *WEST* locatie.  

Bij deze aanwijzen in het scenario is de **Locatiecode** op de componentregel van de productieorder ingesteld op *WEST*. Bovendien worden op de pagina  **Artikeltraceringsregels** de 30 eenheden van LOTA en de 70 eenheden van LOTB toegewezen aan de componentregel van de productieorder.  

Nu bestaan de volgende ordertracking-items in de *Reservering toegang*  tafel.  

<!-- ![Fourth example of order tracking entries in Reservation Entry table.](media/supply_planning_RTAM_4.png "supply_planning_RTAM_4")   -->
 **Reserveringsinschrijvingen**

|Postnr.|Positief|Artikelnr.|Vestigingscode|Hoeveelheid|Status reservering|Omschrijving|Partijnr.|Type bron|Voor id|Binding|  
|---------|--------|--------|-------------|--------|------------------|-----------|-------|-----------|---------|-------| 
|10|-|GEPRODUCEERD ARTIKEL|WEST|-100|Reservering|Geproduceerd item|-|37|1001|Order-op-order|
|10|Ja|GEPRODUCEERD ARTIKEL|WEST|100|Reservering|Geproduceerd item|-|5406|101004|Order-op-order|
|21|-|ONDERDEEL|WEST|-70|Tracering|Component|LOTB|5407|101004|-| 
|21|Ja|ONDERDEEL|WEST|70|Tracering|Component|LOTB|32|-|-| 
|22|-|ONDERDEEL|WEST|-30|Tracering|Component|LOTA|5407|1001004|-| 
|22|Ja|ONDERDEEL|WEST|30|Tracering|Component|LOTA|32|-|-| 

#### <a name="entry-numbers-21-and-22"></a>Volgnummers 21 en 22

Omdat de componentbehoefte is gewijzigd naar de  *WEST* locatie en de levering beschikbaar is als artikelgrootboekposten op de  *WEST* locatie, worden alle ordertrackingposten voor de twee lotnummers nu volledig getraceerd, wat wordt aangegeven door de reserveringsstatus van  *Tracking*.  

Het veld  **Lotnr.**  is nu ingevuld in de ordertraceringsinvoer voor tabel 5407, omdat de lotnummers zijn toegewezen aan de componentregels van de productieorder.  

## <a name="action-messaging"></a>Planningsboodschap

Wanneer het ordertraceringssysteem detecteert dat het ordernetwerk niet in evenwicht is, wordt automatisch een planningsboodschap gemaakt om de gebruiker te waarschuwen. Actieberichten zijn door het systeem gegenereerde oproepen voor gebruikersacties waarin de details van de onbalans worden gespecificeerd, evenals suggesties voor het herstellen van de balans in het ordernetwerk. Ze worden weergegeven als planningslijnen op de pagina  **Planningswerkbladen** wanneer u de actie  **Actieberichten ophalen**  kiest. Daarnaast worden er tijdens de planningsrun actieberichten op planningsregels gegenereerd, die de suggesties van het planningssysteem weerspiegelen om de balans in het ordernetwerk te herstellen. In beide gevallen worden de suggesties uitgevoerd op het ordernetwerk, wanneer u de actie  **Actiebericht uitvoeren**  kiest.  

Een planningsboodschap betreft één stuklijstniveau tegelijk. Als de gebruiker de actiemelding accepteert, kan dit leiden tot aanvullende actiemeldingen op het volgende stuklijstniveau.  

De volgende tabel toont de planningsboodschappen die bestaan.  

|Planningsboodschap|Description|  
|--------------------|---------------------------------------|  
|**Aantal wijzigen**|Wijzigt het aantal op een bestaande voorzieningenorder om te voldoen aan gewijzigde of nieuwe vraag.|  
|**Herplannen**|Herplant de vervaldatum op een bestaande order.|  
|**Herplannen en aantal wijzigen**|Herplant de vervaldatum en wijzigt het aantal op een bestaande order.|  
|**Nieuw**|Maakt een nieuwe order aan als de vraag niet kan worden vervuld door een van de voorgaande actieberichten.|  
|**Annuleren**|Hiermee annuleert u een bestaande order.|  

Het ordertraceringssysteem probeert altijd om een verstoord evenwicht in het bestaande ordernetwerk op te lossen. Als dit niet mogelijk is, wordt er een actiebericht gegenereerd om een nieuwe order aan te maken. Hierna volgt de prioriteitlijst die het ordertraceringssysteem gebruikt om te bepalen hoe het evenwicht wordt hersteld. Als er extra vraag in het ordernetwerk terechtkomt, probeert het systeem de order te traceren aan de hand van de volgende controles:  

1. Controleer op bovenmatige voorziening in de bestaande ordertraceringsrecord voor deze vraag.  
1. Controleer op geplande ontvangsten op volgorde van ontvangstdatum. De laatst mogelijke datum wordt geselecteerd.  
1. Controleer op beschikbare voorraad.  
1. Controleer of er een voorzieningenorder bestaat in de huidige ordertraceringsrecord. Indien dit het geval is, geeft het systeem een actiebericht van het type  *Wijzigen*  om de bestelling te verhogen.  
1. Controleer of er geen voorzieningenorder bestaat in de huidige ordertraceringsrecord. Indien dit het geval is, geeft het systeem een actiebericht van het type  *Nieuw*  uit om een nieuwe order aan te maken.  

Openstaande vraag doorloopt de lijst en compenseert op elk punt de beschikbare voorraad. Eventuele resterende vraag wordt altijd gedekt door controle 4 of controle 5.  

Als er een afname van vraag optreedt, probeert het ordertraceringssysteem de onbalans op te lossen door de vorige controles in omgekeerde volgorde uit te voeren. Dit betekent dat de bestaande planningsboodschappen kunnen worden gewijzigd of zelfs worden verwijderd, indien nodig. Het ordertraceringssysteem geeft altijd het nettoresultaat van berekeningen weer aan de gebruiker.  

## <a name="order-tracking-and-planning"></a>Ordertracering en planning

Wanneer het planningssysteem wordt uitgevoerd, worden alle bestaande ordertraceringsrecords en planningsboodschapposten verwijderd en opnieuw gemaakt als planningsregelvoorstellen volgens vraag-voorzieningcombinaties en prioriteiten. Wanneer de planning is voltooid, is het ordernetwerk in evenwicht.  

### <a name="planning-system-versus-order-tracking-and-action-messaging"></a>Planningssysteem versus ordertracering en planningsboodschappen

 In de volgende vergelijking worden de verschillen getoond tussen de methoden die door het planningssysteem worden gebruikt om planningsregelvoorstellen te maken, en de methoden die door het ordertraceringssysteem worden gebruikt om ordertraceringsrecords en planningsboodschappen te maken.  

- Het planningssysteem verwerkt het volledige vraag-voorzieningpatroon van een bepaald artikel, terwijl ordertracering de order verwerkt waardoor deze is geactiveerd.  

- Het planningssysteem verwerkt alle niveaus van de stuklijsthiërarchie, terwijl ordertracering één stuklijstniveau per keer verwerkt.  

- Het planningssysteem legt koppelingen tussen vraag en voorzieningen op basis van de prioriteitsvervaldatum. Ordertracering creëert koppelingen tussen vraag en aanbod op basis van de orderinvoervolgorde.  

- Het planningssysteem houdt rekening met planningsparameters, terwijl ordertracking dat niet doet.  

- Het planningssysteem maakt koppelingen in een door de gebruiker geactiveerde batchmodus wanneer vraag en voorziening worden vereffend, terwijl bij ordertracering de koppelingen automatisch en dynamisch worden gemaakt wanneer de gebruiker orders invoert.  

## <a name="see-also"></a>Zie ook

[Ontwerpdetails: Centrale begrippen van het planningssysteem](design-details-central-concepts-of-the-planning-system.md)  
[Ontwerpdetails: Voorzieningsplanning](design-details-supply-planning.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
