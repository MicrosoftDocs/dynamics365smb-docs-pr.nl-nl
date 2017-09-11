---
title: Resourcegebruik en prijzen vastleggen en aanpassen| Microsoft Docs
description: Beschrijft hoe u het resourcegebruik of -verbruik kunt vastleggen dat is gekoppeld aan een project, om kosten, prijzen en werksoorten bij te houden en te beheren.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, capacity, staff
ms.date: 06/06/2017
ms.author: sgroespe
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 48692c9837007c6dd9c3891f0940b6f15b1d6541
ms.contentlocale: nl-nl
ms.lasthandoff: 07/07/2017


---
# <a name="how-to-use-resources-for-jobs"></a><span data-ttu-id="afe60-103">Procedure: Resources gebruiken voor projecten</span><span class="sxs-lookup"><span data-stu-id="afe60-103">How to: Use Resources for Jobs</span></span>
<span data-ttu-id="afe60-104">U legt het gebruik van resources vast in het projectdagboek om kosten, prijzen en de werksoorten bij te houden die zijn gekoppeld aan projecten.</span><span class="sxs-lookup"><span data-stu-id="afe60-104">You record the usage of resources in the job journal to keep track of costs, prices, and the work types that are linked to jobs.</span></span> <span data-ttu-id="afe60-105">Zie voor meer informatie [Procedure: Gebruik vastleggen voor projecten](projects-how-record-job-usage.md).</span><span class="sxs-lookup"><span data-stu-id="afe60-105">For more information, see [How to: Record Usage for Jobs](projects-how-record-job-usage.md).</span></span>

<span data-ttu-id="afe60-106">U kunt ook het verbruik van een resource boeken in een resourcedagboek.</span><span class="sxs-lookup"><span data-stu-id="afe60-106">You can also post the usage of a resource in a resource journal.</span></span> <span data-ttu-id="afe60-107">Posten die in een resourcedagboek zijn geboekt, werken niet door in het grootboek.</span><span class="sxs-lookup"><span data-stu-id="afe60-107">Entries posted in a resource journal have no effect on the general ledger.</span></span>

