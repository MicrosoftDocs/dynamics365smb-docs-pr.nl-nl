---
title: 'Ontwerpdetails: Verwachte kostenboeking | Microsoft Docs'
description: Verwachte kosten zijn de schatting van, bijvoorbeeld de kosten van een ingekocht artikel, die u vastlegt voordat u de factuur voor het artikel ontvangt.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: ae88a455552c7194422d07e6e666bd81b7eab101
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "793706"
---
# <a name="design-details-expected-cost-posting"></a><span data-ttu-id="7bc9e-103">Ontwerpdetails: Verwachte kostenboeking</span><span class="sxs-lookup"><span data-stu-id="7bc9e-103">Design Details: Expected Cost Posting</span></span>
<span data-ttu-id="7bc9e-104">Verwachte kosten zijn de schatting van, bijvoorbeeld de kosten van een ingekocht artikel, die u vastlegt voordat u de factuur voor het artikel ontvangt.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-104">Expected costs represent the estimation of, for example, a purchased item’s cost that you record before you receive the invoice for the item.</span></span>  

 <span data-ttu-id="7bc9e-105">U kunt verwachte kosten boeken naar de voorraad en het grootboek.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-105">You can post expected cost to inventory and to the general ledger.</span></span> <span data-ttu-id="7bc9e-106">Wanneer u een aantal boekt dat alleen wordt ontvangen of verzonden, maar niet gefactureerd, wordt een waardepost gemaakt met de verwachte kosten.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-106">When you post a quantity that is only received or shipped but not invoiced, then a value entry is created with the expected cost.</span></span> <span data-ttu-id="7bc9e-107">Deze verwachte kosten zijn van invloed op de voorraadwaarde, maar worden niet geboekt naar het grootboek, tenzij u het systeem hebt ingesteld om dit te doen.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-107">This expected cost affects the inventory value, but is not posted to the general ledger unless you set up the system up to do so.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="7bc9e-108">Verwachte kosten worden alleen beheerd voor artikeltransacties.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-108">Expected costs are only managed for item transactions.</span></span> <span data-ttu-id="7bc9e-109">Verwachte kosten zijn niet voor immateriële transactiesoorten zoals capaciteit en artikelkosten.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-109">Expected costs are not for immaterial transaction types, such as capacity and item charges.</span></span>  

 <span data-ttu-id="7bc9e-110">Als slechts het aantaldeel van een voorraadtoename is geboekt, verandert de voorraadwaarde in het grootboek niet, tenzij u het selectievakje **Verw. kostprijs naar GB boeken** hebt geselecteerd op de pagina **Voorraadinstelling**.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-110">If only the quantity part of an inventory increase has been posted, then the inventory value in the general ledger does not change unless you have selected the **Expected Cost Posting to G/L** check box on the **Inventory Setup** page.</span></span> <span data-ttu-id="7bc9e-111">In dat geval worden de verwachte kosten geboekt naar interimrekeningen op het moment van ontvangst.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-111">In that case, the expected cost is posted to interim accounts at the time of receipt.</span></span> <span data-ttu-id="7bc9e-112">Nadat de ontvangst volledig is gefactureerd, worden de interimrekeningen vereffend en worden de werkelijke kosten geboekt naar de voorraadrekening.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-112">After the receipt has been fully invoiced, the interim accounts are then balanced and the actual cost is posted to the inventory account.</span></span>  

 <span data-ttu-id="7bc9e-113">Ter ondersteuning van reconciliatie en traceerbaarheid bevat de gefactureerde waardepost het verwachte kostenbedrag dat is geboekt om de interimrekeningen te vereffenen.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-113">To support reconciliation and traceability work, the invoiced value entry shows the expected cost amount that has been posted to balance the interim accounts.</span></span>  

## <a name="example"></a><span data-ttu-id="7bc9e-114">Opmerking</span><span class="sxs-lookup"><span data-stu-id="7bc9e-114">Example</span></span>  
 <span data-ttu-id="7bc9e-115">Het volgende voorbeeld toont verwachte kosten als het selectievakje **Autom. voorraadwaarde boeken** en **Verw. kostprijs naar GB boeken** zijn ingeschakeld op de pagina **Voorraadinstelling**.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-115">The following example shows expected cost if the **Automatic Cost Posting** check box and the **Expected Cost Posting to G/L** check box are selected on the **Inventory Setup** page.</span></span>  

 <span data-ttu-id="7bc9e-116">U boekt een inkooporder als ontvangen.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-116">You post a purchase order as received.</span></span> <span data-ttu-id="7bc9e-117">De verwachte kosten zijn LV 95,00.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-117">The expected cost is LCY 95.00.</span></span>  

 <span data-ttu-id="7bc9e-118">**Waardeposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-118">**Value Entries**</span></span>  

