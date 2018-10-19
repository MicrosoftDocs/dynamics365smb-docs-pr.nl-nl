---
title: Artikeltypen | Microsoft Docs
description: U kunt de voorraadwaarde van een artikel herwaarderen met de waarderingsmethoden FIFO of Gemiddeld, bijvoorbeeld als de kosten van een artikel veranderen om andere redenen dan transacties.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: b976ca548bf02511e818fa981395cb9261757468
ms.contentlocale: nl-nl
ms.lasthandoff: 09/28/2018

---
# <a name="about-item-types"></a><span data-ttu-id="36a7f-103">Over artikeltypen</span><span class="sxs-lookup"><span data-stu-id="36a7f-103">About Item Types</span></span>
<span data-ttu-id="36a7f-104">In het veld **Soort** in het venster **Artikel** kunt u selecteren waarvoor het artikel in uw bedrijf wordt gebruikt en dus hoe het wordt beheerd in het systeem.</span><span class="sxs-lookup"><span data-stu-id="36a7f-104">In the **Type** field in the **Item Card** window, you can select what the item is used for in your business and therefore how it is managed in the system.</span></span> <span data-ttu-id="36a7f-105">Er zijn drie opties:</span><span class="sxs-lookup"><span data-stu-id="36a7f-105">Three options exist:</span></span>

|<span data-ttu-id="36a7f-106">Optie</span><span class="sxs-lookup"><span data-stu-id="36a7f-106">Option</span></span>|<span data-ttu-id="36a7f-107">Gebruikelijk doel</span><span class="sxs-lookup"><span data-stu-id="36a7f-107">Typical Purpose</span></span>|
|------|-----------|
|<span data-ttu-id="36a7f-108">Voorraad</span><span class="sxs-lookup"><span data-stu-id="36a7f-108">Inventory</span></span>|<span data-ttu-id="36a7f-109">Een fysieke eenheid, bijvoorbeeld een fiets, voor volledige bedrijfsondersteuning.</span><span class="sxs-lookup"><span data-stu-id="36a7f-109">A physical unit, such as a bicycle, for full business support.</span></span>|
|<span data-ttu-id="36a7f-110">Niet-voorraad</span><span class="sxs-lookup"><span data-stu-id="36a7f-110">Non-Inventory</span></span>|<span data-ttu-id="36a7f-111">Een fysieke eenheid, zoals een bout, voor beperkte bedrijfsondersteuning, bijvoorbeeld omdat het artikel alleen intern wordt gebruikt en lage kosten heeft.</span><span class="sxs-lookup"><span data-stu-id="36a7f-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span></span>|
|<span data-ttu-id="36a7f-112">Onderhoud</span><span class="sxs-lookup"><span data-stu-id="36a7f-112">Service</span></span>|<span data-ttu-id="36a7f-113">Een arbeidstijdseenheid, zoals een adviesuur, voor beperkte bedrijfsondersteuning.</span><span class="sxs-lookup"><span data-stu-id="36a7f-113">A labor time unit, such as a consultancy hour, for limited business support.</span></span>|

<span data-ttu-id="36a7f-114">Het soort **Voorraad** betreft volledige tracering van voorraadaantal en -waarde.</span><span class="sxs-lookup"><span data-stu-id="36a7f-114">The **Inventory** type involves full tracking of inventory quantity and value.</span></span> <span data-ttu-id="36a7f-115">Daarom worden alle artikeltransactiesoorten ondersteund en kunnen artikelen van het type voorraad worden gebruikt met alle functies voor artikelverwerking.</span><span class="sxs-lookup"><span data-stu-id="36a7f-115">Therefore, all item transaction types are supported, and items of type Inventory can be used with all item-handling features.</span></span>

<span data-ttu-id="36a7f-116">De typen **Service** en **Niet-voorraad** betreffen geen tracering van voorraadaantal en -waarde.</span><span class="sxs-lookup"><span data-stu-id="36a7f-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span></span> <span data-ttu-id="36a7f-117">Daarom worden alleen geselecteerde artikeltransactietypen en -functies ondersteund.</span><span class="sxs-lookup"><span data-stu-id="36a7f-117">Therefore, only selected item transaction types and features are supported.</span></span>

<span data-ttu-id="36a7f-118">De drie artikeltypen ondersteunen respectievelijk de volgende functies.</span><span class="sxs-lookup"><span data-stu-id="36a7f-118">The three item types support the following features respectively.</span></span>

