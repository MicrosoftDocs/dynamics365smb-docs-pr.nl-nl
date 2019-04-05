---
title: Artikeltypen | Microsoft Docs
description: U kunt de voorraadwaarde van een artikel herwaarderen met de waarderingsmethoden FIFO of Gemiddeld, bijvoorbeeld als de kosten van een artikel veranderen om andere redenen dan transacties.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 11/18/2018
ms.author: sgroespe
ms.openlocfilehash: 2240840e977bcd1186c74972ce0457deb03058a0
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "794898"
---
# <a name="about-item-types"></a><span data-ttu-id="f17ff-103">Over artikeltypen</span><span class="sxs-lookup"><span data-stu-id="f17ff-103">About Item Types</span></span>
<span data-ttu-id="f17ff-104">In het veld **Soort** op de pagina **Artikel** kunt u selecteren waarvoor het artikel in uw bedrijf wordt gebruikt en dus hoe het wordt beheerd in het systeem.</span><span class="sxs-lookup"><span data-stu-id="f17ff-104">In the **Type** field on the **Item Card** page, you can select what the item is used for in your business and therefore how it is managed in the system.</span></span> <span data-ttu-id="f17ff-105">Er zijn drie opties:</span><span class="sxs-lookup"><span data-stu-id="f17ff-105">Three options exist:</span></span>

|<span data-ttu-id="f17ff-106">Optie</span><span class="sxs-lookup"><span data-stu-id="f17ff-106">Option</span></span>|<span data-ttu-id="f17ff-107">Gebruikelijk doel</span><span class="sxs-lookup"><span data-stu-id="f17ff-107">Typical Purpose</span></span>|
|------|-----------|
|<span data-ttu-id="f17ff-108">Voorraad</span><span class="sxs-lookup"><span data-stu-id="f17ff-108">Inventory</span></span>|<span data-ttu-id="f17ff-109">Een fysieke eenheid, bijvoorbeeld een fiets, voor volledige bedrijfsondersteuning.</span><span class="sxs-lookup"><span data-stu-id="f17ff-109">A physical unit, such as a bicycle, for full business support.</span></span>|
|<span data-ttu-id="f17ff-110">Niet-voorraad</span><span class="sxs-lookup"><span data-stu-id="f17ff-110">Non-Inventory</span></span>|<span data-ttu-id="f17ff-111">Een fysieke eenheid, zoals een bout, voor beperkte bedrijfsondersteuning, bijvoorbeeld omdat het artikel alleen intern wordt gebruikt en lage kosten heeft.</span><span class="sxs-lookup"><span data-stu-id="f17ff-111">A physical unit, such as a bolt, for limited business support, for example, because the item is only used internally and has a low cost.</span></span>|
|<span data-ttu-id="f17ff-112">Onderhoud</span><span class="sxs-lookup"><span data-stu-id="f17ff-112">Service</span></span>|<span data-ttu-id="f17ff-113">Een arbeidstijdseenheid, zoals een adviesuur, voor beperkte bedrijfsondersteuning.</span><span class="sxs-lookup"><span data-stu-id="f17ff-113">A labor time unit, such as a consultancy hour, for limited business support.</span></span>|

<span data-ttu-id="f17ff-114">Het soort **Voorraad** betreft volledige tracering van voorraadaantal en -waarde.</span><span class="sxs-lookup"><span data-stu-id="f17ff-114">The **Inventory** type involves full tracking of inventory quantity and value.</span></span> <span data-ttu-id="f17ff-115">Daarom worden alle artikeltransactiesoorten ondersteund en kunnen artikelen van het type voorraad worden gebruikt met alle functies voor artikelverwerking.</span><span class="sxs-lookup"><span data-stu-id="f17ff-115">Therefore, all item transaction types are supported, and items of type Inventory can be used with all item-handling features.</span></span>

<span data-ttu-id="f17ff-116">De typen **Service** en **Niet-voorraad** betreffen geen tracering van voorraadaantal en -waarde.</span><span class="sxs-lookup"><span data-stu-id="f17ff-116">The **Service** and **Non-Inventory** types do not involve tracking of inventory quantity and value.</span></span> <span data-ttu-id="f17ff-117">Daarom worden alleen geselecteerde artikeltransactietypen en -functies ondersteund.</span><span class="sxs-lookup"><span data-stu-id="f17ff-117">Therefore, only selected item transaction types and features are supported.</span></span>

<span data-ttu-id="f17ff-118">De drie artikeltypen ondersteunen respectievelijk de volgende functies.</span><span class="sxs-lookup"><span data-stu-id="f17ff-118">The three item types support the following features respectively.</span></span>

