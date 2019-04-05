---
title: 'Ontwerpdetails - Wijzigingen in codeunit 12: Toewijzing algemene variabelen voor dagboekboekingsregel | Microsoft Docs'
description: De volgende wijzigingen zijn geïmplementeerd in deze versie van Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 9cb19558c8c441eac188504e798ca36d86b599d5
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "794379"
---
# <a name="codeunit-12-changes-mapping-global-variables-for-general-journal-post-line"></a><span data-ttu-id="e61e2-103">Wijzigingen in codeunit 12: Toewijzing algemene variabelen voor dagboekboekingsregel</span><span class="sxs-lookup"><span data-stu-id="e61e2-103">Codeunit 12 Changes: Mapping Global Variables for General Journal Post Line</span></span>
<span data-ttu-id="e61e2-104">De volgende wijzigingen zijn geïmplementeerd in deze versie van [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="e61e2-104">The following changes have been implemented in this release of [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  

|<span data-ttu-id="e61e2-105">**Microsoft Dynamics NAV 2009 R2**</span><span class="sxs-lookup"><span data-stu-id="e61e2-105">**Microsoft Dynamics NAV 2009 R2**</span></span>|<span data-ttu-id="e61e2-106">**Microsoft Dynamics NAV 2013 R2**</span><span class="sxs-lookup"><span data-stu-id="e61e2-106">**Microsoft Dynamics NAV 2013 R2**</span></span>|<span data-ttu-id="e61e2-107">**Opmerking**</span><span class="sxs-lookup"><span data-stu-id="e61e2-107">**Comment**</span></span>|  
|----------------------------------------|----------------------------------------|-----------------|  
|<span data-ttu-id="e61e2-108">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="e61e2-108">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="e61e2-109">GLSetup@1009 : Record 98;</span><span class="sxs-lookup"><span data-stu-id="e61e2-109">GLSetup@1009 : Record 98;</span></span>|<span data-ttu-id="e61e2-110">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-110">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-111">SalesSetup@1010 : Record 311;</span><span class="sxs-lookup"><span data-stu-id="e61e2-111">SalesSetup@1010 : Record 311;</span></span>||<span data-ttu-id="e61e2-112">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-112">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-113">PurchSetup@1011 : Record 312;</span><span class="sxs-lookup"><span data-stu-id="e61e2-113">PurchSetup@1011 : Record 312;</span></span>||<span data-ttu-id="e61e2-114">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-114">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-115">AccountingPeriod@1012 : Record 50;</span><span class="sxs-lookup"><span data-stu-id="e61e2-115">AccountingPeriod@1012 : Record 50;</span></span>||<span data-ttu-id="e61e2-116">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-116">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-117">GLAcc@1013 : Record 15;</span><span class="sxs-lookup"><span data-stu-id="e61e2-117">GLAcc@1013 : Record 15;</span></span>||<span data-ttu-id="e61e2-118">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-118">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-119">GLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-119">GLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="e61e2-120">GlobalGLEntry@1014 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-120">GlobalGLEntry@1014 : Record 17;</span></span>|<span data-ttu-id="e61e2-121">Naam gewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-121">Renamed</span></span>|  
|<span data-ttu-id="e61e2-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-122">GLEntryTmp@1015 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e61e2-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-123">TempGLEntryBuf@1010 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e61e2-124">Naam gewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-124">Renamed</span></span>|  
|<span data-ttu-id="e61e2-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-125">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e61e2-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-126">TempGLEntryVAT@1016 : TEMPORARY Record 17;</span></span>|<span data-ttu-id="e61e2-127">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-127">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-128">OrigGLEntry@1017 : Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-128">OrigGLEntry@1017 : Record 17;</span></span>||<span data-ttu-id="e61e2-129">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="e61e2-129">Deleted</span></span>|  
|<span data-ttu-id="e61e2-130">VATPostingSetup@1019 : Record 325;</span><span class="sxs-lookup"><span data-stu-id="e61e2-130">VATPostingSetup@1019 : Record 325;</span></span>||<span data-ttu-id="e61e2-131">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-131">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-132">Cust@1020 : Record 18;</span><span class="sxs-lookup"><span data-stu-id="e61e2-132">Cust@1020 : Record 18;</span></span>||<span data-ttu-id="e61e2-133">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-133">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-134">Vend@1021 : Record 23;</span><span class="sxs-lookup"><span data-stu-id="e61e2-134">Vend@1021 : Record 23;</span></span>||<span data-ttu-id="e61e2-135">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-135">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-136">GenJnlLine@1022 : Record 81;</span><span class="sxs-lookup"><span data-stu-id="e61e2-136">GenJnlLine@1022 : Record 81;</span></span>||<span data-ttu-id="e61e2-137">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-137">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-138">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="e61e2-138">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="e61e2-139">GLReg@1029 : Record 45;</span><span class="sxs-lookup"><span data-stu-id="e61e2-139">GLReg@1029 : Record 45;</span></span>|<span data-ttu-id="e61e2-140">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-140">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-141">CustPostingGr@1030 : Record 92;</span><span class="sxs-lookup"><span data-stu-id="e61e2-141">CustPostingGr@1030 : Record 92;</span></span>||<span data-ttu-id="e61e2-142">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-142">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-143">VendPostingGr@1031 : Record 93;</span><span class="sxs-lookup"><span data-stu-id="e61e2-143">VendPostingGr@1031 : Record 93;</span></span>||<span data-ttu-id="e61e2-144">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-144">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-145">Currency@1032 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="e61e2-145">Currency@1032 : Record 4;</span></span>||<span data-ttu-id="e61e2-146">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-146">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-147">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="e61e2-147">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="e61e2-148">AddCurrency@1033 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="e61e2-148">AddCurrency@1033 : Record 4;</span></span>|<span data-ttu-id="e61e2-149">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-149">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-150">ApplnCurrency@1034 : Record 4;</span><span class="sxs-lookup"><span data-stu-id="e61e2-150">ApplnCurrency@1034 : Record 4;</span></span>||<span data-ttu-id="e61e2-151">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-151">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-152">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="e61e2-152">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="e61e2-153">CurrExchRate@1035 : Record 330;</span><span class="sxs-lookup"><span data-stu-id="e61e2-153">CurrExchRate@1035 : Record 330;</span></span>|<span data-ttu-id="e61e2-154">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-154">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-155">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="e61e2-155">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="e61e2-156">VATEntry@1038 : Record 254;</span><span class="sxs-lookup"><span data-stu-id="e61e2-156">VATEntry@1038 : Record 254;</span></span>|<span data-ttu-id="e61e2-157">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-157">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-158">BankAcc@1039 : Record 270;</span><span class="sxs-lookup"><span data-stu-id="e61e2-158">BankAcc@1039 : Record 270;</span></span>||<span data-ttu-id="e61e2-159">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-159">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-160">BankAccLedgEntry@1040 : Record 271;</span><span class="sxs-lookup"><span data-stu-id="e61e2-160">BankAccLedgEntry@1040 : Record 271;</span></span>||<span data-ttu-id="e61e2-161">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-161">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-162">CheckLedgEntry@1041 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="e61e2-162">CheckLedgEntry@1041 : Record 272;</span></span>||<span data-ttu-id="e61e2-163">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-163">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-164">CheckLedgEntry2@1042 : Record 272;</span><span class="sxs-lookup"><span data-stu-id="e61e2-164">CheckLedgEntry2@1042 : Record 272;</span></span>||<span data-ttu-id="e61e2-165">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-165">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-166">BankAccPostingGr@1043 : Record 277;</span><span class="sxs-lookup"><span data-stu-id="e61e2-166">BankAccPostingGr@1043 : Record 277;</span></span>||<span data-ttu-id="e61e2-167">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-167">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-168">GenJnlTemplate@1044 : Record 80;</span><span class="sxs-lookup"><span data-stu-id="e61e2-168">GenJnlTemplate@1044 : Record 80;</span></span>||<span data-ttu-id="e61e2-169">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-169">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-170">TaxJurisdiction@1045 : Record 320;</span><span class="sxs-lookup"><span data-stu-id="e61e2-170">TaxJurisdiction@1045 : Record 320;</span></span>||<span data-ttu-id="e61e2-171">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-171">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-172">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="e61e2-172">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="e61e2-173">TaxDetail@1046 : Record 322;</span><span class="sxs-lookup"><span data-stu-id="e61e2-173">TaxDetail@1046 : Record 322;</span></span>|<span data-ttu-id="e61e2-174">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-174">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span><span class="sxs-lookup"><span data-stu-id="e61e2-175">FAGLPostBuf@1047 : TEMPORARY Record 5637;</span></span>||<span data-ttu-id="e61e2-176">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-176">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-177">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="e61e2-177">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="e61e2-178">UnrealizedCustLedgEntry@1084 : Record 21;</span><span class="sxs-lookup"><span data-stu-id="e61e2-178">UnrealizedCustLedgEntry@1084 : Record 21;</span></span>|<span data-ttu-id="e61e2-179">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-179">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-180">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="e61e2-180">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="e61e2-181">UnrealizedVendLedgEntry@1085 : Record 25;</span><span class="sxs-lookup"><span data-stu-id="e61e2-181">UnrealizedVendLedgEntry@1085 : Record 25;</span></span>|<span data-ttu-id="e61e2-182">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-182">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-183">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="e61e2-183">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="e61e2-184">GLEntryVATEntryLink@1087 : Record 253;</span><span class="sxs-lookup"><span data-stu-id="e61e2-184">GLEntryVATEntryLink@1087 : Record 253;</span></span>|<span data-ttu-id="e61e2-185">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-185">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-186">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="e61e2-186">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="e61e2-187">TempVATEntry@1088 : TEMPORARY Record 254;</span><span class="sxs-lookup"><span data-stu-id="e61e2-187">TempVATEntry@1088 : TEMPORARY Record 254;</span></span>|<span data-ttu-id="e61e2-188">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-188">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span><span class="sxs-lookup"><span data-stu-id="e61e2-189">ReversedGLEntryTemp@1089 : TEMPORARY Record 17;</span></span>||<span data-ttu-id="e61e2-190">Verplaatst naar Codeunit17</span><span class="sxs-lookup"><span data-stu-id="e61e2-190">Moved to Codeunit17</span></span>|  
|<span data-ttu-id="e61e2-191">CostAccSetup@1092 : Record 1108;</span><span class="sxs-lookup"><span data-stu-id="e61e2-191">CostAccSetup@1092 : Record 1108;</span></span>||<span data-ttu-id="e61e2-192">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-192">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-193">GenJnlCheckLine@1048 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="e61e2-193">GenJnlCheckLine@1048 : Codeunit 11;</span></span>|<span data-ttu-id="e61e2-194">GenJnlCheckLine@1001 : Codeunit 11;</span><span class="sxs-lookup"><span data-stu-id="e61e2-194">GenJnlCheckLine@1001 : Codeunit 11;</span></span>|<span data-ttu-id="e61e2-195">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-195">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span><span class="sxs-lookup"><span data-stu-id="e61e2-196">ExchAccGLJnlLine@1049 : Codeunit 366;</span></span>||<span data-ttu-id="e61e2-197">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-197">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-198">FAJnlPostLine@1050 : Codeunit 5632;</span><span class="sxs-lookup"><span data-stu-id="e61e2-198">FAJnlPostLine@1050 : Codeunit 5632;</span></span>||<span data-ttu-id="e61e2-199">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-199">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-200">SalesTaxCalculate@1051 : Codeunit 398;</span><span class="sxs-lookup"><span data-stu-id="e61e2-200">SalesTaxCalculate@1051 : Codeunit 398;</span></span>||<span data-ttu-id="e61e2-201">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-201">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-202">GenJnlApply@1052 : Codeunit 225;</span><span class="sxs-lookup"><span data-stu-id="e61e2-202">GenJnlApply@1052 : Codeunit 225;</span></span>||<span data-ttu-id="e61e2-203">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-203">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-204">DimMgt@1053 : Codeunit 408;</span><span class="sxs-lookup"><span data-stu-id="e61e2-204">DimMgt@1053 : Codeunit 408;</span></span>||<span data-ttu-id="e61e2-205">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-205">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-206">JobPostLine@1028 : Codeunit 1001;</span><span class="sxs-lookup"><span data-stu-id="e61e2-206">JobPostLine@1028 : Codeunit 1001;</span></span>||<span data-ttu-id="e61e2-207">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-207">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span><span class="sxs-lookup"><span data-stu-id="e61e2-208">TransferGlEntriesToCA@1091 : Codeunit 1105;</span></span>||<span data-ttu-id="e61e2-209">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-209">Changed to Local</span></span>|  
||<span data-ttu-id="e61e2-210">PaymentToleranceMgt@1002 : Codeunit 426;</span><span class="sxs-lookup"><span data-stu-id="e61e2-210">PaymentToleranceMgt@1002 : Codeunit 426;</span></span>|<span data-ttu-id="e61e2-211">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="e61e2-211">Added</span></span>|  
||<span data-ttu-id="e61e2-212">AddCurrencyCode@1117 : Code[10];</span><span class="sxs-lookup"><span data-stu-id="e61e2-212">AddCurrencyCode@1117 : Code[10];</span></span>|<span data-ttu-id="e61e2-213">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="e61e2-213">Added</span></span>|  
|<span data-ttu-id="e61e2-214">FiscalYearStartDate@1054 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-214">FiscalYearStartDate@1054 : Date;</span></span>|<span data-ttu-id="e61e2-215">FiscalYearStartDate@1011 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-215">FiscalYearStartDate@1011 : Date;</span></span>|<span data-ttu-id="e61e2-216">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-216">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-217">NextEntryNo@1055 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-217">NextEntryNo@1055 : Integer;</span></span>|<span data-ttu-id="e61e2-218">NextEntryNo@1022 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-218">NextEntryNo@1022 : Integer;</span></span>|<span data-ttu-id="e61e2-219">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-219">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-220">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-220">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="e61e2-221">BalanceCheckAmount@1056 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-221">BalanceCheckAmount@1056 : Decimal;</span></span>|<span data-ttu-id="e61e2-222">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-222">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-223">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-223">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="e61e2-224">BalanceCheckAmount2@1057 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-224">BalanceCheckAmount2@1057 : Decimal;</span></span>|<span data-ttu-id="e61e2-225">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-225">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-226">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="e61e2-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-227">BalanceCheckAddCurrAmount@1058 : Decimal;</span></span>|<span data-ttu-id="e61e2-228">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-228">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-229">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="e61e2-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-230">BalanceCheckAddCurrAmount2@1059 : Decimal;</span></span>|<span data-ttu-id="e61e2-231">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-231">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-232">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-232">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="e61e2-233">CurrentBalance@1060 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-233">CurrentBalance@1060 : Decimal;</span></span>|<span data-ttu-id="e61e2-234">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-234">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-235">SalesTaxBaseAmount@1061 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-235">SalesTaxBaseAmount@1061 : Decimal;</span></span>||<span data-ttu-id="e61e2-236">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-236">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-237">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-237">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="e61e2-238">TotalAddCurrAmount@1062 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-238">TotalAddCurrAmount@1062 : Decimal;</span></span>|<span data-ttu-id="e61e2-239">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-239">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-240">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-240">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="e61e2-241">TotalAmount@1063 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-241">TotalAmount@1063 : Decimal;</span></span>|<span data-ttu-id="e61e2-242">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-242">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-243">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="e61e2-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-244">UnrealizedRemainingAmountCust@1086 : Decimal;</span></span>|<span data-ttu-id="e61e2-245">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-245">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-246">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="e61e2-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-247">UnrealizedRemainingAmountVend@1074 : Decimal;</span></span>|<span data-ttu-id="e61e2-248">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-248">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-249">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-249">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="e61e2-250">NextVATEntryNo@1064 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-250">NextVATEntryNo@1064 : Integer;</span></span>|<span data-ttu-id="e61e2-251">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-251">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-252">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-252">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="e61e2-253">FirstNewVATEntryNo@1065 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-253">FirstNewVATEntryNo@1065 : Integer;</span></span>|<span data-ttu-id="e61e2-254">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-254">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-255">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-255">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="e61e2-256">NextTransactionNo@1066 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-256">NextTransactionNo@1066 : Integer;</span></span>|<span data-ttu-id="e61e2-257">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-257">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-258">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-258">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="e61e2-259">NextConnectionNo@1067 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-259">NextConnectionNo@1067 : Integer;</span></span>|<span data-ttu-id="e61e2-260">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-260">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-261">InsertedTempGLEntryVAT@1068 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-261">InsertedTempGLEntryVAT@1068 : Integer;</span></span>|<span data-ttu-id="e61e2-262">InsertedTempGLEntryVAT@1027 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-262">InsertedTempGLEntryVAT@1027 : Integer;</span></span>|<span data-ttu-id="e61e2-263">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-263">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-264">LastDocNo@1069 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="e61e2-264">LastDocNo@1069 : Code[20];</span></span>|<span data-ttu-id="e61e2-265">LastDocNo@1023 : Code[20];</span><span class="sxs-lookup"><span data-stu-id="e61e2-265">LastDocNo@1023 : Code[20];</span></span>|<span data-ttu-id="e61e2-266">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-266">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-267">LastLineNo@1070 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-267">LastLineNo@1070 : Integer;</span></span>||<span data-ttu-id="e61e2-268">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="e61e2-268">Deleted</span></span>|  
|<span data-ttu-id="e61e2-269">LastDate@1071 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-269">LastDate@1071 : Date;</span></span>|<span data-ttu-id="e61e2-270">LastDate@1021 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-270">LastDate@1021 : Date;</span></span>|<span data-ttu-id="e61e2-271">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-271">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="e61e2-272">LastDocType@1072 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="e61e2-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span><span class="sxs-lookup"><span data-stu-id="e61e2-273">LastDocType@1025 : ' ,Payment,Invoice,Credit Memo,Finance Charge Memo,Reminder';</span></span>|<span data-ttu-id="e61e2-274">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-274">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-275">NextCheckEntryNo@1073 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-275">NextCheckEntryNo@1073 : Integer;</span></span>|<span data-ttu-id="e61e2-276">NextCheckEntryNo@1028 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-276">NextCheckEntryNo@1028 : Integer;</span></span>|<span data-ttu-id="e61e2-277">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-277">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-278">AddCurrGLEntryVATAmt@1075 : Decimal;</span></span>|<span data-ttu-id="e61e2-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-279">AddCurrGLEntryVATAmt@1017 : Decimal;</span></span>|<span data-ttu-id="e61e2-280">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-280">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-281">CurrencyDate@1076 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-281">CurrencyDate@1076 : Date;</span></span>|<span data-ttu-id="e61e2-282">CurrencyDate@1020 : Date;</span><span class="sxs-lookup"><span data-stu-id="e61e2-282">CurrencyDate@1020 : Date;</span></span>|<span data-ttu-id="e61e2-283">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-283">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-284">CurrencyFactor@1077 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-284">CurrencyFactor@1077 : Decimal;</span></span>|<span data-ttu-id="e61e2-285">CurrencyFactor@1019 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-285">CurrencyFactor@1019 : Decimal;</span></span>|<span data-ttu-id="e61e2-286">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-286">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-287">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-287">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="e61e2-288">UseCurrFactorOnly@1078 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-288">UseCurrFactorOnly@1078 : Boolean;</span></span>|<span data-ttu-id="e61e2-289">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-289">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-290">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-290">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="e61e2-291">NonAddCurrCodeOccured@1079 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-291">NonAddCurrCodeOccured@1079 : Boolean;</span></span>|<span data-ttu-id="e61e2-292">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-292">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-293">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-293">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="e61e2-294">FADimAlreadyChecked@1080 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-294">FADimAlreadyChecked@1080 : Boolean;</span></span>|<span data-ttu-id="e61e2-295">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-295">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-296">AllApplied@1081 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-296">AllApplied@1081 : Boolean;</span></span>||<span data-ttu-id="e61e2-297">Gewijzigd naar lokaal</span><span class="sxs-lookup"><span data-stu-id="e61e2-297">Changed to Local</span></span>|  
|<span data-ttu-id="e61e2-298">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-298">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="e61e2-299">OverrideDimErr@1018 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-299">OverrideDimErr@1018 : Boolean;</span></span>|<span data-ttu-id="e61e2-300">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-300">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-301">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-301">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="e61e2-302">JobLine@1036 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-302">JobLine@1036 : Boolean;</span></span>|<span data-ttu-id="e61e2-303">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-303">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-304">Prepayment@1037 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-304">Prepayment@1037 : Boolean;</span></span>||<span data-ttu-id="e61e2-305">Verwijderd</span><span class="sxs-lookup"><span data-stu-id="e61e2-305">Deleted</span></span>|  
|<span data-ttu-id="e61e2-306">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-306">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="e61e2-307">CheckUnrealizedCust@1082 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-307">CheckUnrealizedCust@1082 : Boolean;</span></span>|<span data-ttu-id="e61e2-308">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-308">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-309">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-309">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="e61e2-310">CheckUnrealizedVend@1083 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-310">CheckUnrealizedVend@1083 : Boolean;</span></span>|<span data-ttu-id="e61e2-311">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-311">Unchanged</span></span>|  
|<span data-ttu-id="e61e2-312">GLEntryNo@1090 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-312">GLEntryNo@1090 : Integer;</span></span>|<span data-ttu-id="e61e2-313">GLEntryNo@1026 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-313">GLEntryNo@1026 : Integer;</span></span>|<span data-ttu-id="e61e2-314">Ongewijzigd</span><span class="sxs-lookup"><span data-stu-id="e61e2-314">Unchanged</span></span>|  
||<span data-ttu-id="e61e2-315">GLSetupRead@1015 : Boolean;</span><span class="sxs-lookup"><span data-stu-id="e61e2-315">GLSetupRead@1015 : Boolean;</span></span>|<span data-ttu-id="e61e2-316">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="e61e2-316">Added</span></span>|  
||<span data-ttu-id="e61e2-317">AmountRoundingPrecision@1012 : Decimal;</span><span class="sxs-lookup"><span data-stu-id="e61e2-317">AmountRoundingPrecision@1012 : Decimal;</span></span>|<span data-ttu-id="e61e2-318">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="e61e2-318">Added</span></span>|  
||<span data-ttu-id="e61e2-319">CrCardTransactionEntryNo@1013 : Integer;</span><span class="sxs-lookup"><span data-stu-id="e61e2-319">CrCardTransactionEntryNo@1013 : Integer;</span></span>|<span data-ttu-id="e61e2-320">Toegevoegd</span><span class="sxs-lookup"><span data-stu-id="e61e2-320">Added</span></span>|  

## <a name="see-also"></a><span data-ttu-id="e61e2-321">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e61e2-321">See Also</span></span>  
 [<span data-ttu-id="e61e2-322">Designdetails: Wijzigingen in codeunit 12: Wijzigingen in procedures voor grootboekboekingen</span><span class="sxs-lookup"><span data-stu-id="e61e2-322">Design Details: Codeunit 12 Changes: Changes in General Journal Post Procedures</span></span>](design-details-codeunit-12-changes-changes-in-general-journal-post-procedures.md)