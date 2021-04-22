---
title: Btw-categorieën instellen
description: Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 9b1b6ffad7cbd7525491a8b433409300b610f56b
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771384"
---
# <a name="set-up-vat-categories"></a><span data-ttu-id="dffff-103">VAT-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="dffff-103">Set Up VAT Categories</span></span>
<span data-ttu-id="dffff-104">Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.</span><span class="sxs-lookup"><span data-stu-id="dffff-104">To use the electronic VAT declaration, you must set up a VAT category code for all XML elements in the electronic VAT declaration.</span></span>  

<span data-ttu-id="dffff-105">U moet alle mogelijke categorie- en subcategoriecombinaties instellen die een XML-element in de elektronische btw-aangifte voorstellen.</span><span class="sxs-lookup"><span data-stu-id="dffff-105">You must set up all of the possible category and subcategory combinations that represent an XML element in the electronic VAT declaration.</span></span> <span data-ttu-id="dffff-106">Vervolgens kunt u de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="dffff-106">Then, you can map the VAT statement data directly to an XML element.</span></span>  

## <a name="to-set-up-a-vat-category"></a><span data-ttu-id="dffff-107">Een btw-categorie instellen</span><span class="sxs-lookup"><span data-stu-id="dffff-107">To set up a VAT category</span></span>  

1.  <span data-ttu-id="dffff-108">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Elektronische aangifte btw-categorieën** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="dffff-108">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Elec. Tax. Decl. VAT Categories**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="dffff-109">Kies op de pagina **Elektronische aangifte btw-categorieën** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="dffff-109">On the **Elec. Tax. Decl. VAT Categories** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="dffff-110">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="dffff-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="dffff-111">Veld</span><span class="sxs-lookup"><span data-stu-id="dffff-111">Field</span></span>|<span data-ttu-id="dffff-112">Description</span><span class="sxs-lookup"><span data-stu-id="dffff-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="dffff-113">**Code**</span><span class="sxs-lookup"><span data-stu-id="dffff-113">**Code**</span></span>|<span data-ttu-id="dffff-114">De unieke code voor elke categorie- en subcategoriecombinatie.</span><span class="sxs-lookup"><span data-stu-id="dffff-114">The unique code for each category and subcategory combination.</span></span> <span data-ttu-id="dffff-115">U kunt maximaal 10 alfanumerieke tekens invoeren.</span><span class="sxs-lookup"><span data-stu-id="dffff-115">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="dffff-116">**Categorie**</span><span class="sxs-lookup"><span data-stu-id="dffff-116">**Category**</span></span>|<span data-ttu-id="dffff-117">Geef de hoofdcategorieoptie voor de btw-aangifte op.</span><span class="sxs-lookup"><span data-stu-id="dffff-117">Specify the main category option for the VAT statement.</span></span>|  
    |<span data-ttu-id="dffff-118">**Door ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="dffff-118">**By Us (Domestic)**</span></span>|<span data-ttu-id="dffff-119">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-119">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="dffff-120">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="dffff-120">Select a subcategory here if the **Category** field displays **By Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="dffff-121">**Aan ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="dffff-121">**To Us (Domestic)**</span></span>|<span data-ttu-id="dffff-122">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-122">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="dffff-123">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="dffff-123">Select a subcategory here if the **Category** field displays **To Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="dffff-124">**Door ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="dffff-124">**By Us (Foreign)**</span></span>|<span data-ttu-id="dffff-125">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-125">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="dffff-126">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="dffff-126">Select a subcategory here if the **Category** field displays **By Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="dffff-127">**Aan ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="dffff-127">**To Us (Foreign)**</span></span>|<span data-ttu-id="dffff-128">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-128">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="dffff-129">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="dffff-129">Select a subcategory here if the **Category** field displays **To Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="dffff-130">**Berekening**</span><span class="sxs-lookup"><span data-stu-id="dffff-130">**Calculation**</span></span>|<span data-ttu-id="dffff-131">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-131">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="dffff-132">Selecteer hier een subcategorie als het veld **Categorie** **Berekening** bevat.</span><span class="sxs-lookup"><span data-stu-id="dffff-132">Select a subcategory here if the **Category** field displays **Calculation**.</span></span>|  
    |<span data-ttu-id="dffff-133">**Optioneel**</span><span class="sxs-lookup"><span data-stu-id="dffff-133">**Optional**</span></span>|<span data-ttu-id="dffff-134">Schakel dit in om aan te geven dat het XML-element dat aangeduid wordt met de categoriecode, niet verplicht is in de elektronische btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="dffff-134">Select to indicate that the XML element that is represented by the category code is not required in the electronic VAT declaration.</span></span>|  

4.  <span data-ttu-id="dffff-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="dffff-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="dffff-136">U kunt nu de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="dffff-136">You can now map the VAT statement data directly to an XML element.</span></span>  

## <a name="see-also"></a><span data-ttu-id="dffff-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="dffff-137">See Also</span></span>  
 [<span data-ttu-id="dffff-138">Elektronische btw- en ICP-aangiften verzenden</span><span class="sxs-lookup"><span data-stu-id="dffff-138">Submitting Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md)  
 [<span data-ttu-id="dffff-139">Elektronische btw- en ICP-aangiften instellen</span><span class="sxs-lookup"><span data-stu-id="dffff-139">Setting Up Electronic VAT and ICP Declarations</span></span>](how-to-set-up-electronic-vat-and-icp-declarations.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]