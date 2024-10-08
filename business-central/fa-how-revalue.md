---
title: Vaste activa herwaarderen
description: 'Meer informatie over hoe u de waarde van vaste activa aanpast, nieuwe bedragen vastlegt als waardevermindering of waardevermeerdering en andere aanschafkosten boekt.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.form: '5628, 5629, 5633'
ms.date: 02/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="revalue-fixed-assets"></a>Vaste activa herwaarderen

De herwaardering van vaste activa kan bestaan uit waardevermeerderingen, waardeverminderingen of algemene waardecorrecties.

Als de waarde van een vast activum stijgt, boekt u een dagboekregel met een waardevermeerdering naar het afschrijvingsboek. Het nieuwe bedrag wordt als een waardevermeerdering vastgelegd op basis van de instelling van de boeking van het vaste activum.

Als de waarde van een vast activum daalt, boekt u een dagboekregel met een lager bedrag, een waardevermindering naar het afschrijvingsboek. Het nieuwe bedrag wordt als een waardevermindering vastgelegd op basis van de instelling van de boeking van het vaste activum.

Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen. Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen.

## <a name="to-post-appreciation-from-the-fixed-asset-gl-journal"></a>Een waardevermeerdering boeken vanuit het financieel dagboek voor vaste activa

1. Kies het pictogram ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **VA-fin. dagboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Maak een eerste dagboekregel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Herwaardering**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermeerdering is ingesteld.

    > [!NOTE]  
    >   Stap 4 werkt alleen als u het volgende hebt ingesteld: op de pagina **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardevermeerderingsrek.** de grootboekdebetrekening en het veld **Tegenrek. waardevermeerdering** bevat de grootboekrekening waarnaar u tegenrekeningsposten voor afschrijving wilt boeken. Zie [Boekingsgroepen voor vaste activa instellen](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups) voor meer informatie.  
5. Kies de actie **Boeken**.

