---
title: Elektronische btw- en ICP-aangiften maken
description: Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 34520c70c0871c9bd1624b3f331834d5b3094f71
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="create-electronic-vat-and-icp-declarations"></a>Elektronische btw- en ICP-aangiften maken
Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.  

> [!NOTE]  
>  Als u het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen** hebt geselecteerd, kunt u een elektronische aangifte voor slechts één bedrijf maken. Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen. Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst. U kunt geen belastinggegevens van ICP-aangiften combineren. ICP-aangiften moeten altijd afzonderlijk worden ingediend.  

Als er geen intracommunautaire leveringen zijn geweest in de aangifteperiode, dan wordt er een elektronische ICP-aangifte aangemaakt zonder XML-elementen voor de leveringen. Als u een dergelijke aangifte verzendt, wordt een foutbericht weergegeven.  

## <a name="to-create-an-electronic-vat-or-icp-declaration"></a>Een elektronische btw- of ICP-aangifte maken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.  
2.  Kies in het venster **Overzicht elektronische aangiften** de actie **Nieuw**.  
3.  Vul in het venster **Elektronische aangiftekaart** op het sneltabblad **Algemeen** de vereiste velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |-----------------------------------|---------------------------------------|  
    |**Sjabloonnaam**|De naam van de sjabloon die wordt gebruikt om de elektronische aangifte te maken.|  
    |**Aangifte**|De naam van het afschrift dat wordt gebruikt om de elektronische aangifte te maken.|  

6.  Kies de knop **OK**.  

De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** in het venster **Elektronische aangiftekaart**.  

## <a name="see-also"></a>Zie ook  
 [Elektronische belastingaangiften](electronic-tax-declarations.md)   
 [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md)   
 [Btw-categorieën instellen](how-to-set-up-vat-categories.md)

