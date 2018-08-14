---
title: "Btw-categorieën instellen"
description: Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: c6f10f8252c00bf0a599f9fa794ee36c41ce92be
ms.openlocfilehash: 78a1c3f655e9a094b06075847c883dbd8f939e75
ms.contentlocale: nl-nl
ms.lasthandoff: 07/31/2018

---
# <a name="set-up-vat-categories"></a><span data-ttu-id="e3e25-103">VAT-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="e3e25-103">Set Up VAT Categories</span></span>
<span data-ttu-id="e3e25-104">Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.</span><span class="sxs-lookup"><span data-stu-id="e3e25-104">To use the electronic VAT declaration, you must set up a VAT category code for all XML elements in the electronic VAT declaration.</span></span>  

<span data-ttu-id="e3e25-105">U moet alle mogelijke categorie- en subcategoriecombinaties instellen die een XML-element in de elektronische btw-aangifte voorstellen.</span><span class="sxs-lookup"><span data-stu-id="e3e25-105">You must set up all of the possible category and subcategory combinations that represent an XML element in the electronic VAT declaration.</span></span> <span data-ttu-id="e3e25-106">Vervolgens kunt u de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="e3e25-106">Then, you can map the VAT statement data directly to an XML element.</span></span>  

## <a name="to-set-up-a-vat-category"></a><span data-ttu-id="e3e25-107">Een btw-categorie instellen</span><span class="sxs-lookup"><span data-stu-id="e3e25-107">To set up a VAT category</span></span>  

1.  <span data-ttu-id="e3e25-108">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangifte btw-categorieën** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e3e25-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax. Decl. VAT Categories**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e3e25-109">Kies in het venster **Elektronische aangifte btw-categorieën** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="e3e25-109">In the **Elec. Tax. Decl. VAT Categories** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="e3e25-110">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="e3e25-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e3e25-111">Veld</span><span class="sxs-lookup"><span data-stu-id="e3e25-111">Field</span></span>|<span data-ttu-id="e3e25-112">Description</span><span class="sxs-lookup"><span data-stu-id="e3e25-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e3e25-113">**Code**</span><span class="sxs-lookup"><span data-stu-id="e3e25-113">**Code**</span></span>|<span data-ttu-id="e3e25-114">De unieke code voor elke categorie- en subcategoriecombinatie.</span><span class="sxs-lookup"><span data-stu-id="e3e25-114">The unique code for each category and subcategory combination.</span></span> <span data-ttu-id="e3e25-115">U kunt maximaal 10 alfanumerieke tekens invoeren.</span><span class="sxs-lookup"><span data-stu-id="e3e25-115">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="e3e25-116">**Categorie**</span><span class="sxs-lookup"><span data-stu-id="e3e25-116">**Category**</span></span>|<span data-ttu-id="e3e25-117">Geef de hoofdcategorieoptie voor de btw-aangifte op.</span><span class="sxs-lookup"><span data-stu-id="e3e25-117">Specify the main category option for the VAT statement.</span></span>|  
    |<span data-ttu-id="e3e25-118">**Door ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="e3e25-118">**By Us (Domestic)**</span></span>|<span data-ttu-id="e3e25-119">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-119">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="e3e25-120">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="e3e25-120">Select a subcategory here if the **Category** field displays **By Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="e3e25-121">**Aan ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="e3e25-121">**To Us (Domestic)**</span></span>|<span data-ttu-id="e3e25-122">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-122">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="e3e25-123">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="e3e25-123">Select a subcategory here if the **Category** field displays **To Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="e3e25-124">**Door ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="e3e25-124">**By Us (Foreign)**</span></span>|<span data-ttu-id="e3e25-125">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-125">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="e3e25-126">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="e3e25-126">Select a subcategory here if the **Category** field displays **By Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="e3e25-127">**Aan ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="e3e25-127">**To Us (Foreign)**</span></span>|<span data-ttu-id="e3e25-128">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-128">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="e3e25-129">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="e3e25-129">Select a subcategory here if the **Category** field displays **To Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="e3e25-130">**Berekening**</span><span class="sxs-lookup"><span data-stu-id="e3e25-130">**Calculation**</span></span>|<span data-ttu-id="e3e25-131">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-131">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="e3e25-132">Selecteer hier een subcategorie als het veld **Categorie** **Berekening** bevat.</span><span class="sxs-lookup"><span data-stu-id="e3e25-132">Select a subcategory here if the **Category** field displays **Calculation**.</span></span>|  
    |<span data-ttu-id="e3e25-133">**Optioneel**</span><span class="sxs-lookup"><span data-stu-id="e3e25-133">**Optional**</span></span>|<span data-ttu-id="e3e25-134">Schakel dit in om aan te geven dat het XML-element dat aangeduid wordt met de categoriecode, niet verplicht is in de elektronische btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="e3e25-134">Select to indicate that the XML element that is represented by the category code is not required in the electronic VAT declaration.</span></span>|  

4.  <span data-ttu-id="e3e25-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="e3e25-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="e3e25-136">U kunt nu de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="e3e25-136">You can now map the VAT statement data directly to an XML element.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e3e25-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e3e25-137">See Also</span></span>  
 [<span data-ttu-id="e3e25-138">Elektronische btw- en ICP-aangiften verzenden</span><span class="sxs-lookup"><span data-stu-id="e3e25-138">Submitting Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md)  
 [<span data-ttu-id="e3e25-139">Elektronische btw- en ICP-aangiften instellen</span><span class="sxs-lookup"><span data-stu-id="e3e25-139">Setting Up Electronic VAT and ICP Declarations</span></span>](how-to-set-up-electronic-vat-and-icp-declarations.md)