## <a name="to-post-a-write-down-from-the-fixed-asset-gl-journal"></a>Een waardevermindering boeken vanuit het financieel dagboek voor vaste activa

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **VA-fin. dagboeken** in en kies vervolgens de gerelateerde koppeling.  
2. Maak een eerste dagboekregel en vul de velden indien nodig in.
3. In het veld **VA-boekingssoort** selecteert u **Waardevermindering**.
4. Kies de actie **VA-tegenrekening invoegen**. Er wordt een tweede dagboekregel gemaakt voor de tegenrekening die voor de boeking van de waardevermindering is ingesteld.

    > [!NOTE]  
    >   Stap 4 werkt alleen als u het volgende hebt ingesteld: op de pagina **VA-boekingsgroep** voor de boekingsgroep van het vaste activum bevat het veld **Waardeverminderingsrekening** de grootboekrekening en het veld **Waardeverminderingskostenrekening** bevat de grootboekdebetrekening waarnaar u tegenrekeningsposten voor waardeverminderingen wilt boeken. Zie [Boekingsgroepen voor vaste activa instellen](fa-how-setup-general.md#to-set-up-fixed-asset-posting-groups) voor meer informatie.
5. Kies de actie **Boeken**.

## <a name="to-perform-general-revaluation-of-fixed-assets"></a>Algemene herwaardering van vaste activa uitvoeren

Indexering wordt gebruikt om meerdere waarden voor vaste activa aan te passen op basis van algemene prijswijzigingen. Met de batchverwerking **Vaste activa indexeren** kunt u diverse bedragen wijzigen, zoals waardeverminderingsbedragen en waardevermeerderingsbedragen. Het selectievakje **Indexering toegestaan** op de pagina **Afschrijvingsboek** moet zijn ingeschakeld.

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Vast activum indexeren** in en kies vervolgens de gerelateerde koppeling.  
2. Vul indien nodig de velden in.
3. Kies de knop **Ok**.

    De herwaardering regels worden gemaakt op basis van uw instellingen in stap 2. De regels worden gemaakt in het dagboek voor vaste activa of het financieel dagboek voor vaste activa, afhankelijk van uw sjabloon en batchinstellingen op de pagina **VA-dagboekinstellingen**. Zie [Algemene gegevens voor vaste activa instellen](fa-how-setup-general.md) voor meer informatie.
4. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **VA-fin. dagboeken** in en kies vervolgens de gerelateerde koppeling.  
5. Selecteer het dagboek met de vaste activa die u wilt herwaarderen en kies vervolgens de actie **Posten**.  
6. Controleer de gemaakte posten en kies vervolgens de actie **Boeken** om het dagboek te boeken.

    > [!TIP]  
    >   Als de indexcijfers alleen voor simulaties worden gebruikt, kunt u een speciaal afschrijvingsboek maken om ze in op te slaan. Deze posten zijn dan niet van invloed op de andere afschrijvingsboeken.

## <a name="to-post-other-acquisition-costs"></a>Andere aanschafkosten boeken

U boekt andere aanschafkosten voor een vast activum vanaf een inkoopfactuur of vanuit een dagboek voor vaste activa op dezelfde manier als u de oorspronkelijke aanschafkosten boekt. Zie [Vaste activa aanschaffen](fa-how-acquire.md) voor meer informatie.  

Als de afschrijving al is berekend voor het vaste activum, schakelt u het selectievakje **Afschrijving aanschafkosten** in om de andere aanschafkosten af te schrijven, verminderd met de restwaarde. Dit bedrag is evenredig aan het bedrag dat al op het eerder aangeschafte vaste activum is afgeschreven. Met deze methode wordt ervoor gezorgd dat de afschrijvingsperiode niet wordt gewijzigd.  

Het afschrijvingspercentage wordt als volgt berekend:  

*P = (totale afschrijving x 100) / afschrijvingsbasis*

*Afschrijvingsbedrag = (P/100) x (extra aanschafkosten - restwaarde)*  

Vergeet niet om het selectievakje **Afschrijving tot VA-boekingsdatum** in te schakelen op de factuur en het financieel dagboek voor vaste activa of de dagboekregels voor vaste activa te selecteren om ervoor te zorgen dat de afschrijving wordt berekend vanaf de laatste boekingsdatum voor vaste activa tot de boekingsdatum van de andere aanschafkosten.

### <a name="example---posting-other-acquisition-costs"></a>Voorbeeld - andere aanschafkosten boeken

Een machine is aangeschaft op 1 augustus 2000. De aanschafkosten bedragen LV 4.800. De afschrijvingsmethode is lineair over vier jaar.

Op 31 augustus 2000 wordt de batchverwerking **Afschrijving berekenen** uitgevoerd. De afschrijving wordt berekend als:

*boekwaarde x aantal afschrijvingsdagen/totaal aantal afschrijvingsdagen = 4800 x 30 / 1440 = 100*  

Op 15 september 2000 wordt een factuur geboekt voor het schilderen van de machine. Het factuurbedrag is LV 480.

Als u het selectievakje **Afschrijving tot VA-boekingsdatum** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:  

15 afschrijvingsdagen (09-01-00 t/m 09-15-00) worden berekend als:

*boekwaarde x aantal afschrijvingsdagen/resterend aantal afschrijvingsdagen = (4800 - 100) x 15 / 1410 = 50*

Als u het selectievakje **Afschrijving aanschafkosten** op de factuur hebt ingeschakeld voordat u deze boekt, wordt de volgende berekening gemaakt:  

*De andere aanschafkosten worden afgeschreven als ((150 x 100) / 4800) / 100 x 480 = 15*

De afschrijvingsbasis is nu *5280 = (4800 + 480)* en de gecumuleerde afschrijving is *165 = (100 + 50 + 15)*, wat overeenkomt met 45 afschrijvingsdagen van de totale aanschafkosten. Deze berekening betekent dat het activum volledig wordt afgeschreven binnen de verwachte levensduur van vier jaar.  

Als de batchverwerking **Afschrijving berekenen** wordt uitgevoerd op 30-09-0, wordt de volgende berekening gemaakt:  

*Resterende afschrijfbare levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*  

*Boekwaarde is (5.280 - 165) = LV 5115*  

*Afschrijvingsbedrag voor september 2000: 5115 x 15 / 1395 = 55,00*  

*Totale afschrijving = 165 + 55 = LV 220*  

Als u het selectievakje **Afschrijving tot VA-boekingsdatum** niet hebt ingeschakeld, verliest het activum 15 afschrijvingsdagen omdat de batchverwerking **Afschrijving berekenen** die op 30-09-00 is uitgevoerd, de afschrijving berekent vanaf 15-09-00 t/m 30-09-00. Als de batchverwerking **Afschrijving berekenen** op 30-09-00 wordt uitgevoerd, is de berekening dus als volgt:  

*Resterende levensduur is 3 jaar, 10 maanden en 15 dagen = 1395 dagen*  

*Boekwaarde is (4.800 + 480 - 100 - 15) = LV 5165*

*Afschrijvingsbedrag voor september 2000: 5165 x 15 / 1395 = 55,54*  

*Totale afschrijving = 100 +15 + 55,54 = LV 170,54*

## <a name="see-also"></a>Zie ook

[Vaste activa](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance.md)  
[Voorbereid zijn om zaken te doen](ui-get-ready-business.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