|<span data-ttu-id="7bc9e-119">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="7bc9e-119">Posting Date</span></span>|<span data-ttu-id="7bc9e-120">Boekingssoort</span><span class="sxs-lookup"><span data-stu-id="7bc9e-120">Entry Type</span></span>|<span data-ttu-id="7bc9e-121">Tot. verw. kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-121">Cost Amount (Expected)</span></span>|<span data-ttu-id="7bc9e-122">Verw. kostn geboekt nr grootbk</span><span class="sxs-lookup"><span data-stu-id="7bc9e-122">Expected Cost Posted to G/L</span></span>|<span data-ttu-id="7bc9e-123">Verwachte kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-123">Expected Cost</span></span>|<span data-ttu-id="7bc9e-124">Artikelpostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-124">Item Ledger Entry No.</span></span>|<span data-ttu-id="7bc9e-125">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="7bc9e-125">Entry No.</span></span>|  
|------------------|----------------|------------------------------|----------------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="7bc9e-126">01-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-126">01-01-20</span></span>|<span data-ttu-id="7bc9e-127">Directe kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-127">Direct Cost</span></span>|<span data-ttu-id="7bc9e-128">95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-128">95.00</span></span>|<span data-ttu-id="7bc9e-129">95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-129">95.00</span></span>|<span data-ttu-id="7bc9e-130">Ja</span><span class="sxs-lookup"><span data-stu-id="7bc9e-130">Yes</span></span>|<span data-ttu-id="7bc9e-131">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-131">1</span></span>|<span data-ttu-id="7bc9e-132">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-132">1</span></span>|  

 <span data-ttu-id="7bc9e-133">**Relatieposten in het grootboek - Relatietabel artikelposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-133">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="7bc9e-134">Grootboekpostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-134">G/L Entry No.</span></span>|<span data-ttu-id="7bc9e-135">Waardepostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-135">Value Entry No.</span></span>|<span data-ttu-id="7bc9e-136">Grootboekjournaalnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-136">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="7bc9e-137">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-137">1</span></span>|<span data-ttu-id="7bc9e-138">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-138">1</span></span>|<span data-ttu-id="7bc9e-139">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-139">1</span></span>|  
|<span data-ttu-id="7bc9e-140">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-140">2</span></span>|<span data-ttu-id="7bc9e-141">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-141">1</span></span>|<span data-ttu-id="7bc9e-142">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-142">1</span></span>|  

 <span data-ttu-id="7bc9e-143">**Grootboekposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-143">**General Ledger Entries**</span></span>  

|<span data-ttu-id="7bc9e-144">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="7bc9e-144">Posting Date</span></span>|<span data-ttu-id="7bc9e-145">Grootboekrekening</span><span class="sxs-lookup"><span data-stu-id="7bc9e-145">G/L Account</span></span>|<span data-ttu-id="7bc9e-146">Rekeningnr. (En-US demo)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-146">Account No. (En-US Demo)</span></span>|<span data-ttu-id="7bc9e-147">Bedrag</span><span class="sxs-lookup"><span data-stu-id="7bc9e-147">Amount</span></span>|<span data-ttu-id="7bc9e-148">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="7bc9e-148">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="7bc9e-149">01-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-149">01-01-20</span></span>|<span data-ttu-id="7bc9e-150">Voorraadtussenrekening (tussenrek.)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-150">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="7bc9e-151">5530</span><span class="sxs-lookup"><span data-stu-id="7bc9e-151">5530</span></span>|<span data-ttu-id="7bc9e-152">-95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-152">-95.00</span></span>|<span data-ttu-id="7bc9e-153">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-153">2</span></span>|  
|<span data-ttu-id="7bc9e-154">01-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-154">01-01-20</span></span>|<span data-ttu-id="7bc9e-155">Voorraadrekening (tussenrek.)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-155">Inventory Account (Interim)</span></span>|<span data-ttu-id="7bc9e-156">2131</span><span class="sxs-lookup"><span data-stu-id="7bc9e-156">2131</span></span>|<span data-ttu-id="7bc9e-157">95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-157">95.00</span></span>|<span data-ttu-id="7bc9e-158">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-158">1</span></span>|  

 <span data-ttu-id="7bc9e-159">U kunt de inkooporder op een later moment boeken als gefactureerd.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-159">At a later date, you post the purchase order as invoiced.</span></span> <span data-ttu-id="7bc9e-160">De gefactureerde kosten zijn LV 100,00.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-160">The invoiced cost is LCY 100.00.</span></span>  

 <span data-ttu-id="7bc9e-161">**Waardeposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-161">**Value Entries**</span></span>  

