---
title: Nieuwe waardeposten maken voor artikelen in de inventaris | Microsoft Docs
description: 'Beschrijft hoe u de waardeposten vermeerdert of vermindert van een of meer artikelen in voorraad door de huidige, berekende waarde ervan te boeken.'
documentationcenter: ''
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'costing, inventory cost, value entries'
ms.search.forms: '5803,'
ms.date: 07/29/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="revalue-inventory"></a>Herwaardeer de voorraad
Gebruik het herwaarderingsdagboek als u de voorraadwaarde van een artikel of een bepaalde artikelpost wilt vermeerderen of verminderen.

## <a name="to-revalue-inventory"></a>Voorraad herwaarderen
1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Herwaarderingsdagboek** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Voorraadwaarde berekenen**.
3. Vul op de pagina **Voorraadwaarde berekenen** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. Kies de knop **Ok**.
5. Voer op elke regel op de pagina  **Artikelherwaarderingsdagboeken**  in het veld  **Eenheidskosten (herwaardering)**  de nieuwe eenheidskosten in. U kunt ook het nieuwe totale bedrag in het veld **Voorraadwaarde (Geherwaardeerd)** invoeren.

    De bijbehorende velden worden automatisch bijgewerkt. Het veld  **bedrag** toont de werkelijke wijziging in de voorraadwaarde voor de geselecteerde artikelpost. Het verschil tussen de waarden in de velden **Voorraadwaarde (Berekend)** en **Voorraadwaarde (Geherwaardeerd)** wordt berekend.
6. Wanneer u alle regels in het herwaarderingsdagboek hebt ingevuld, kiest u de actie **Boeken**.

Nieuwe waardeposten worden nu gemaakt om de herwaarderingen weer te geven die u hebt geboekt. U kunt de nieuwe waarden op de desbetreffende artikelkaarten bekijken.

## <a name="see-also"></a>Zie ook
[Ontwerpdetails: herwaardering](design-details-revaluation.md)    
[Voorraad](inventory-manage-inventory.md)    
[Verkoop](sales-manage-sales.md)    
[Inkoop](purchasing-manage-purchasing.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
