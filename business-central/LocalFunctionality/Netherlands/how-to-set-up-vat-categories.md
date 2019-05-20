---
title: Btw-categorieën instellen
description: Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: f7e6639a052f018f46996fb418774978435da997
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/29/2019
ms.locfileid: "1246011"
---
# <a name="set-up-vat-categories"></a><span data-ttu-id="8d22d-103">VAT-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="8d22d-103">Set Up VAT Categories</span></span>
<span data-ttu-id="8d22d-104">Als u de elektronische btw-aangifte wilt gebruiken, moet u een btw-categoriecode voor alle XML-elementen in de elektronische btw-aangifte instellen.</span><span class="sxs-lookup"><span data-stu-id="8d22d-104">To use the electronic VAT declaration, you must set up a VAT category code for all XML elements in the electronic VAT declaration.</span></span>  

<span data-ttu-id="8d22d-105">U moet alle mogelijke categorie- en subcategoriecombinaties instellen die een XML-element in de elektronische btw-aangifte voorstellen.</span><span class="sxs-lookup"><span data-stu-id="8d22d-105">You must set up all of the possible category and subcategory combinations that represent an XML element in the electronic VAT declaration.</span></span> <span data-ttu-id="8d22d-106">Vervolgens kunt u de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="8d22d-106">Then, you can map the VAT statement data directly to an XML element.</span></span>  

## <a name="to-set-up-a-vat-category"></a><span data-ttu-id="8d22d-107">Een btw-categorie instellen</span><span class="sxs-lookup"><span data-stu-id="8d22d-107">To set up a VAT category</span></span>  

1.  <span data-ttu-id="8d22d-108">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangifte btw-categorieën** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8d22d-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax. Decl. VAT Categories**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8d22d-109">Kies op de pagina **Elektronische aangifte btw-categorieën** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="8d22d-109">On the **Elec. Tax. Decl. VAT Categories** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="8d22d-110">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="8d22d-110">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="8d22d-111">Veld</span><span class="sxs-lookup"><span data-stu-id="8d22d-111">Field</span></span>|<span data-ttu-id="8d22d-112">Description</span><span class="sxs-lookup"><span data-stu-id="8d22d-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="8d22d-113">**Code**</span><span class="sxs-lookup"><span data-stu-id="8d22d-113">**Code**</span></span>|<span data-ttu-id="8d22d-114">De unieke code voor elke categorie- en subcategoriecombinatie.</span><span class="sxs-lookup"><span data-stu-id="8d22d-114">The unique code for each category and subcategory combination.</span></span> <span data-ttu-id="8d22d-115">U kunt maximaal 10 alfanumerieke tekens invoeren.</span><span class="sxs-lookup"><span data-stu-id="8d22d-115">You can enter a maximum of 10 alphanumeric characters.</span></span>|  
    |<span data-ttu-id="8d22d-116">**Categorie**</span><span class="sxs-lookup"><span data-stu-id="8d22d-116">**Category**</span></span>|<span data-ttu-id="8d22d-117">Geef de hoofdcategorieoptie voor de btw-aangifte op.</span><span class="sxs-lookup"><span data-stu-id="8d22d-117">Specify the main category option for the VAT statement.</span></span>|  
    |<span data-ttu-id="8d22d-118">**Door ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="8d22d-118">**By Us (Domestic)**</span></span>|<span data-ttu-id="8d22d-119">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-119">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="8d22d-120">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="8d22d-120">Select a subcategory here if the **Category** field displays **By Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="8d22d-121">**Aan ons (Binnenland)**</span><span class="sxs-lookup"><span data-stu-id="8d22d-121">**To Us (Domestic)**</span></span>|<span data-ttu-id="8d22d-122">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-122">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="8d22d-123">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Binnenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="8d22d-123">Select a subcategory here if the **Category** field displays **To Us (Domestic)**.</span></span>|  
    |<span data-ttu-id="8d22d-124">**Door ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="8d22d-124">**By Us (Foreign)**</span></span>|<span data-ttu-id="8d22d-125">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-125">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="8d22d-126">Selecteer hier een subcategorie als het veld **Categorie** **Door ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="8d22d-126">Select a subcategory here if the **Category** field displays **By Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="8d22d-127">**Aan ons (Buitenland)**</span><span class="sxs-lookup"><span data-stu-id="8d22d-127">**To Us (Foreign)**</span></span>|<span data-ttu-id="8d22d-128">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-128">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="8d22d-129">Selecteer hier een subcategorie als het veld **Categorie** **Aan ons (Buitenland)** bevat.</span><span class="sxs-lookup"><span data-stu-id="8d22d-129">Select a subcategory here if the **Category** field displays **To Us (Foreign)**.</span></span>|  
    |<span data-ttu-id="8d22d-130">**Berekening**</span><span class="sxs-lookup"><span data-stu-id="8d22d-130">**Calculation**</span></span>|<span data-ttu-id="8d22d-131">De subcategorie voor de btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-131">The subcategory for the VAT Statement.</span></span><br /><br /> <span data-ttu-id="8d22d-132">Selecteer hier een subcategorie als het veld **Categorie** **Berekening** bevat.</span><span class="sxs-lookup"><span data-stu-id="8d22d-132">Select a subcategory here if the **Category** field displays **Calculation**.</span></span>|  
    |<span data-ttu-id="8d22d-133">**Optioneel**</span><span class="sxs-lookup"><span data-stu-id="8d22d-133">**Optional**</span></span>|<span data-ttu-id="8d22d-134">Schakel dit in om aan te geven dat het XML-element dat aangeduid wordt met de categoriecode, niet verplicht is in de elektronische btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="8d22d-134">Select to indicate that the XML element that is represented by the category code is not required in the electronic VAT declaration.</span></span>|  

4.  <span data-ttu-id="8d22d-135">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="8d22d-135">Choose the **OK** button.</span></span>  

<span data-ttu-id="8d22d-136">U kunt nu de btw-aangiftegegevens direct aan een XML-element toewijzen.</span><span class="sxs-lookup"><span data-stu-id="8d22d-136">You can now map the VAT statement data directly to an XML element.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8d22d-137">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8d22d-137">See Also</span></span>  
 [<span data-ttu-id="8d22d-138">Elektronische btw- en ICP-aangiften verzenden</span><span class="sxs-lookup"><span data-stu-id="8d22d-138">Submitting Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md)  
 [<span data-ttu-id="8d22d-139">Elektronische btw- en ICP-aangiften instellen</span><span class="sxs-lookup"><span data-stu-id="8d22d-139">Setting Up Electronic VAT and ICP Declarations</span></span>](how-to-set-up-electronic-vat-and-icp-declarations.md)
