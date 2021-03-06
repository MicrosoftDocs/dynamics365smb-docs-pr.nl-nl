---
title: 'Procedure: Vooruitbetalingen verkoop instellen en factureren'
description: Vooruitbetalingen zijn betalingen die worden gefactureerd en geboekt naar een verkoop- of inkoopvooruitbetalingsorder vóór de definitieve facturering. U kunt een aanbetaling vragen voordat u bestelde artikelen fabriceert, of u kunt een betaling vragen voordat u artikelen naar een klant verzendt. Met de vooruitbetalingsfunctionaliteit in Business Central kunt u vereiste borgsommen factureren en innen van klanten of kunt u borgsommen overmaken aan leveranciers. Zodoende zorgt u dat alle betalingen worden geboekt tegen een factuur.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 05/25/2021
ms.author: edupont
ms.openlocfilehash: dacf9e5492f583513e69f2316a0440fce2597269
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216177"
---
# <a name="walkthrough-setting-up-and-invoicing-sales-prepayments"></a>Procedure: Vooruitbetalingen verkoop instellen en factureren

<!-- [!INCLUDE[complete_sample_data](includes/complete_sample_data.md)]   -->

Vooruitbetalingen zijn betalingen die worden gefactureerd en geboekt naar een verkoop- of inkoopvooruitbetalingsorder vóór de definitieve facturering. U kunt een aanbetaling vragen voordat u bestelde artikelen fabriceert, of u kunt een betaling vragen voordat u artikelen naar een klant verzendt. Met de vooruitbetalingsfunctionaliteit in [!INCLUDE[prod_short](includes/prod_short.md)] kunt u vereiste borgsommen factureren en innen van klanten of kunt u borgsommen overmaken aan leveranciers. Zodoende zorgt u dat alle betalingen worden geboekt tegen een factuur.  

Vooruitbetalingsvereisten kunnen worden gedefinieerd voor een klant of leverancier, voor alle artikelen of bepaalde artikelen. Nadat u de benodigde instellingen hebt gemaakt, kunt u vooruitbetalingsfacturen genereren van verkoop- en inkooporders voor het berekende vooruitbetalingsbedrag. U kunt indien nodig de standaardbedragen op de facturen wijzigen. U kunt bijvoorbeeld tevens aanvullende vooruitbetalingsfacturen versturen, als er extra artikelen worden toegevoegd aan de order.  

## <a name="about-this-walkthrough"></a>Informatie over deze procedure  

In deze procedure komen de volgende scenario's aan de orde:  

-  Vooruitbetalingen instellen  
-  Een order maken waarvoor een vooruitbetaling vereist is  
-  Een vooruitbetalingsfactuur maken  
-  De vooruitbetalingsvereisten voor een order aanpassen  
-  Vooruitbetalingen vereffenen met een order  
-  Het uiteindelijke bedrag van een order met vooruitbetaling factureren  

### <a name="roles"></a>Rollen

Deze procedure bevat taken voor de volgende rollen:  

-  Administrateur (Phyllis)  
-  Orderverwerker (Susan)  
-  Administratie vorderingen (Arnie)  

## <a name="story"></a>Scenario

 Phyllis is administrateur. Ze is administrateur en bepaalt welke klanten een aanbetaling moeten doen voordat artikelen worden gefabriceerd of verzonden. Phyllis stelt [!INCLUDE[prod_short](includes/prod_short.md)] in op het automatisch berekenen van vooruitbetalingen.  

 Susan is verkooporderverwerker. Als een klant belt om een order te plaatsen, voert ze de order in het systeem in terwijl ze de klant aan de telefoon heeft. Op deze manier kan ze prijzen en betalingsvoorwaarden meteen met de klant controleren en ze kan de order aanpassen terwijl ze met de klant onderhandelt.  

 Arnie werkt op de afdeling Vorderingen, waar hij facturen en betalingen boekt.  

 In dit scenario stelt Phyllis de vereisten voor vooruitbetalingen in voor de klant Selangorian. Ze baseert dit op hun historische betalingsgegevens en geeft Susan instructies voor het afhandelen van hun orders.  

 Wanneer de klant belt, onderhandelt Susan met de klant totdat een overeenkomst wordt bereikt. Ze kan de vooruitbetaling vervolgens op verschillende manieren berekenen.  

 Nadat Susan de vooruitbetalingsfactuur heeft verstuurd, bestelt te klant een extra artikel. Susan werkt de order bij en maakt een tweede vooruitbetalingsfactuur.  

 Arnie registreert de betaling van de klant en past deze toe op de facturen, waarna hij de uiteindelijke factuur stuurt.  

## <a name="setting-up-prepayments"></a>Vooruitbetalingen instellen

