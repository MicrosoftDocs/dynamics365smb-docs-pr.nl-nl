---
title: De boeken sluiten
description: 'Meer informatie over het sluiten van de boeken voor een boekjaar of -periode, en wat er gebeurt nadat u het jaareinde hebt afgesloten.'
author: jswymer
ms.topic: overview
ms.devlang: al
ms.search.keywords: 'year closing, close accounting period, close fiscal year, bank account detailed trial balance'
m.search.form: 100
ms.date: 08/05/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="closing-the-books"></a>De boeken sluiten
Nadat gezorgd hebt dat alle rekeningen actueel zijn, en u kosten en inkomsten hebt verdeeld, kunt u de boeken van een boekhoudperiode of boekjaar sluiten.

U bent niet verplicht om Sluiten een jaar lang te gebruiken, maar het maakt het werken in het systeem wel makkelijker voor u, omdat u gebruik kunt maken van de handige filteropties die worden geboden. Bovendien hoeft u zich geen zorgen te maken over het verlies van transactiedetails wanneer u het jaar afsluit omdat alle details behouden blijven, zelfs nadat u het jaar hebt afgesloten.

## <a name="closing-book-process"></a>Sluitingsproces van het boek
Bij het proces voor het afsluiten van boeken zijn drie hoofdtaken betrokken:

1. De boekingsperiode afsluiten.

    Een boekjaar wordt gedefinieerd als een of meer open perioden zoals die zijn gedefinieerd op de pagina **Boekingsperioden**. Een boekjaar bestaat over het algemeen uit 12 perioden van een maand, maar u kunt een jaar ook anders definiëren.

    Zie [Boekingsperioden afsluiten](year-close-account-periods.md) voor meer informatie.
2. Naboekingen registreren.

    Wanneer u een boekjaar sluit, moet u een aantal administratieve transacties invoeren (zoals vooraf betaalde en te betalen artikelen). De transacties worden herwaarderingsposten genoemd. Er zijn geen speciale regels voor het boeken van deze posten en ze bevatten .Net als andere posten) een vinkje in het veld  **Post van vorig jaar**  als ze zijn geboekt op een datum in een afgesloten boekjaar. Zelfs als een boekjaar is afgesloten, kunt u er nog steeds grootboekposten voor boeken.
3. Saldi van de WenV-rekeningen overboeken naar de balans.

    Nadat een boekjaar is gesloten en alle naboekingen zijn geboekt, moeten de resultatenrekeningen worden gesloten en het netto inkomen van het jaar moet worden overgedragen naar een rekening onder de vermogensrekening van de eigenaren op de balans. Gebruik hiervoor de batchverwerking Afsluiten WenV-rekening. De batchverwerking verwerkt alle grootboekrekeningen van het soort Resultaten en maakt tegenboekingen voor de bijbehorende saldo's. Deze posten worden geplaatst in een dagboek van waar ze kunnen worden geboekt. De batchtaak boekt ze niet automatisch, behalve wanneer er een extra rapportagevaluta wordt gebruikt. Wanneer een extra rapportagevaluta wordt gebruikt, boekt de batchverwerking direct naar het grootboek.

    Zie [Afsluiten WenV-rekening](year-close-income-statement.md) voor meer informatie.
4. Het boeken van de jaareinde-ultimopost samen met de uitstellende vermogensrekeningposten.

    Wanneer de batchverwerking Afsluiten WenV-rekening is voltooid, boekt u de posten die zijn gegenereerd door de batchverwerking. Als u geen rekening voor winstreservering hebt opgegeven in de batchtaak, voert u één regel in met een vereffeningspost waarmee u de nettowinst boekt op de juiste rekening grootboek onder het eigen vermogen op de balans. Boek ten slotte het dagboek.

    Zie [Jaareinde-ultimopost boeken](year-how-post-year-end-close-entry.md) voor meer informatie.

## <a name="what-happens-when-you-close"></a>Wat er gebeurt wanneer u afsluit

Wanneer u het boekjaar aan het einde van het jaar afsluit, verplaatst het systeem uw resultaten van de berekende resultaten. Het systeem markeert tevens het boekjaar als "afgesloten," en markeert alle volgende posten voor het afgesloten jaar als "posten van het vorige jaar."

Het systeem genereert vervolgens een afsluitende boeking, maar boekt de boeking niet automatisch. U krijgt de mogelijkheid om de compenserende eigenvermogensrekeningpost(en) te maken, zodat u kunt bepalen hoe u uw afsluitende post wilt toewijzen. Als een bedrijf bijvoorbeeld verschillende divisies heeft, kunt u in het systeem één ultimopost laten genereren voor alle divisies en kunt u vervolgens een uitstellende post voor de vermogensrekening van elke divisie maken.

U kunt in een eerder boekjaar boeken, zelfs nadat de resultatenrekeningen zijn gesloten, als u nadien nogmaals de batchverwerking Afsluiten WenV-rekening uitvoert.

## <a name="see-also"></a>Zie ook

[Werken met boekhoudperioden en boekjaren](finance-accounting-periods-and-fiscal-years.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    


[!INCLUDE[footer-include](includes/footer-banner.md)]