|<span data-ttu-id="36a7f-119">Artikelsoort</span><span class="sxs-lookup"><span data-stu-id="36a7f-119">Item Type</span></span>|<span data-ttu-id="36a7f-120">Verkoop</span><span class="sxs-lookup"><span data-stu-id="36a7f-120">Sales</span></span>|<span data-ttu-id="36a7f-121">Inkopen</span><span class="sxs-lookup"><span data-stu-id="36a7f-121">Purchasing</span></span>|<span data-ttu-id="36a7f-122">Projectverbruik</span><span class="sxs-lookup"><span data-stu-id="36a7f-122">Job Consumption</span></span>|<span data-ttu-id="36a7f-123">Serviceverbruik</span><span class="sxs-lookup"><span data-stu-id="36a7f-123">Service Consumption</span></span>|<span data-ttu-id="36a7f-124">Assemblageverbruik</span><span class="sxs-lookup"><span data-stu-id="36a7f-124">Assembly Consumption</span></span>|<span data-ttu-id="36a7f-125">Productieverbruik</span><span class="sxs-lookup"><span data-stu-id="36a7f-125">Production Consumption</span></span>|<span data-ttu-id="36a7f-126">Assemblyuitvoer</span><span class="sxs-lookup"><span data-stu-id="36a7f-126">Assemply Output</span></span>|<span data-ttu-id="36a7f-127">Productieoutput</span><span class="sxs-lookup"><span data-stu-id="36a7f-127">Production Output</span></span>|<span data-ttu-id="36a7f-128">Locatietransfer</span><span class="sxs-lookup"><span data-stu-id="36a7f-128">Location Transfer</span></span>|<span data-ttu-id="36a7f-129">Fysieke telling</span><span class="sxs-lookup"><span data-stu-id="36a7f-129">Physical Counting</span></span>|<span data-ttu-id="36a7f-130">Voorraadherwaardering</span><span class="sxs-lookup"><span data-stu-id="36a7f-130">Inventory Revaluation</span></span>|<span data-ttu-id="36a7f-131">Voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="36a7f-131">Inventory Costing</span></span>|<span data-ttu-id="36a7f-132">Artikeltracering</span><span class="sxs-lookup"><span data-stu-id="36a7f-132">Item Tracking</span></span>|<span data-ttu-id="36a7f-133">Reservering</span><span class="sxs-lookup"><span data-stu-id="36a7f-133">Reservation</span></span>|<span data-ttu-id="36a7f-134">Magazijn</span><span class="sxs-lookup"><span data-stu-id="36a7f-134">Warehousing</span></span>|<span data-ttu-id="36a7f-135">Planning</span><span class="sxs-lookup"><span data-stu-id="36a7f-135">Planning</span></span>|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|<span data-ttu-id="36a7f-136">Voorraad</span><span class="sxs-lookup"><span data-stu-id="36a7f-136">Inventory</span></span>|<span data-ttu-id="36a7f-137">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-137">Yes</span></span>|<span data-ttu-id="36a7f-138">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-138">Yes</span></span>|<span data-ttu-id="36a7f-139">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-139">Yes</span></span>|<span data-ttu-id="36a7f-140">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-140">Yes</span></span>|<span data-ttu-id="36a7f-141">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-141">Yes</span></span>|<span data-ttu-id="36a7f-142">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-142">Yes</span></span>|<span data-ttu-id="36a7f-143">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-143">Yes</span></span>|<span data-ttu-id="36a7f-144">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-144">Yes</span></span>|<span data-ttu-id="36a7f-145">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-145">Yes</span></span>|<span data-ttu-id="36a7f-146">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-146">Yes</span></span>|<span data-ttu-id="36a7f-147">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-147">Yes</span></span>|<span data-ttu-id="36a7f-148">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-148">Yes</span></span>|<span data-ttu-id="36a7f-149">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-149">Yes</span></span>|<span data-ttu-id="36a7f-150">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-150">Yes</span></span>|<span data-ttu-id="36a7f-151">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-151">Yes</span></span>|<span data-ttu-id="36a7f-152">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-152">Yes</span></span>|
|<span data-ttu-id="36a7f-153">Niet-voorraad</span><span class="sxs-lookup"><span data-stu-id="36a7f-153">Non-Inventory</span></span>|<span data-ttu-id="36a7f-154">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-154">Yes</span></span>|<span data-ttu-id="36a7f-155">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-155">Yes</span></span>|<span data-ttu-id="36a7f-156">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-156">Yes</span></span>|<span data-ttu-id="36a7f-157">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-157">Yes</span></span>|<span data-ttu-id="36a7f-158">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-158">Yes</span></span>|<span data-ttu-id="36a7f-159">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-159">Yes</span></span>|<span data-ttu-id="36a7f-160">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-160">Yes</span></span>|<span data-ttu-id="36a7f-161">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-161">No</span></span>|<span data-ttu-id="36a7f-162">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-162">No</span></span>|<span data-ttu-id="36a7f-163">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-163">No</span></span>|<span data-ttu-id="36a7f-164">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-164">No</span></span>|<span data-ttu-id="36a7f-165">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-165">No</span></span>|<span data-ttu-id="36a7f-166">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-166">No</span></span>|<span data-ttu-id="36a7f-167">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-167">No</span></span>|<span data-ttu-id="36a7f-168">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-168">No</span></span>|<span data-ttu-id="36a7f-169">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-169">No</span></span>|
|<span data-ttu-id="36a7f-170">Onderhoud</span><span class="sxs-lookup"><span data-stu-id="36a7f-170">Service</span></span>|<span data-ttu-id="36a7f-171">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-171">Yes</span></span>|<span data-ttu-id="36a7f-172">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-172">Yes</span></span>|<span data-ttu-id="36a7f-173">Ja</span><span class="sxs-lookup"><span data-stu-id="36a7f-173">Yes</span></span>|<span data-ttu-id="36a7f-174">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-174">No</span></span>|<span data-ttu-id="36a7f-175">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-175">No</span></span>|<span data-ttu-id="36a7f-176">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-176">No</span></span>|<span data-ttu-id="36a7f-177">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-177">No</span></span>|<span data-ttu-id="36a7f-178">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-178">No</span></span>|<span data-ttu-id="36a7f-179">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-179">No</span></span>|<span data-ttu-id="36a7f-180">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-180">No</span></span>|<span data-ttu-id="36a7f-181">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-181">No</span></span>|<span data-ttu-id="36a7f-182">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-182">No</span></span>|<span data-ttu-id="36a7f-183">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-183">No</span></span>|<span data-ttu-id="36a7f-184">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-184">No</span></span>|<span data-ttu-id="36a7f-185">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-185">No</span></span>|<span data-ttu-id="36a7f-186">Nr.</span><span class="sxs-lookup"><span data-stu-id="36a7f-186">No</span></span>|

