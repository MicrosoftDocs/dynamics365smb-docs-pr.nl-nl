---
title: Outputboeking tegenboeken | Microsoft Docs
description: Het kan voorkomen dat een outputboeking moet worden tegengeboekt. Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 09/06/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 7ac453ff87d78e6be0567ba93b58c0f8938f4052
ms.contentlocale: nl-nl
ms.lasthandoff: 09/22/2017

---
# <a name="how-to-reverse-output-posting"></a>Procedure: een outputboeking tegenboeken
Het kan voorkomen dat een outputboeking moet worden tegengeboekt. Dit is bijvoorbeeld het geval als er een gegevensinvoerfout is gemaakt en er een onjuiste hoeveelheid output is geboekt op een productieorder.  

## <a name="to-reverse-an-output-posting"></a>Een outputboeking tegenboeken  
1.  Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Outputdagboek** in en klik vervolgens op de gerelateerde koppeling. Selecteer uw batch.  
2. Vul de velden in. Zie voor meer informatie [Procedure: Output en bewerkingstijd in batches boeken](production-how-to-post-output-quantity.md).
3.  Selecteer in het veld **Vereffenen met post** de bijbehorende artikelpost. Hiermee voert u een tegenboeking uit van de capaciteit en artikelposten.  
4. Boek de tegenboeking door het dagboek te boeken.  

De posten van het outputdagboek worden als positieve herwaardering geboekt op de artikelposten.  

## <a name="see-also"></a>Zie ook  
 [Productie](production-manage-manufacturing.md)    
 [Productie instellen](production-configure-production-processes.md)  
 [Gepland](production-planning.md)      
 [Voorraad](inventory-manage-inventory.md)  
 [Inkoop](purchasing-manage-purchasing.md)  
 [Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)  
