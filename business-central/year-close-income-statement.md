---
title: Sluiten winst- en verliesrekeningen
description: Bij jaarafsluiting moet u de batchverwerking Afsluiten WenV-rekening uitvoeren om de boekhoudperioden te sluiten die het boekjaar vormen.
author: jswymer
ms.topic: conceptual
ms.search.keywords: 'year closing, close accounting period, close fiscal year, bank account detailed trial balance'
ms.date: 08/05/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="close-income-statement-accounts"></a>Sluiten winst- en verliesrekeningen

Wanneer een boekjaar is afgelopen, moet u de hierin opgenomen perioden afsluiten. Voer hiervoor de batchverwerking **Afsluiten WenV-rekening** uit. Met deze taak wordt het jaarresultaat overgeboekt naar een rekening op de balans en worden de resultatenrekeningen afgesloten. In een dagboek worden regels gemaakt die u vervolgens kunt boeken.

## <a name="to-run-the-close-income-statement-batch-job"></a>De batchverwerking Afsluiten WenV-rekening uitvoeren

1. Sluit het boekjaar. Het boekjaar moet zijn afgesloten voordat u de batchverwerking kunt uitvoeren. Zie [Boekingsperioden afsluiten](year-close-account-periods.md) voor meer informatie.
2. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Resultatenrekening sluiten** in en kies vervolgens de gerelateerde koppeling.
3. Kies **OK** om de batchverwerking te starten.

## <a name="about-the-close-income-statement-batch-job"></a>Informatie over de batchverwerking Resultatenrekening afsluiten

De batchverwerking verwerkt alle grootboekrekeningen van het soort Resultaten en maakt tegenboekingen voor de bijbehorende saldo's. Dat wil zeggen, dat elke post de som is van alle grootboekposten op de rekening van het boekjaar. Deze nieuwe posten worden geplaatst in een dagboek waarin u een tegenrekening en resultatenrekening in de balans moet opgeven voordat u boekt. Wanneer u het dagboek boekt, wordt een post geboekt in elke resultatenrekening zodat het saldo nul wordt en het jaarresultaat tegelijkertijd wordt overgebracht naar de balans.

U moet het dagboek zelf boeken. De batchtaak boekt de boekingen niet automatisch, behalve wanneer er een extra rapportagevaluta wordt gebruikt. Wanneer een extra rapportagevaluta wordt gebruikt, boekt de batchverwerking posten direct naar het grootboek.

De datum op de regels die tijdens de batchverwerking in het dagboek worden opgenomen, is altijd een ultimodatum voor het boekjaar. De ultimodatum is een fictieve datum tussen de laatste dag van het oude boekjaar en de eerste dag van het nieuwe jaar. Het voordeel van boeken op een ultimodatum is dat u de juiste saldo's behoudt voor de gewone datums van het boekjaar.

U kunt de batchverwerking **Afsluiten WenV-rekening** meerdere keren gebruiken. Als u de batchverwerking opnieuw uitvoert, kunt ook naar vorige boekjaren boeken, zelfs nadat de WenV-rekeningen zijn afgesloten.

## <a name="see-also"></a>Zie ook

[Boeken sluiten](year-close-books.md)    
[Plaats de jaarafsluiting](year-how-post-year-end-close-entry.md)    
[Werken met boekhoudperioden en boekjaren](finance-accounting-periods-and-fiscal-years.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