Als administrateur stelt Phyllis het systeem in voor het verwerken van vooruitbetalingen van klanten.  

-  Phyllis besluit voor de vooruitbetalingen dezelfde nummerreeks te gebruiken als voor de verkoopfacturen.  
-  Phyllis stelt de toepassing in om te controleren of vooruitbetalingen zijn vereist voordat de uiteindelijke factuur voor een order wordt verzonden.  
-  Phyllis stelt standaardwaarden in voor een vereist vooruitbetalingspercentage voor bepaalde artikelen en klanten.  

In de volgende procedures wordt beschreven hoe de taken van Phyllis worden uitgevoerd:  

#### <a name="to-set-up-number-series-for-prepayments"></a>Nummerreeks voor vooruitbetalingen instellen

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Verkoopinstellingen** in en kies de desbetreffende koppeling.  
2.  Vouw op de pagina **Verkoopinstellingen** het sneltabblad **Nummerreeks** uit.  
3.  Controleer of de nummerreeks voor geboekte vooruitbetalingsfacturen in het veld **Geboekte vooruitbetalingsfactuurnrs.** overeenkomt met de reeks voor geboekte verkoopfacturen (**Factuurnrs. (Geboekt)**) en of de nummerreeks voor geboekte vooruitbetalingscreditnota's (**Geboekte vooruitbetalingscreditnotanrs.**) overeenkomt met de reeks voor geboekte creditnota's (**Creditnotanrs. (Geboekt)**).  

#### <a name="to-block-shipments-for-unpaid-prepayment"></a>Verzendingen blokkeren voor niet voldane vooruitbetalingen

1.  Schakel op de pagina **Verkoopinstellingen** op het sneltabblad **Algemeen** het selectievakje **Vooruitbetaling controleren bij boeken** in.

Vanaf dit moment kunt geen orders verzenden of factureren waarvoor een niet-betaald vooruitbetalingsbedrag openstaat.  

Phyllis stelt in dat bij klant 20000 standaard een aanbetaling van 30% voor alle orders moet worden gefactureerd. Daarom voert ze een standaardpercentage voor vooruitbetaling in voor de klant.  

Phyllis stelt in dat bij alle klanten een aanbetaling van 20% wordt gefactureerd voor artikel 1896-S. Klant 20000 heeft een slechte betalingsgeschiedenis. Daarom vereist zij een 40%-vooruitbetaling van klant 20000 voor artikel 1896-S. In de volgende procedure wordt beschreven hoe de aanbetalingspercentages worden ingesteld.  

#### <a name="to-assign-default-prepayment-percentages-to-customers-and-items"></a>Standaardpercentages voorvooruitbetaling toewijzen aan klanten en artikelen

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Klanten** in en kies de gerelateerde koppeling.  
2.  Open de kaart voor klant 20000 (Trey Research).
3.  Typ **30** in het veld **Vooruitbetaling %**.  
4.  Selecteer **Verwant**, selecteer dan **Verkoop** en dan **Vooruitbetalingspercentages**
5.  Vul twee regels op de pagina **Vooruitbetalingspercentages verkoop** als volgt in.  

    |**Verkoopsoort**|**Verkoopscode**|**Artikelnr.**|**Vooruitbetaling %**|  
    |--------------------|--------------------|------------------|----------------------|  
    |**Klant**|**20000**|**1896-S**|**40**|  
    |**Alle klanten**| |**1896-S**|**20**|  

    > [!IMPORTANT]  
    >  Afhankelijk van uw land/regio, moet u voor artikel 1896-S ook een belastinggroepcode opgeven op het sneltabblad **Facturering**.  

6.  Sluit alle pagina's.  

#### <a name="to-specify-an-account-for-sales-prepayments-in-general-posting-setup"></a>Een vooruitbetalingsrekening verkoop opgeven in de boekingsgroepinstellingen

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Boekingsgroepinstellingen** in en kies de desbetreffende koppeling.  
2.  Selecteer de regel waar de **Bedrijfsboekingsgroep** is ingesteld op **BINNENLAND** en de **Productboekingsgroep** op **DETAILHANDEL**.  
3.  Geef in het veld **Vooruitbetalingsrekening verkoop** de relevante rekening op. Uw selectie wordt automatisch opgeslagen.  

## <a name="creating-an-order-that-requires-a-prepayment"></a>Een order maken waarvoor vooruitbetaling is vereist

 In het volgende scenario maakt Susan, de orderprocessor, een order terwijl ze met een klant praat. Voor de artikelen die de klant bestelt is een vooruitbetaling vereist en de klant heeft in het verleden een aantal keer te laat betaald. Susan heeft daarom de instructie gekregen om een vast bedrag van **800** als vooruitbetaling op de order te eisen.  

