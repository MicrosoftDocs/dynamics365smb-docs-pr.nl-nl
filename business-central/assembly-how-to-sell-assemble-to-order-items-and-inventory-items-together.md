---
title: Op-order-assembleren-artikelen en voorraadartikelen samen verkopen | Microsoft Docs
description: Als een assemblageartikel is ingesteld op assembleren op voorraad, neemt het standaardproces voor de verkooporder aan dat het item al is samengesteld en uit de voorraad kan worden gepickt, als deze beschikbaar is. Maar als een deel (of allemaal) van de hoeveelheid niet beschikbaar is, hebt u de flexibiliteit om ter plekke een assemblageorder voor het resterende aantal te maken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 123d4613d042d9c3f7f863e7cd98b45c84a368ad
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5772926"
---
# <a name="sell-assemble-to-order-items-and-inventory-items-together"></a>Op-order-assembleren-artikelen en voorraadartikelen samen verkopen
Als het veld **Assemblagebeleid** op de artikelkaart van assemblageartikel **Op voorraad assembleren** bevat, neemt het standaardproces voor de verkooporder aan dat het item al is samengesteld en uit de voorraad kan worden gepickt, als deze beschikbaar is. Daarom wordt er geen assemblageorder automatisch gemaakt en gekoppeld aan de verkooporderregel. Als echter een deel van (of de gehele) hoeveelheid niet beschikbaar is, kunt u een assemblageorder maken voor het resterende aantal door het veld **Aantal voor op order assembleren** op de verkooporderregel in te vullen. Op deze manier kunt u het artikel dat u wilt bestellen, samenstellen, ook al is het standaard ingesteld om op voorraad te worden geassembleerd.  

Soortgelijke flexibiliteit bestaat wanneer u artikelen verkoopt die samengesteld moeten worden voor de order, en een gedeelte van het aantal is in voorraad, zodat u deze hoeveelheid wilt aftrekken van de assemblageorder. Zie voor meer informatie [Voorraadartikelen verkopen in assembleren-op-order-stromen](assembly-how-to-sell-inventory-items-in-assemble-to-order-flows.md).  

> [!NOTE]  
>  Bepaalde regels zijn van toepassing op het veld **Te verzenden aantal** op verkooporderregels die een combinatie van het op-order-assembleren-aantallen en voorraadaantallen bevatten. Zie voor meer informatie de sectie Combinatiescenario's in [Op voorraad assembleren of Op order assembleren begrijpen](assembly-assemble-to-order-or-assemble-to-stock.md).  

> [!NOTE]  
>  De volgende procedure bevat niet de standaard verkooporderstappen die u moet volgen voordat u een assemblageorder kunt maken voor hoeveelheden die niet beschikbaar zijn.

## <a name="to-sell-assemble-to-order-items-and-inventory-items-together"></a>Op-order-assembleren-artikelen en voorraadartikelen samen verkopen  
1.  Op de verkooporderregel voor een artikel dat in voorraad moet worden geassembleerd voert u in het veld **Hoeveelheid** een hoeveelheid in dat groter is dan de voorraad. De pagina **Beschikbaarheid controleren** verschijnt. Zie voor meer informatie [Beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md).
2.  Let op het veld **Totaal aantal** (een negatieve waarde), die u in de volgende stap invoert.  
3.  Voer de waarde uit de vorige stap in het veld **Aantal voor op order assembleren** .  
4.  Wijzigingen in de assemblagecomponenten uitvoeren. Zie voor meer informatie [Op order geassembleerde artikelen verkopen](assembly-how-to-sell-items-assembled-to-order.md).  
5.  Geef de verkooporder vrij voor het picken van de voorraadartikelen en assemblage van de niet beschikbare artikelen. Zie voor meer informatie over deze standaardassemblagestappen [Artikelen samenstellen](assembly-how-to-assemble-items.md).  

> [!CAUTION]  
>  Het veld **Opslaglocatie** in de verkooporder kan al vooraf zijn ingevuld volgens het veld **Opslaglocatiecode assembleren-op-order verzending** of **Opslagloc.code Vanuit-assembl.** op de locatiekaart. In dat geval is het veld **Opslaglocatie** op de verkooporderregel mogelijk onjuist in deze combinatie van hoeveelheden assembleren voor order en assembleren voor voorraad. Het is verstandig om het veld **Opslaglocatie** te onderzoeken en te controleren of de plaatsing voor alle hoeveelheden werkt. U kunt ook twee verschillende hoeveelheden invoeren op aparte verkooporderregels.  

## <a name="see-also"></a>Zie ook  
[Assemblagebeheer](assembly-assemble-items.md)  
[Werken met stuklijsten](inventory-how-work-BOMs.md)  
[Voorraad](inventory-manage-inventory.md)  
[Ontwerpdetails: Magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]