> [!NOTE]  
>   <span data-ttu-id="afe60-108">Deze functionaliteit vereist dat uw ervaring is ingesteld op **Pakket**.</span><span class="sxs-lookup"><span data-stu-id="afe60-108">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="afe60-109">Zie voor meer informatie [Uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-ervaring aanpassen](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="afe60-109">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-assign-resources-to-jobs"></a><span data-ttu-id="afe60-110">Resources toewijzen aan projecten</span><span class="sxs-lookup"><span data-stu-id="afe60-110">To assign resources to jobs</span></span>
<span data-ttu-id="afe60-111">U wijst resources aan projecten toe door projectplanningsregels voor het project te maken.</span><span class="sxs-lookup"><span data-stu-id="afe60-111">You assign resources to jobs by creating job planning lines for the job.</span></span> <span data-ttu-id="afe60-112">Zie [Procedure: Projecten maken](projects-how-create-jobs.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="afe60-112">For more information, see [How to: Create Jobs](projects-how-create-jobs.md).</span></span>

## <a name="to-record-resource-usage-for-a-job"></a><span data-ttu-id="afe60-113">Resourceverbruik voor een project vastleggen</span><span class="sxs-lookup"><span data-stu-id="afe60-113">To record resource usage for a job</span></span>
1. <span data-ttu-id="afe60-114">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Projectdagboeken** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="afe60-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Job Journals**, and then choose the related link.</span></span>
2. <span data-ttu-id="afe60-115">Open een relevante projectdagboekbatch en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="afe60-115">Open a relevant job journal batch, and then fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
3. <span data-ttu-id="afe60-116">Wanneer het dagboek compleet is, kiest u de actie **Boeken**.</span><span class="sxs-lookup"><span data-stu-id="afe60-116">When the journal is complete, choose the **Post** action.</span></span>

## <a name="to-adjust-resource-prices"></a><span data-ttu-id="afe60-117">Resourceprijzen aanpassen</span><span class="sxs-lookup"><span data-stu-id="afe60-117">To adjust resource prices</span></span>
<span data-ttu-id="afe60-118">Als u kost- of verkoopprijzen wilt wijzigen voor een groot aantal resources, kunt u een batchverwerking gebruiken.</span><span class="sxs-lookup"><span data-stu-id="afe60-118">If you want to change costs or prices for a large number of resources, you can use a batch job.</span></span>  

1. <span data-ttu-id="afe60-119">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Resourceprijzen herwaarderen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="afe60-119">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Adjust Resource Costs/Prices**, and then choose the related link.</span></span>
2. <span data-ttu-id="afe60-120">Vul de overige velden op een regel desgewenst in en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="afe60-120">Fill in the fields on a line as necessary, and then choose the **OK** button.</span></span>

> [!NOTE]  
>   <span data-ttu-id="afe60-121">Met deze batchverwerking worden geen alternatieve kosten of prijzen voor resources gemaakt of aangepast.</span><span class="sxs-lookup"><span data-stu-id="afe60-121">This batch job does not create or adjust alternate costs or prices for resources.</span></span> <span data-ttu-id="afe60-122">Dit verandert alleen de inhoud van het veld op de resourcekaart voor het veld **Aan te passen prijs** dat u hebt geselecteerd in de batchtaak.</span><span class="sxs-lookup"><span data-stu-id="afe60-122">It only changes the contents of the field on the resource card for the **Adjust Field** field that you selected in the batch job.</span></span> <span data-ttu-id="afe60-123">De aanpassing werkt onmiddellijk door voor de resources. Controleer daarom uw herwaarderingsfactoren zorgvuldig voordat u de batchverwerking uitvoert.</span><span class="sxs-lookup"><span data-stu-id="afe60-123">The adjustment will take effect immediately for resources, so check your adjustment factors before you run the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-existing-alternate-prices"></a><span data-ttu-id="afe60-124">Suggesties voor wijzigingen van resourceprijzen krijgen op basis van bestaande alternatieve prijzen</span><span class="sxs-lookup"><span data-stu-id="afe60-124">To get resource price change suggestions based on existing alternate prices</span></span>
<span data-ttu-id="afe60-125">Als u al alternatieve resourceprijzen hebt ingesteld voor bepaalde resources, kunt u een batchverwerking gebruiken om meerdere alternatieve resourceprijzen in te stellen.</span><span class="sxs-lookup"><span data-stu-id="afe60-125">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="afe60-126">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png ""pictogram Zoeken naar pagina of rapport"), voer **Resourceprijswijzigingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="afe60-126">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="afe60-127">Kies de actie **Res.prijsvoorstellen (Prijs)** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="afe60-127">Choose the **Suggest Res. Price Chg. (Price)** action, and then fill in the fields as necessary.</span></span>
3. <span data-ttu-id="afe60-128">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="afe60-128">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="afe60-129">Nadat de batchverwerking is voltooid, bevat het venster **Resourceprijswijzigingen** de resultaten van de batchverwerking.</span><span class="sxs-lookup"><span data-stu-id="afe60-129">When the batch job is finished, the **Resource Price Changes** window shows the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-standard-prices"></a><span data-ttu-id="afe60-130">Resourceprijsvoorstellen ophalen op basis van standaardverkoopprijzen</span><span class="sxs-lookup"><span data-stu-id="afe60-130">To get resource price change suggestions based on standard prices</span></span>
<span data-ttu-id="afe60-131">Als u meerdere alternatieve resourceprijzen wilt instellen op basis van de standaardverkoopprijzen op de resourcekaarten, kunt u een batchverwerking gebruiken.</span><span class="sxs-lookup"><span data-stu-id="afe60-131">If you want to set up multiple alternate resource prices based on the standard prices on the resource cards, you can use a batch job.</span></span>  

1. <span data-ttu-id="afe60-132">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png ""pictogram Zoeken naar pagina of rapport"), voer **Resourceprijswijzigingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="afe60-132">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Resource Price Changes**, and then choose the related link.</span></span>
2. <span data-ttu-id="afe60-133">Kies de actie **Res.prijsvoorstellen (Res.)** en vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="afe60-133">Choose the **Suggest Res. Price Chg. (Res.)** action, and then fill in the fields as necessary.</span></span>  
3. <span data-ttu-id="afe60-134">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="afe60-134">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="afe60-135">Nadat de batchverwerking is voltooid, opent u het venster **Resourceprijswijzigingen** om de resultaten van de batchverwerking te bekijken.</span><span class="sxs-lookup"><span data-stu-id="afe60-135">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="to-get-resource-price-change-suggestions-based-on-alternate-prices"></a><span data-ttu-id="afe60-136">Suggesties voor wijzigingen van resourceprijzen krijgen op basis van alternatieve prijzen</span><span class="sxs-lookup"><span data-stu-id="afe60-136">To get resource price change suggestions based on alternate prices</span></span>
<span data-ttu-id="afe60-137">Als u al alternatieve resourceprijzen hebt ingesteld voor bepaalde resources, kunt u een batchverwerking gebruiken om meerdere alternatieve resourceprijzen in te stellen.</span><span class="sxs-lookup"><span data-stu-id="afe60-137">If you have already set up alternate resource price for some resources, you can use a batch job to set up multiple alternate resource prices.</span></span>

1. <span data-ttu-id="afe60-138">Voer **Res.prijsvoorstellen (Prijs)** in het tekstvak **Zoeken** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="afe60-138">In the **Search** box, enter **Suggest Res. Price Chg. (Price)**, and then choose the related link.</span></span>  
2. <span data-ttu-id="afe60-139">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="afe60-139">Fill in the fields as necessary.</span></span>
3. <span data-ttu-id="afe60-140">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="afe60-140">Choose the **OK** button.</span></span>  
4. <span data-ttu-id="afe60-141">Nadat de batchverwerking is voltooid, opent u het venster **Resourceprijswijzigingen** om de resultaten van de batchverwerking te bekijken.</span><span class="sxs-lookup"><span data-stu-id="afe60-141">When the batch job is finished, open the **Resource Price Changes** window to see the results of the batch job.</span></span>

## <a name="see-also"></a><span data-ttu-id="afe60-142">Zie ook</span><span class="sxs-lookup"><span data-stu-id="afe60-142">See Also</span></span>
[<span data-ttu-id="afe60-143">Projectbeheer</span><span class="sxs-lookup"><span data-stu-id="afe60-143">Project Management</span></span>](projects-manage-projects.md)  
[<span data-ttu-id="afe60-144">Financiën</span><span class="sxs-lookup"><span data-stu-id="afe60-144">Finance</span></span>](finance.md)  
<span data-ttu-id="afe60-145">[Inkoop](purchasing-manage-purchasing.md)       </span><span class="sxs-lookup"><span data-stu-id="afe60-145">[Purchasing](purchasing-manage-purchasing.md)       </span></span>  
<span data-ttu-id="afe60-146">[Verkoop](sales-manage-sales.md)   </span><span class="sxs-lookup"><span data-stu-id="afe60-146">[Sales](sales-manage-sales.md)   </span></span>  
<span data-ttu-id="afe60-147">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="afe60-147">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  