De klant vraagt of het goed is als hij 35% betaalt, een voorstel waarin Susan zich kan vinden. Zij wijzigt daarom de order.  

Susan maakt de vooruitbetalingsfactuur en verzendt deze naar de klant.  

#### <a name="to-create-a-sales-order-with-a-prepayment"></a>Een verkooporder maken met een vooruitbetaling

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Verkooporders** in en kies de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Kies in het veld **Klantnr.** de waarde **20000**.  
4.  Accepteer de waarschuwing voor openstaand saldo die verschijnt.  
5.  Vul op twee verkoopregels de volgende gegevens in.  

    |**Soort**|**Nr.**|**Aantal**|  
    |--------------|-------------|------------------|  
    |**Artikel**|**1896-S**|**1**|  
    |**Artikel**|**1900-S**|**1**|

    De vooruitbetalingsvelden op de verkoopregel zijn standaard verborgen, dus u moet ze weergeven. Hiervoor moet u de pagina personaliseren. Zie voor meer informatie [Een pagina personaliseren via de banner Personaliseren](ui-personalization-user.md#to-start-personalizing-a-page-through-the-personalizing-banner).

6.  Controleer of het veld **Vooruitbetaling %** op de regel voor artikel **1900-S** op **30** staat. Dit is standaard overgenomen van de verkoopkop die wordt gevuld op basis van de klantkaart.  

    Het veld **Vooruitbetaling %** op de regel voor artikel **1896-S** is **40**. Dit is het percentage dat u hebt ingevoerd op de pagina **Vooruitbetalingspercentages verkoop** voor artikel **1896-S** en klant **20000**.  

    Zie voor meer informatie [Vooruitbetalingen instellen](finance-set-up-prepayments.md) voor meer informatie.  
7.  Kies bij de actie **Order** **Statistieken**.  
8.  Op het sneltabblad **Vooruitbetaling** bevat het veld **Vooruitbetalingsregelbedrag excl. btw** het bedrag **458.16**. Als u nu een vooruitbetalingsfavtuur voor de order maakt, is dit het bedrag dat op de factuur wordt weergegeven.  

    In dit scenario heeft Susan instructies ontvangen om een totale vooruitbetaling van **800** voor te stellen voor de order.  

    > [!IMPORTANT]  
    >  De volgende stap kunt u in uw land\regio misschien niet uitvoeren.  
9.  Wijzig het bedrag in het veld **Vooruitbetalingsregelbedrag excl. btw** in **800** en sluit de pagina.  
10.  Controleer het veld **Vooruitbetaling %** op de verkoopregels en u ziet dat dit is herberekend als **67,02438** en **67,02282**.  

     Bij de herberekening zijn alle regels meegenomen die een vooruitbetalingspercentage hebben dat hoger is dan 0.  

     De klant vraagt nu of het vooruitbetalingspercentage op 35% kan worden gezet. De leidinggevende van Susan keurt de wijziging goed.
11.  Voer op de pagina **Verkooporder** op het sneltabblad **Vooruitbetaling** in het veld **Vooruitbetaling %** de waarde **35** in.  
12.  In de waarschuwing die wordt weergegeven, kiest u de knop **Ja**. Er wordt een tarief van 35% toegepast als het betalingspercentage voor de hele order.  
13.  Controleer of de regels juist zijn bijgewerkt.  

## <a name="creating-a-prepayment-invoice"></a>Een vooruitbetalingsfactuur maken  
Nadat de juiste vooruitbetalingswaarden voor de order zijn ingevoerd, maakt Susan de vooruitbetalingsfactuur en stuurt ze deze naar de klant.  

#### <a name="to-create-a-prepayment-invoice"></a>Een vooruitbetalingsfactuur maken

1.  Kies op de pagina **Verkooporder** **Acties**, vervolgens **Boeking**, dan **Vooruitbetaling** en selecteer vervolgens **Vooruitbetalingsfactuur boeken en afdrukken**
2.  Kies de knop **Ja** om de factuur te boeken.  

> [!NOTE]  
>  Susan zou **Vooruitbetalingsfactuur boeken en afdrukken** kiezen en de factuur naar de klant verzenden.  

## <a name="creating-an-additional-prepayment-invoice"></a>Een extra vooruitbetalingsfactuur maken

De volgende dag belt de klant op en vraagt Susan om een wijziging in de order te maken. De klant wil twee stuks van artikel 1100. Susan opent de order en wijzigt deze en maakt vervolgens een tweede vooruitbetalingsfactuur voor de order en stuurt deze naar de klant.  

#### <a name="to-create-an-additional-prepayment-invoice"></a>Een extra vooruitbetalingsfactuur maken

1.  Kies op de pagina **Verkooporder** de actie **Vrijgeven** en dan **Opnieuw openen**.  
2.  Typ **2** in het veld **Aantal** voor artikel **1896-S**.  

    Kies bij de actie **Order** **Statistieken**. Het veld **Vooruitbetalingsregelbedrag excl. btw** bevat nu **768.04** en het veld **Gefactureerd vooruitbetalingsbedrag excl. btw** bevat **417.76**. Dit geeft aan dat er een extra vooruitbetalingsbedrag bestaat dat nog niet is gefactureerd.  
3.  Als u een factuur wilt boeken voor het extra vooruitbetalingsbedrag, kiest u **Acties**, dan **Boeking**, dan **Vooruitbetaling** en selecteert u **Vooruitbetalingsfactuur boeken en afdrukken**
4.  Kies de knop **Ja** om de factuur te boeken.  

## <a name="applying-the-prepayments"></a>Vooruitbetalingen vereffenen  
De klant betaalt het vooruitbetalingsbedrag en Arnie, die op de afdeling Vorderingen werkt, registreert de betaling en vereffent deze met de vooruitbetalingsfacturen.  

#### <a name="to-apply-a-payment-to-the-prepayment-invoices"></a>Een betaling vereffenen met vooruitbetalingsfacturen

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Ontvangstendagboeken** in en kies de gerelateerde koppeling.  
2.  Vul op een dagboekregel de volgende gegevens in.  

    |Veldnaam|Voer in|  
    |----------------|-----------|  
    |**Documentsoort**|**Betaling**|  
    |**Rekeningsoort**|**Klant**|  
    |**Rekeningnr.**|**20000**|  
3.  Kies de actie **Verwerken** en dan **Posten vereffenen**.  
4.  Selecteer op de pagina **Klantenposten vereffenen** de eerste vooruitbetalingsfactuur en kies vervolgens de actie **Verwerken** en dan **Vereffenings-id instellen**.  
5.  Herhaal de vorige stap voor de tweede vooruitbetaling.  
6.  Kies de knop **Ok**.  

    In het bedragveld is nu het totaal van de twee vooruitbetalingsfacturen ingevuld.  

7.  Om het journaal te boeken kiest u de actie **Boeken/afdrukken** en selecteert u vervolgens **Boeken**.
8.  Kies de knop **Ja**.

## <a name="invoicing-the-remaining-amount"></a>Het resterende bedrag factureren

Arnie heeft nu doorgekregen dat de artikelen voor de order zijn verzonden en dat de order gereed is voor facturering. Arnie maakt de factuur voor de order.  

#### <a name="to-invoice-the-remaining-amount"></a>Het resterende bedrag factureren

1.  Open de verkooporder.
2.  Kies de actie **Boeking** en dan **Boeken**.
3.  Klik op **Verzenden en factureren** en kies vervolgens **OK**.
4.  Klik op de knop **Ja** als u een voorbeeld van de factuur wilt bekijken.

> [!NOTE]  
>  Gewoonlijk heeft de verzendafdeling de verzending al geboekt.  

Arnie kan de geschiedenis bekijken om te controleren of de verkoopfactuur volgens plan is gemaakt.

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Geboekte verkoopfacturen** in en kies vervolgens de desbetreffende koppeling.  

## <a name="next-steps"></a>Volgende stappen

In dit overzicht hebt u de stappen doorlopen om [!INCLUDE[prod_short](includes/prod_short.md)] in te stellen voor het afhandelen van vooruitbetalingen. U hebt gezien hoe u standaard vooruitbetalingspercentages voor klanten en artikelen kunt instellen, en u hebt verschillende methoden gebruikt om de vooruitbetalingen van een order te berekenen. U hebt geprobeerd één totaal vooruitbetalingsbedrag aan de order toe te wijzen en u hebt het vooruitbetalingsbedrag laten berekenen als een percentage van de gehele order.  

Ook hebt u geleerd hoe u een vooruitbetalingsfactuur boekt, een tweede vooruitbetalingsfactuur maakt als de order wordt gewijzigd en de uiteindelijke factuur boekt voor het resterende bedrag.  

De functie voor vooruitbetalingen in [!INCLUDE[prod_short](includes/prod_short.md)] maakt het eenvoudig om vooruitbetalingsregels voor klanten en artikelen in te stellen en stelt u in staat om alle betalingen tegen een factuur te boeken.  

## <a name="see-also"></a>Zie ook  
[Vooruitbetalingen factureren](finance-invoice-prepayments.md)  
[Financiën](finance.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Procedures voor bedrijfsprocessen](walkthrough-business-process-walkthroughs.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
