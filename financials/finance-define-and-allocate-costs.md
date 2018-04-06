---
title: "Kosten definiëren en toewijzen | Microsoft Docs"
description: "Tijdens kostenverdelingen worden kosten en opbrengsten verplaatst tussen kostensoorten , kostenplaatsen en kostenobjecten. U kunt zo veel verdelingen definiëren als u nodig hebt."
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
ms.sourcegitcommit: bec0619be0a65e3625759e13d2866ac615d7513c
ms.openlocfilehash: 04e5a95b7a926528cc26c254390d08e3bce6ad8a
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="defining-and-allocating-costs"></a><span data-ttu-id="c5789-104">Kosten definiëren en toewijzen</span><span class="sxs-lookup"><span data-stu-id="c5789-104">Defining and Allocating Costs</span></span>
<span data-ttu-id="c5789-105">Tijdens kostenverdelingen worden kosten en opbrengsten verplaatst tussen kostensoorten , kostenplaatsen en kostenobjecten.</span><span class="sxs-lookup"><span data-stu-id="c5789-105">Cost allocations move costs and revenues between cost types, cost centers, and cost objects.</span></span> <span data-ttu-id="c5789-106">U kunt zo veel verdelingen definiëren als u nodig hebt.</span><span class="sxs-lookup"><span data-stu-id="c5789-106">You can define as many allocations as you need.</span></span> <span data-ttu-id="c5789-107">Elke verdeling bestaat uit:</span><span class="sxs-lookup"><span data-stu-id="c5789-107">Each allocation consists of:</span></span>  

-   <span data-ttu-id="c5789-108">Een toewijzingsbron.</span><span class="sxs-lookup"><span data-stu-id="c5789-108">An allocation source.</span></span>  
-   <span data-ttu-id="c5789-109">Een of meer verdeeldoelen.</span><span class="sxs-lookup"><span data-stu-id="c5789-109">One or more allocation targets.</span></span>  

<span data-ttu-id="c5789-110">De verdelingsbron bepaalt welke kosten moeten worden verdeeld en de verdeeldoelen bepalen waaraan de kosten moeten worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="c5789-110">The allocation source establishes which costs must be allocated, and the allocation targets determine where the costs must be allocated.</span></span> <span data-ttu-id="c5789-111">Een verdelingsbron kan bijvoorbeeld zijn de kosten voor de kostensoort elektriciteit en verwarming.</span><span class="sxs-lookup"><span data-stu-id="c5789-111">For example, an allocation source can be the costs for the Electricity and Heating cost type.</span></span> <span data-ttu-id="c5789-112">U kunt alle verwarmings- en elektriciteitskosten aan drie kostenplaatsen toewijzen: Werkplaats, Productie en Verkoop.</span><span class="sxs-lookup"><span data-stu-id="c5789-112">You allocate all electricity and heating costs to three cost centers: Workshop, Production, and Sales.</span></span> <span data-ttu-id="c5789-113">Deze kostenplaatsen zijn uw verdeeldoelen.</span><span class="sxs-lookup"><span data-stu-id="c5789-113">These cost centers are your allocation targets.</span></span>  

<span data-ttu-id="c5789-114">Voor elke verdelingsbron definieert u een verdelingsniveau, een geldigheidsperiode en een variant als groeperings-id.</span><span class="sxs-lookup"><span data-stu-id="c5789-114">For each allocation source, you define an allocation level, a validity period, and a variant as grouping identifier.</span></span> <span data-ttu-id="c5789-115">U kunt met behulp van een batchtaak filters instellen om verdelingsdefinities te selecteren en vervolgens wordt de kostenverdeling automatisch uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="c5789-115">You can use a batch job to set filters to select allocation definitions and then run cost allocations automatically.</span></span>  

<span data-ttu-id="c5789-116">Voor elk verdeeldoel moet u een verdelingbasis definiëren.</span><span class="sxs-lookup"><span data-stu-id="c5789-116">For each allocation target, you define an allocation base.</span></span> <span data-ttu-id="c5789-117">De verdelingbasis kan statisch of dynamisch zijn.</span><span class="sxs-lookup"><span data-stu-id="c5789-117">The allocation base can be either static or dynamic.</span></span>  

