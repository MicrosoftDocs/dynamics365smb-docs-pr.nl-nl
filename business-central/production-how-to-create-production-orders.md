---
title: Productieorderkoppen maken | Microsoft Docs
description: U kunt een productieorder handmatig maken. De eerste stap is het maken van een productieorderkop.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 90d04a6f951c3312f88f536bfab680bcd071de63
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781935"
---
# <a name="create-production-order-headers"></a>Productieorderkoppen maken
U kunt een productieorder handmatig maken. De eerste stap is het maken van een productieorderkop.

Productieorders worden meestal automatisch op basis van een planningsfunctie gemaakt om te voldoen aan een bekende vraag. Zie [Planning](production-planning.md) voor meer informatie.   

In de volgende procedure wordt een vast geplande productieorder gemaakt. U kunt ook productieorders maken met een andere status.  

## <a name="to-create-a-production-order-header"></a>Productieorderkoppen maken  
1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Vast geplande productieorders** in en kies de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Selecteer in het veld **Nr.** het volgende nummer uit de reeks in.  
4.  Selecteer in het veld **Bronsoort** de bron van de productieorder.

    Hier kunt u opgeven of er voor een familie van artikelen moet worden geproduceerd. Zie [Werken met productfamilies](production-how-work-family.md) voor meer informatie.
5.  Selecteer in het veld **Bronnr.** het artikelnummer, de productfamilie of de verkoopkop waarvoor de productieorder moet worden gegenereerd.  
6.  Vul de velden **Aantal** en **Vervaldatum** in op basis van de specificaties.  

Wanneer productievereisten veranderen, bijvoorbeeld onderdelen of bewerkingen, kunt u de productieorder snel herplannen. Zie [Productieorders direct opnieuw plannen of vernieuwen](production-how-to-replan-refresh-production-orders.md) voor meer informatie. 

## <a name="see-also"></a>Zie ook  
[Productie](production-manage-manufacturing.md)    
[Productie instellen](production-configure-production-processes.md)  
[Gepland](production-planning.md)      
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]