|<span data-ttu-id="f17ff-119">Artikelsoort</span><span class="sxs-lookup"><span data-stu-id="f17ff-119">Item Type</span></span>|<span data-ttu-id="f17ff-120">Verkoop</span><span class="sxs-lookup"><span data-stu-id="f17ff-120">Sales</span></span>|<span data-ttu-id="f17ff-121">Inkopen</span><span class="sxs-lookup"><span data-stu-id="f17ff-121">Purchasing</span></span>|<span data-ttu-id="f17ff-122">Projectverbruik</span><span class="sxs-lookup"><span data-stu-id="f17ff-122">Job Consumption</span></span>|<span data-ttu-id="f17ff-123">Serviceverbruik</span><span class="sxs-lookup"><span data-stu-id="f17ff-123">Service Consumption</span></span>|<span data-ttu-id="f17ff-124">Assemblageverbruik</span><span class="sxs-lookup"><span data-stu-id="f17ff-124">Assembly Consumption</span></span>|<span data-ttu-id="f17ff-125">Productieverbruik</span><span class="sxs-lookup"><span data-stu-id="f17ff-125">Production Consumption</span></span>|<span data-ttu-id="f17ff-126">Assemblage-uitvoer</span><span class="sxs-lookup"><span data-stu-id="f17ff-126">Assembly Output</span></span>|<span data-ttu-id="f17ff-127">Productieoutput</span><span class="sxs-lookup"><span data-stu-id="f17ff-127">Production Output</span></span>|<span data-ttu-id="f17ff-128">Locatietransfer</span><span class="sxs-lookup"><span data-stu-id="f17ff-128">Location Transfer</span></span>|<span data-ttu-id="f17ff-129">Fysieke telling</span><span class="sxs-lookup"><span data-stu-id="f17ff-129">Physical Counting</span></span>|<span data-ttu-id="f17ff-130">Voorraadherwaardering</span><span class="sxs-lookup"><span data-stu-id="f17ff-130">Inventory Revaluation</span></span>|<span data-ttu-id="f17ff-131">Voorraadwaardering</span><span class="sxs-lookup"><span data-stu-id="f17ff-131">Inventory Costing</span></span>|<span data-ttu-id="f17ff-132">Artikeltracering</span><span class="sxs-lookup"><span data-stu-id="f17ff-132">Item Tracking</span></span>|<span data-ttu-id="f17ff-133">Reservering</span><span class="sxs-lookup"><span data-stu-id="f17ff-133">Reservation</span></span>|<span data-ttu-id="f17ff-134">Magazijn</span><span class="sxs-lookup"><span data-stu-id="f17ff-134">Warehousing</span></span>|<span data-ttu-id="f17ff-135">Planning</span><span class="sxs-lookup"><span data-stu-id="f17ff-135">Planning</span></span>|
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|-|
|<span data-ttu-id="f17ff-136">Voorraad</span><span class="sxs-lookup"><span data-stu-id="f17ff-136">Inventory</span></span>|<span data-ttu-id="f17ff-137">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-137">Yes</span></span>|<span data-ttu-id="f17ff-138">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-138">Yes</span></span>|<span data-ttu-id="f17ff-139">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-139">Yes</span></span>|<span data-ttu-id="f17ff-140">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-140">Yes</span></span>|<span data-ttu-id="f17ff-141">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-141">Yes</span></span>|<span data-ttu-id="f17ff-142">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-142">Yes</span></span>|<span data-ttu-id="f17ff-143">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-143">Yes</span></span>|<span data-ttu-id="f17ff-144">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-144">Yes</span></span>|<span data-ttu-id="f17ff-145">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-145">Yes</span></span>|<span data-ttu-id="f17ff-146">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-146">Yes</span></span>|<span data-ttu-id="f17ff-147">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-147">Yes</span></span>|<span data-ttu-id="f17ff-148">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-148">Yes</span></span>|<span data-ttu-id="f17ff-149">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-149">Yes</span></span>|<span data-ttu-id="f17ff-150">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-150">Yes</span></span>|<span data-ttu-id="f17ff-151">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-151">Yes</span></span>|<span data-ttu-id="f17ff-152">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-152">Yes</span></span>|
|<span data-ttu-id="f17ff-153">Niet-voorraad</span><span class="sxs-lookup"><span data-stu-id="f17ff-153">Non-Inventory</span></span>|<span data-ttu-id="f17ff-154">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-154">Yes</span></span>|<span data-ttu-id="f17ff-155">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-155">Yes</span></span>|<span data-ttu-id="f17ff-156">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-156">Yes</span></span>|<span data-ttu-id="f17ff-157">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-157">Yes</span></span>|<span data-ttu-id="f17ff-158">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-158">Yes</span></span>|<span data-ttu-id="f17ff-159">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-159">Yes</span></span>|<span data-ttu-id="f17ff-160">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-160">No</span></span>|<span data-ttu-id="f17ff-161">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-161">No</span></span>|<span data-ttu-id="f17ff-162">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-162">No</span></span>|<span data-ttu-id="f17ff-163">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-163">No</span></span>|<span data-ttu-id="f17ff-164">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-164">No</span></span>|<span data-ttu-id="f17ff-165">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-165">No</span></span>|<span data-ttu-id="f17ff-166">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-166">No</span></span>|<span data-ttu-id="f17ff-167">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-167">No</span></span>|<span data-ttu-id="f17ff-168">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-168">No</span></span>|<span data-ttu-id="f17ff-169">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-169">No</span></span>|
|<span data-ttu-id="f17ff-170">Onderhoud</span><span class="sxs-lookup"><span data-stu-id="f17ff-170">Service</span></span>|<span data-ttu-id="f17ff-171">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-171">Yes</span></span>|<span data-ttu-id="f17ff-172">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-172">Yes</span></span>|<span data-ttu-id="f17ff-173">Ja</span><span class="sxs-lookup"><span data-stu-id="f17ff-173">Yes</span></span>|<span data-ttu-id="f17ff-174">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-174">No</span></span>|<span data-ttu-id="f17ff-175">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-175">No</span></span>|<span data-ttu-id="f17ff-176">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-176">No</span></span>|<span data-ttu-id="f17ff-177">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-177">No</span></span>|<span data-ttu-id="f17ff-178">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-178">No</span></span>|<span data-ttu-id="f17ff-179">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-179">No</span></span>|<span data-ttu-id="f17ff-180">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-180">No</span></span>|<span data-ttu-id="f17ff-181">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-181">No</span></span>|<span data-ttu-id="f17ff-182">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-182">No</span></span>|<span data-ttu-id="f17ff-183">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-183">No</span></span>|<span data-ttu-id="f17ff-184">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-184">No</span></span>|<span data-ttu-id="f17ff-185">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-185">No</span></span>|<span data-ttu-id="f17ff-186">Nr.</span><span class="sxs-lookup"><span data-stu-id="f17ff-186">No</span></span>|

