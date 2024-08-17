---
title: Artikelen overbrengen tussen magazijnvestigingen
description: 'Leer hoe u voorraad verplaatst van de ene plaats of magazijn naar een andere, met het herindelingsdagboek of met transferorders.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 08/12/2024
ms.custom: bap-template
ms.search.keywords: 'move, warehouse'
ms.search.forms: '5746, 5745, 5759, 5753, 5743, 5758, 5752, 5744, 5749, 5740, 5741, 5742, 5757, 5748, 5747, 9285, 5756, 5755'
ms.service: dynamics-365-business-central
---

# Voorraad overbrengen tussen vestigingen

U kunt voorraadartikelen tussen vestigingen overbrengen door transferorders te maken. U kunt ook het artikelherindelingsdagboek gebruiken.

> [!NOTE]
> Als u artikelen wilt overbrengen, moet u locaties en transferroutes instellen. Ga naar  [Locaties instellen voor meer informatie over het instellen van locaties](inventory-how-setup-locations.md). U kunt geen transferorders gebruiken voor *lege* locaties.

## Transferorders

U kunt een uitgaande transfer vanuit de ene vestiging verzenden en een inkomende transfer op de bestemming ontvangen. U kunt het volgende doen:

* Volg een hoeveelheid die onderweg is.
* Definieer agenda's, bewerkingsplannen en inkomende en uitgaande verwerkingstijden voor datumberekening en planning. Ga voor meer informatie over planning naar [Over planningsfunctionaliteit](production-about-planning-functionality.md).
* Gebruik verschillende magazijnfuncties voor inkomende en uitgaande locaties.
* Gebruik met enkele beperkingen transferorders voor directe transfers.

## Artikelherindelingsdagboeken

U kunt de pagina **Artikelherindelingsdagboek** gebruiken voor het volgende:

* Directe transfer van artikelen tussen locaties.
* Verplaats items tussen bakken. Ga naar [Verplaats items ongepland in basismagazijnconfiguraties voor meer informatie over het verplaatsen van items tussen bakken](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md).
* Wijzig een lot- of serienummer in een nieuw lot- of serienummer. Ga voor meer informatie over het herindelen van serie- en lotnummers naar [Serie- of lotnummers herindelen](inventory-how-work-item-tracking.md#to-reclassify-serial-or-lot-numbers).
* De vervaldatum in een nieuwe datum veranderen.
* Herindeel artikelen van een lege locatie naar een daadwerkelijke locatie.
* Magazijnposten maken als u geen magazijnactiviteiten beheert.

## Artikelen overbrengen met een transferorder

1. Kies het pictogram ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transferorders** in en kies vervolgens de gerelateerde koppeling
2. Vul op de pagina **Transferorder** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Als u tijdens het instellen van de transferroute de velden **Transitcode**, **Expediteur** en **Expediteurservice** op de pagina **Transferroutegegevens** hebt ingevuld, worden de bijbehorende velden op de transferorder automatisch ingevuld.

    Wanneer u het veld **Servicecode expediteur** invult, wordt de ontvangstdatum in de ontvangstvestiging berekend door de verzendtijd van de expediteurservice op te tellen bij de verzenddatum.

3. Er zijn verschillende manieren om de regels in te vullen:

    |Optie  |Omschrijving  |
    |---------|---------|
    |Handmatig     | Vul op het sneltabblad **Regels** een regel in voor een artikel of gebruik de actie **Artikelen selecteren** om meerdere artikelen te kiezen.        |
    |Automatisch     | * Kies de actie **Opslaglocatie-inhoud ophalen** om bestaande artikelen uit een specifieke opslaglocatie te selecteren.<br><br>* Kies **Ontvangstregels ophalen** om artikelen te selecteren die net zijn aangekomen op de aflevervestiging.        |

    U kunt de artikelen nu verzenden.
4. Kies de actie **Boeken**, kies de optie **Verzenden** en kies vervolgens de knop **OK**.

    De artikelen zijn nu in transit tussen de opgegeven vestigingen volgens de opgegeven transferroute.

    Als magazijnmedewerker op de aflevervestiging gaat u verder om de artikelen te ontvangen. De tranferorderregels zijn dezelfde als bij verzending en kunnen niet worden bewerkt.
5. Kies de actie **Boeken**, kies de optie **Ontvangen** en kies vervolgens de knop **OK**.

### Een transferverzending ongedaan maken

Als u een fout vindt in een hoeveelheid op een geboekte transferorder, kunt u de hoeveelheid eenvoudig corrigeren zolang de zending niet is ontvangen. Op de pagina  **Geboekte overdrachtszending** maakt de actie  **Zending ongedaan maken** correctieregels aan, als volgt:

* De waarde in het veld **Verzonden aantal** wordt verlaagd met de hoeveelheid die u ongedaan hebt gemaakt.
* De waarde in het veld **Te verzenden aantal** wordt verhoogd met de hoeveelheid die u ongedaan hebt gemaakt.
* Het selectievakje **Correctie** is ingeschakeld voor de regels.

Als de verzonden hoeveelheid in een magazijnzending is, wordt er een correctieregel aangemaakt in de geboekte magazijnzending.

Om de correctie te voltooien, heropent u de transferorder, voert u het juiste aantal in en boekt u de order. Als u een magazijnverzending gebruikt om de bestelling te verzenden, maakt en boekt u een nieuwe magazijnverzending.

### Meerdere overboekingsopdrachten in een batch boeken

In de volgende procedure wordt uitgelegd hoe u transferorders in een batch boekt.

1. 1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transferorders** in en kies vervolgens de gerelateerde koppeling  
2. Selecteer op de pagina **Transferorders** de orders die u wilt boeken.
3. In het veld **Nr.** opent u het contextmenu en kiest u **Meer selecteren**.
4. Schakel het selectievakje in voor de regels voor elke order die u wilt boeken.
5. Kies de actie  **Post**  en kies vervolgens  **Batch posten**.
6. Vul op de pagina **Transferorderrecord per batch boeken** de benodigde velden in.

   > [!TIP]
    > Voor transferorders die een transitvestiging gebruiken, kunt u **Verzenden** of **Ontvangen** kiezen. Herhaal deze stap als u beide moet doen. Voor oders waar **Direct boeken** is ingeschakeld, werken beide opties op dezelfde manier en wordt de order volledig geboekt.

7. Selecteer **OK**.
8. Om mogelijke problemen te bekijken, opent u de pagina **Foutberichtregister**.

    > [!NOTE]
    > Het boeken van meerdere documenten kan enige tijd duren en andere gebruikers blokkeren. Overweeg om boeken op de achtergrond in te schakelen. Zie voor meer informatie [Gebruik van taakwachtrijen om taken te plannen](/dynamics365/business-central/admin-job-queues-schedule-tasks).

### Plan een taakwachtrijpost om meerdere documenten in een batch te boeken

U kunt ook de taakwachtrij gebruiken om boekingen te plannen op een tijdstip dat het uw organisatie uitkomt. Het kan bijvoorbeeld zinvol zijn voor uw bedrijf om bepaalde routines uit te voeren wanneer de meeste gegevensinvoer voor die dag is gedaan.

In de volgende procedure wordt getoond hoe u het rapport **Transferorders per batch boeken** instelt om op werkdagen om 16.00 uur automatisch directe transferorders te boeken. Die tijd wordt slechts als voorbeeld gebruikt. De stappen zijn hetzelfde voor andere documenten.  

1. Zoek de pagina **Taakwachtrijposten** op en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Nieuw**.  
3. Selecteer in het veld **Uit te voeren objecttype** **Rapport**.  
4. Selecteer in het veld **Uit te voeren object-id** de optie **5707, Transferorders per batch boeken**.
5. Selecteer het selectievakje **Rapportaanvraagpagina**.
6. Kies op de aanvraagpagina **Transferorders per batch boeken** de optie **Verzenden**, filter op **Directe transfer** en selecteer vervolgens **OK**.

   > [!IMPORTANT]
   > Het is belangrijk om filters in te stellen. Anders zal [!INCLUDE [prod_short](includes/prod_short.md)] alle documenten boeken, zelfs als ze nog niet klaar zijn. U kunt overwegen een filter in te stellen voor het veld **Status** met de waarde **Vrijgegeven** en een filter in te stellen voor het veld **Boekingsdatum** met de waarde **..vandaag**. Ga voor meer informatie over filters naar [Sorteren, zoeken en filteren](/dynamics365/business-central/ui-enter-criteria-filters).

7. Selecteer alle selectievakjes van **Uitvoeren op maandagen** tot **Uitvoeren op vrijdagen**.
8. Voer in het veld **Starttijd** de waarde **4 PM** in.
9. Kies de actie **Status instellen op Gereed**.

### Vergelijking van verschillende instellingen voor overdrachtsopdrachten

U kunt overdrachtsopdrachten op verschillende manieren plaatsen, met of zonder een in-transitlocatie. Schakel de schakelaar  **Directe overdracht** uit en selecteer de tijdelijke locatie in het veld  **In transitcode** op de pagina  **Overdrachtsopdracht** . Wanneer u de verzending van een overdrachtsorder boekt die gebruikmaakt van de locatie 'in transit', zijn de artikelen op de regel niet langer beschikbaar op een van uw locaties omdat ze onderweg zijn. Directe boeking zorgt ervoor dat er geen gebruik wordt gemaakt van een in-transitlocatie en dat het verzend- en ontvangstproces gelijktijdig plaatsvinden. Het exacte gedrag van directe boeking kan verschillen, afhankelijk van de waarde die is geselecteerd in het veld  **Directe overboeking** op de pagina  **Voorraadinstellingen** .

De onderstaande tabel beschrijft hoe de combinaties verschillen.

|Mogelijkheid|Het veld  **Directe overdracht** is uitgeschakeld op de pagina  **Overdrachtsopdracht** |**Directe overschrijving** is ingeschakeld op de pagina **Overboekingsopdracht** </br>**Directe overdrachtsboeking** is ingesteld op **Directe overdracht** op de **pagina Inventarisinstellingen** |**Directe overdracht** is ingeschakeld op de pagina **Overdrachtsopdracht** </br>**Directe overdrachtsboeking** is ingesteld op **Ontvangst en verzending** op de pagina **Inventarisinstellingen** |
|---|---|---|---|
|Gebruik de locatie tijdens het transport|Ja|Nr.|Nr.|
|Kan een ontvangstbewijs verzenden zonder verzending.</br>Kan  **Ongedaan maken ontvangstbewijs** gebruiken.|Ja|Nr.|Nr.|
|Gedeeltelijke plaatsing|Ja|Nr.|Ja|
|Artikelposten|4:</br>Transfer van Van-Locatie,</br>Overdracht naar In-Transit,</br>Overstappen van In-Transit,</br>Overbrengen naar de locatie.|2:</br>Transfer van Van-Locatie,</br>Overbrengen naar de locatie.|4:</br>Transfer van Van-Locatie,</br>Overbrengen naar *blanco*,</br>Overdracht van *blanco*,</br>Overbrengen naar de gewenste locatie.|
|Geboekte documenten|Geposte transferzending,</br>Overdrachtsbewijs verzonden.|Directe overdracht geplaatst|Geposte transferzending,</br>Overdrachtsbewijs verzonden.|
|Reservering: inkomende en uitgaande vluchten|Ja|Ja|Ja|
|Artikelkosten - toewijzen aan geboekte overdrachtsontvangst|Ja|Nr.|Ja|
|Magazijnafhandeling|Volledig|Nr.|Beperkt, zie hieronder|

Matrix voor magazijnafhandeling voor configuratie: **Directe overdracht** is ingeschakeld op de pagina **Overdrachtsorder**  en **Directe overdrachtsboeking** is ingesteld op **Directe overdracht** op de pagina **Voorraadinstellingen** .

|Van \ Naar|Naar: Geen magazijnafhandeling|Aan: Magazijnontvangst|Naar: Inventaris wegzetten|Aan: Gerichte opslag en pick|
|-|-|-|-|-|
|**Van: Geen magazijnafhandeling**|1|Niet ondersteund|1, 4|Niet ondersteund|
|**Van: Magazijnzending**|1, 2|Niet ondersteund|1,2,4|Niet ondersteund|
|**Van: Inventaris wegzetten**|1, 3|Niet ondersteund|1,3,4|Niet ondersteund|
|**Van: Geregisseerde opslag en pick**|2|Niet ondersteund|2|Niet ondersteund|

De getallen in de cellen geven aan welke boekingsopties worden ondersteund.

1. Post van overdrachtsopdracht. Voor sommige combinaties moet u mogelijk het veld  **Te verzenden aantal**  invullen.
2. Een magazijnzending aanmaken en boeken.
3. Maak en publiceer een inventarisselectie.
4. Maak en boek een inventarisatie. Voor sommige combinaties moet u mogelijk het veld  **Te verzenden aantal** invullen.

Ongeacht de methode worden de verzend- en ontvangsttransacties uitgevoerd. U kunt bijvoorbeeld een overdrachtsorder maken van een locatie waar voorraad moet worden verzameld naar een locatie waar voorraad moet worden weggezet. U kunt de voorraadopslag aanmaken en boeken, en zowel de verzend- als ontvangsttransacties worden aangemaakt. U kunt dergelijke documenten ook boeken vanuit een overdrachtsorder of vanuit een inventarisatie.  

Voor meer informatie over magazijnbeheer, zie  [Overzicht magazijnbeheer](design-details-warehouse-management.md).

## Artikelen overbrengen met het artikelherindelingsdagboek

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Artikelherindelingsdagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Vul op de pagina **Artikelherindelingsdagboeken** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. Voer in het veld **Vestiging** de vestiging in waar de artikelen momenteel zijn opgeslagen.

    > [!NOTE]  
    > Als u artikelen wilt overbrengen die geen vestigingscode hebben, laat u het veld **Vestiging** leeg.
4. Voer in het veld **Nieuwe vestiging** de vestiging in waarnaar u de artikelen wilt overbrengen.
5. Kies de actie **Boeken**.

    [!INCLUDE [preview-posting-inventory](includes/preview-posting-inventory.md)]


## Zie ook

[Voorraad beheren](inventory-manage-inventory.md)  
[Vestigingen instellen](inventory-how-setup-locations.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Wijzigen welke functies worden weergegeven](ui-experiences.md)  
[Algemene bedrijfsfunctionaliteit](ui-across-business-areas.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