|<span data-ttu-id="7bc9e-162">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="7bc9e-162">Posting Date</span></span>|<span data-ttu-id="7bc9e-163">Tot. werk. kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-163">Cost Amount (Actual)</span></span>|<span data-ttu-id="7bc9e-164">Tot. verw. kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-164">Cost Amount (Expected)</span></span>|<span data-ttu-id="7bc9e-165">Vrd.-waarde geboekt</span><span class="sxs-lookup"><span data-stu-id="7bc9e-165">Cost Posted to G/L</span></span>|<span data-ttu-id="7bc9e-166">Verwachte kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-166">Expected Cost</span></span>|<span data-ttu-id="7bc9e-167">Artikelpostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-167">Item Ledger Entry No.</span></span>|<span data-ttu-id="7bc9e-168">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="7bc9e-168">Entry No.</span></span>|  
|------------------|----------------------------|------------------------------|-------------------------|-------------------|---------------------------|---------------|  
|<span data-ttu-id="7bc9e-169">15-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-169">01-15-20</span></span>|<span data-ttu-id="7bc9e-170">100.00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-170">100.00</span></span>|<span data-ttu-id="7bc9e-171">-95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-171">-95.00</span></span>|<span data-ttu-id="7bc9e-172">100.00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-172">100.00</span></span>|<span data-ttu-id="7bc9e-173">Nee</span><span class="sxs-lookup"><span data-stu-id="7bc9e-173">No</span></span>|<span data-ttu-id="7bc9e-174">1</span><span class="sxs-lookup"><span data-stu-id="7bc9e-174">1</span></span>|<span data-ttu-id="7bc9e-175">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-175">2</span></span>|  

 <span data-ttu-id="7bc9e-176">**Relatieposten in het grootboek - Relatietabel artikelposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-176">**Relation Entries in the G/L – Item Ledger Relation Table**</span></span>  

|<span data-ttu-id="7bc9e-177">Grootboekpostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-177">G/L Entry No.</span></span>|<span data-ttu-id="7bc9e-178">Waardepostnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-178">Value Entry No.</span></span>|<span data-ttu-id="7bc9e-179">Grootboekjournaalnr.</span><span class="sxs-lookup"><span data-stu-id="7bc9e-179">G/L Register No.</span></span>|  
|--------------------|---------------------|-----------------------|  
|<span data-ttu-id="7bc9e-180">3</span><span class="sxs-lookup"><span data-stu-id="7bc9e-180">3</span></span>|<span data-ttu-id="7bc9e-181">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-181">2</span></span>|<span data-ttu-id="7bc9e-182">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-182">2</span></span>|  
|<span data-ttu-id="7bc9e-183">4</span><span class="sxs-lookup"><span data-stu-id="7bc9e-183">4</span></span>|<span data-ttu-id="7bc9e-184">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-184">2</span></span>|<span data-ttu-id="7bc9e-185">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-185">2</span></span>|  
|<span data-ttu-id="7bc9e-186">5</span><span class="sxs-lookup"><span data-stu-id="7bc9e-186">5</span></span>|<span data-ttu-id="7bc9e-187">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-187">2</span></span>|<span data-ttu-id="7bc9e-188">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-188">2</span></span>|  
|<span data-ttu-id="7bc9e-189">6</span><span class="sxs-lookup"><span data-stu-id="7bc9e-189">6</span></span>|<span data-ttu-id="7bc9e-190">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-190">2</span></span>|<span data-ttu-id="7bc9e-191">2</span><span class="sxs-lookup"><span data-stu-id="7bc9e-191">2</span></span>|  

 <span data-ttu-id="7bc9e-192">**Grootboekposten**</span><span class="sxs-lookup"><span data-stu-id="7bc9e-192">**General Ledger Entries**</span></span>  

