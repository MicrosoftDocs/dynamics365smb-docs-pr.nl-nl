---
title: Een inkooporder maken om een aanbod op te vragen | Microsoft Docs
description: Beschrijft hoe u een verkoopaanbieding of een offerteaanvraagdocument maakt om uw aanbod aan een klant vast te leggen om producten onder bepaalde voorwaarden te verkopen.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: rfq
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 416c5a4e4376932c16a1496f2db2b0c79307d22b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772616"
---
# <a name="request-quotes"></a>Offertes aanvragen
U kunt een inkoopofferte als conceptversie van de inkooporder gebruiken. De order kan vervolgens in een inkoopfactuur of een order worden omgezet.


## <a name="to-create-a-purchase-quote"></a>Een inkoopofferte maken
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Inkoopoffertes** in en kies de gerelateerde koppeling.
2. Maak een nieuw document op dezelfde manier als u een inkooporder maakt. Zie voor meer informatie [Inkopen vastleggen](purchasing-how-record-purchases.md).

## <a name="to-convert-a-purchase-quote-to-a-purchase-order"></a>Een inkoopofferte omzetten in een inkooporder
Wanneer u de leveranciersofferte hebt geaccepteerd, kunt u deze omzetten naar een inkoopfactuur of order om de inkoop te verwerken.

1. Open eeen inkoopofferte die klaar is om te worden geconverteerd en kies de actie **Order maken**.

De inkoopofferte wordt verwijderd uit de database. Een inkoopfactuur of -order wordt gemaakt op basis van de informatie in de inkoopofferte waarin u de inkoop kunt verwerken. Op de inkoopfactuur of inkooporder vermeldt het veld **Offertenr.** het nummer van de inkoopofferte van waaruit het is gemaakt.

## <a name="see-also"></a>Zie ook
[Inkoop](purchasing-manage-purchasing.md)  
[Inkoop instellen](purchasing-setup-purchasing.md)  
[Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]