> [!NOTE]
> <span data-ttu-id="f17ff-187">Artikelen die u aan uw klanten aanbiedt, maar die u niet in uw systeem wilt beheren tot u ze begint te verkopen, kunnen worden ingesteld als catalogusartikelen.</span><span class="sxs-lookup"><span data-stu-id="f17ff-187">Items that you offer to your customers but you do not want manage in your system until you start selling them can be set up as catalog items.</span></span> <span data-ttu-id="f17ff-188">Catalogusartikelen moeten niet worden verward met normale artikelen van het type Niet-voorraad.</span><span class="sxs-lookup"><span data-stu-id="f17ff-188">Catalog items are not to be mistaken with regular items of type Non-Inventory.</span></span> <span data-ttu-id="f17ff-189">Zie voor meer informatie [Werken met catalogusartikelen](inventory-how-work-nonstock-items.md).</span><span class="sxs-lookup"><span data-stu-id="f17ff-189">For more information, see [Work with Catalog Items](inventory-how-work-nonstock-items.md).</span></span>

> [!NOTE]
> <span data-ttu-id="f17ff-190">Artikelen van klanten waaraan u onderhoud verricht, zoals een printer, worden serviceartikelen genoemd.</span><span class="sxs-lookup"><span data-stu-id="f17ff-190">Customers' items that you perform service on, such as a printer, are called service items.</span></span> <span data-ttu-id="f17ff-191">Serviceartikelen hebben niets van doen met normale of catalogusartikelen.</span><span class="sxs-lookup"><span data-stu-id="f17ff-191">Service items have nothing to do with regular or catalog items.</span></span> <span data-ttu-id="f17ff-192">Serviceonderdelen kunnen echter gewone artikelen zijn.</span><span class="sxs-lookup"><span data-stu-id="f17ff-192">However, service components can be regular items.</span></span> <span data-ttu-id="f17ff-193">Zie voor meer informatie [Serviceartikelen en serviceartikelonderdelen instellen](service-how-setup-service-items.md).</span><span class="sxs-lookup"><span data-stu-id="f17ff-193">For more information, see [Set Up Service Items and Service Item Components](service-how-setup-service-items.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="f17ff-194">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f17ff-194">See Also</span></span>
[<span data-ttu-id="f17ff-195">Nieuwe artikelen registreren</span><span class="sxs-lookup"><span data-stu-id="f17ff-195">Register New Items</span></span>](inventory-how-register-new-items.md)  
[<span data-ttu-id="f17ff-196">Voorraad instellen</span><span class="sxs-lookup"><span data-stu-id="f17ff-196">Setting Up Inventory</span></span>](inventory-setup-inventory.md)  
[<span data-ttu-id="f17ff-197">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="f17ff-197">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="f17ff-198">Voorraad</span><span class="sxs-lookup"><span data-stu-id="f17ff-198">Inventory</span></span>](inventory-manage-inventory.md)  
<span data-ttu-id="f17ff-199">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="f17ff-199">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>