|<span data-ttu-id="7bc9e-193">Boekingsdatum</span><span class="sxs-lookup"><span data-stu-id="7bc9e-193">Posting Date</span></span>|<span data-ttu-id="7bc9e-194">Grootboekrekening</span><span class="sxs-lookup"><span data-stu-id="7bc9e-194">G/L Account</span></span>|<span data-ttu-id="7bc9e-195">Rekeningnr. (En-US demo)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-195">Account No. (En-US Demo)</span></span>|<span data-ttu-id="7bc9e-196">Bedrag</span><span class="sxs-lookup"><span data-stu-id="7bc9e-196">Amount</span></span>|<span data-ttu-id="7bc9e-197">Volgnummer</span><span class="sxs-lookup"><span data-stu-id="7bc9e-197">Entry No.</span></span>|  
|------------------|------------------|---------------------------------|------------|---------------|  
|<span data-ttu-id="7bc9e-198">15-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-198">01-15-20</span></span>|<span data-ttu-id="7bc9e-199">Voorraadtussenrekening (tussenrek.)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-199">Inventory Accrual Account (Interim)</span></span>|<span data-ttu-id="7bc9e-200">5530</span><span class="sxs-lookup"><span data-stu-id="7bc9e-200">5530</span></span>|<span data-ttu-id="7bc9e-201">95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-201">95.00</span></span>|<span data-ttu-id="7bc9e-202">4</span><span class="sxs-lookup"><span data-stu-id="7bc9e-202">4</span></span>|  
|<span data-ttu-id="7bc9e-203">15-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-203">01-15-20</span></span>|<span data-ttu-id="7bc9e-204">Voorraadrekening (tussenrek.)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-204">Inventory Account (Interim)</span></span>|<span data-ttu-id="7bc9e-205">2131</span><span class="sxs-lookup"><span data-stu-id="7bc9e-205">2131</span></span>|<span data-ttu-id="7bc9e-206">-95,00</span><span class="sxs-lookup"><span data-stu-id="7bc9e-206">-95.00</span></span>|<span data-ttu-id="7bc9e-207">3</span><span class="sxs-lookup"><span data-stu-id="7bc9e-207">3</span></span>|  
|<span data-ttu-id="7bc9e-208">15-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-208">01-15-20</span></span>|<span data-ttu-id="7bc9e-209">Vereffeningsrekening directe kosten</span><span class="sxs-lookup"><span data-stu-id="7bc9e-209">Direct Cost Applied Account</span></span>|<span data-ttu-id="7bc9e-210">7291</span><span class="sxs-lookup"><span data-stu-id="7bc9e-210">7291</span></span>|<span data-ttu-id="7bc9e-211">-100</span><span class="sxs-lookup"><span data-stu-id="7bc9e-211">-100</span></span>|<span data-ttu-id="7bc9e-212">6</span><span class="sxs-lookup"><span data-stu-id="7bc9e-212">6</span></span>|  
|<span data-ttu-id="7bc9e-213">15-01-20</span><span class="sxs-lookup"><span data-stu-id="7bc9e-213">01-15-20</span></span>|<span data-ttu-id="7bc9e-214">Voorraadrekening</span><span class="sxs-lookup"><span data-stu-id="7bc9e-214">Inventory Account</span></span>|<span data-ttu-id="7bc9e-215">2130</span><span class="sxs-lookup"><span data-stu-id="7bc9e-215">2130</span></span>|<span data-ttu-id="7bc9e-216">100</span><span class="sxs-lookup"><span data-stu-id="7bc9e-216">100</span></span>|<span data-ttu-id="7bc9e-217">5</span><span class="sxs-lookup"><span data-stu-id="7bc9e-217">5</span></span>|  

## <a name="see-also"></a><span data-ttu-id="7bc9e-218">Zie ook</span><span class="sxs-lookup"><span data-stu-id="7bc9e-218">See Also</span></span>
 <span data-ttu-id="7bc9e-219">[Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md) </span><span class="sxs-lookup"><span data-stu-id="7bc9e-219">[Design Details: Inventory Costing](design-details-inventory-costing.md) </span></span>  
 <span data-ttu-id="7bc9e-220">[Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md) </span><span class="sxs-lookup"><span data-stu-id="7bc9e-220">[Design Details: Cost Adjustment](design-details-cost-adjustment.md) </span></span>  
 <span data-ttu-id="7bc9e-221">[Ontwerpdetails: Reconciliatie met het grootboek](design-details-reconciliation-with-the-general-ledger.md) </span><span class="sxs-lookup"><span data-stu-id="7bc9e-221">[Design Details: Reconciliation with the General Ledger](design-details-reconciliation-with-the-general-ledger.md) </span></span>  
 <span data-ttu-id="7bc9e-222">[Ontwerpdetails: Voorraadboeking](design-details-inventory-posting.md) </span><span class="sxs-lookup"><span data-stu-id="7bc9e-222">[Design Details: Inventory Posting](design-details-inventory-posting.md) </span></span>  
 [<span data-ttu-id="7bc9e-223">Ontwerpdetails: Verschil</span><span class="sxs-lookup"><span data-stu-id="7bc9e-223">Design Details: Variance</span></span>](design-details-variance.md)  
 [<span data-ttu-id="7bc9e-224">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="7bc9e-224">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
 [<span data-ttu-id="7bc9e-225">Financiën</span><span class="sxs-lookup"><span data-stu-id="7bc9e-225">Finance</span></span>](finance.md)  
 <span data-ttu-id="7bc9e-226">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7bc9e-226">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>