> [!NOTE]
> <span data-ttu-id="36a7f-187">Artikelen die u aan uw klanten aanbiedt, maar die u niet in uw systeem wilt beheren tot u ze begint te verkopen, kunnen worden ingesteld als catalogusartikelen.</span><span class="sxs-lookup"><span data-stu-id="36a7f-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalog items.</span></span> <span data-ttu-id="36a7f-188">Catalogusartikelen moeten niet worden verward met normale artikelen van het type Niet-voorraad.</span><span class="sxs-lookup"><span data-stu-id="36a7f-188">Catalog items are not to be mistaken with regular items of type Non-Inventory.</span></span> <span data-ttu-id="36a7f-189">Zie voor meer informatie [Werken met catalogusartikelen](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="36a7f-189">For more information, see [Work with Catalog Items](inventory-how-work-nonstock-items.md).</span></span>

> [!NOTE]
> <span data-ttu-id="36a7f-190">Artikelen van klanten waaraan u onderhoud verricht, zoals een printer, worden serviceartikelen genoemd.</span><span class="sxs-lookup"><span data-stu-id="36a7f-190">Customers' items that you perform service on, such as a printer, are called service items.</span></span> <span data-ttu-id="36a7f-191">Serviceartikelen hebben niets van doen met normale of catalogusartikelen.</span><span class="sxs-lookup"><span data-stu-id="36a7f-191">Service items have nothing to do with regular or catalog items.</span></span> <span data-ttu-id="36a7f-192">Serviceonderdelen kunnen echter gewone artikelen zijn.</span><span class="sxs-lookup"><span data-stu-id="36a7f-192">However, service components can be regular items.</span></span> <span data-ttu-id="36a7f-193">Zie voor meer informatie [Serviceartikelen en serviceartikelonderdelen instellen](service-how-setup-service-items.md).</span><span class="sxs-lookup"><span data-stu-id="36a7f-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="36a7f-194">Zie ook</span><span class="sxs-lookup"><span data-stu-id="36a7f-194">See Also</span></span>
[<span data-ttu-id="36a7f-195">Nieuwe artikelen registreren</span><span class="sxs-lookup"><span data-stu-id="36a7f-195">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="36a7f-196">Voorraad instellen</span><span class="sxs-lookup"><span data-stu-id="36a7f-196">Setting Up Inventory</span></span>](inventory-setup-inventory.md)  
[<span data-ttu-id="36a7f-197">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="36a7f-197">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="36a7f-198">Voorraad</span><span class="sxs-lookup"><span data-stu-id="36a7f-198">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="36a7f-199">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="36a7f-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>