-   <span data-ttu-id="c5789-118">Statische toewijzingen zijn gebaseerd op een vaste waarde voor bijvoorbeeld oppervlak of een vastgestelde verdeelsleutel, zoals 5:2:4.</span><span class="sxs-lookup"><span data-stu-id="c5789-118">Static allocation bases are based on a definite value, such as square footage or an established allocation ratio, such as 5:2:4.</span></span>  
-   <span data-ttu-id="c5789-119">Dynamische toewijzingen zijn afhankelijk van wijzigbare waarden, bijvoorbeeld het aantal werknemers in een kostenplaats of de omzet van een kostenobject gedurende een bepaalde periode.</span><span class="sxs-lookup"><span data-stu-id="c5789-119">Dynamic allocation bases depend on changeable values, such as the number of employees in a cost center or sales revenue of a cost object throughout a certain time period.</span></span>  

<span data-ttu-id="c5789-120">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="c5789-120">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>

|<span data-ttu-id="c5789-121">Aan</span><span class="sxs-lookup"><span data-stu-id="c5789-121">To</span></span>|<span data-ttu-id="c5789-122">Zie</span><span class="sxs-lookup"><span data-stu-id="c5789-122">See</span></span>|  
|--------|---------|  
|<span data-ttu-id="c5789-123">Een verdelingsbron en de doelen ervoor instellen.</span><span class="sxs-lookup"><span data-stu-id="c5789-123">Set up allocation source and its targets.</span></span>|[<span data-ttu-id="c5789-124">Een verdelingsbron en de doelen ervoor instellen</span><span class="sxs-lookup"><span data-stu-id="c5789-124">Set Up Allocation Source and Targets</span></span>](finance-how-to-set-up-allocation-source-and-targets.md)|  
|<span data-ttu-id="c5789-125">Filters instellen voor dynamische toewijzingsgrondslagen.</span><span class="sxs-lookup"><span data-stu-id="c5789-125">Set up various filters for dynamic allocation bases.</span></span>|[<span data-ttu-id="c5789-126">Filters instellen voor dynamische toewijzingsgrondslagen</span><span class="sxs-lookup"><span data-stu-id="c5789-126">Setting Filters for Dynamic Allocation Bases</span></span>](finance-setting-filters-for-dynamic-allocation-bases.md)|  
|<span data-ttu-id="c5789-127">Zie een voorbeeld van hoe een statische toewijzing kan worden gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="c5789-127">See an example of how to define a static allocation.</span></span>|[<span data-ttu-id="c5789-128">Voorbeeld scenario: statische toewijzingen op basis van de verdeelsleutel definiëren</span><span class="sxs-lookup"><span data-stu-id="c5789-128">Scenario Example: Defining Static Allocations Based on Allocation Ratio</span></span>](finance-scenario-example-defining-static-allocations-based-on-allocation-ratio.md)|  
|<span data-ttu-id="c5789-129">Zie een voorbeeld van hoe een dynamische toewijzing kan worden gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="c5789-129">See an example of how to define a dynamic allocation.</span></span>|[<span data-ttu-id="c5789-130">Voorbeeld scenario: dynamische toewijzingen op basis van de verkochte artikelen definiëren</span><span class="sxs-lookup"><span data-stu-id="c5789-130">Scenario Example: Defining Dynamic Allocations Based on Items Sold</span></span>](finance-scenario-example-defining-dynamic-allocations-based-on-items-sold.md)|  

## <a name="see-also"></a><span data-ttu-id="c5789-131">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c5789-131">See Also</span></span>  
 <span data-ttu-id="c5789-132">[Kostenboekhouding instellen](finance-set-up-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="c5789-132">[Setting Up Cost Accounting](finance-set-up-cost-accounting.md) </span></span>  
 <span data-ttu-id="c5789-133">[Kostenposten overbrengen en boeken](finance-transfer-and-post-cost-entries.md) </span><span class="sxs-lookup"><span data-stu-id="c5789-133">[Transferring and Posting Cost Entries](finance-transfer-and-post-cost-entries.md) </span></span>  
 <span data-ttu-id="c5789-134">[Kosten verantwoorden](finance-manage-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="c5789-134">[Accounting for Costs](finance-manage-cost-accounting.md) </span></span>  
 <span data-ttu-id="c5789-135">[Terminologie in kostprijsboekhouding](finance-terminology-in-cost-accounting.md) </span><span class="sxs-lookup"><span data-stu-id="c5789-135">[Terminology in Cost Accounting](finance-terminology-in-cost-accounting.md) </span></span>  
 [<span data-ttu-id="c5789-136">Kostprijsboekhouding</span><span class="sxs-lookup"><span data-stu-id="c5789-136">About Cost Accounting</span></span>](finance-about-cost-accounting.md)

