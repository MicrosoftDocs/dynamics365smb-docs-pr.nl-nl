---
title: Btw-categorieën instellen
description: Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: 330752e75b7e7e6215216b13f6bc4220f58451e2
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778357"
---
# <a name="set-up-vat-categories"></a>VAT-categorieën instellen
Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.  

U moet alle mogelijke categorie- en subcategoriecombinaties instellen die een XML-element in de elektronische btw-aangifte voorstellen. Vervolgens kunt u de btw-aangiftegegevens direct aan een XML-element toewijzen.  

## <a name="to-set-up-a-vat-category"></a>Een btw-categorie instellen  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Elektronische aangifte btw-categorieën** in en kies de gerelateerde koppeling.  
2.  Kies op de pagina **Elektronische aangifte btw-categorieën** de actie **Nieuw**.  
3.  Vul de velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|De unieke code voor elke categorie- en subcategoriecombinatie. U kunt maximaal 10 alfanumerieke tekens invoeren.|  
    |**Categorie**|Geef de hoofdcategorieoptie voor de btw-aangifte op.|  
    |**Door ons (Binnenland)**|De subcategorie voor de btw-aangifte.<br /><br /> Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Binnenland)** bevat.|  
    |**Aan ons (Binnenland)**|De subcategorie voor de btw-aangifte.<br /><br /> Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Binnenland)** bevat.|  
    |**Door ons (Buitenland)**|De subcategorie voor de btw-aangifte.<br /><br /> Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Buitenland)** bevat.|  
    |**Aan ons (Buitenland)**|De subcategorie voor de btw-aangifte.<br /><br /> Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Buitenland)** bevat.|  
    |**Berekening**|De subcategorie voor de btw-aangifte.<br /><br /> Selecteer hier een subcategorie als het veld **Categorie** **Berekening** bevat.|  
    |**Optioneel**|Schakel dit in om aan te geven dat het XML-element dat aangeduid wordt met de categoriecode, niet verplicht is in de elektronische btw-aangifte.|  

4.  Kies de knop **OK**.  

U kunt nu de btw-aangiftegegevens direct aan een XML-element toewijzen.  

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md)  
 [Elektronische btw- en ICP-aangiften instellen](how-to-set-up-electronic-vat-and-icp-declarations.md)
