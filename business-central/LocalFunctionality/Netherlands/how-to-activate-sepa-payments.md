---
title: SEPA-betalingen activeren
description: Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen.
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: ae496d22944590308e24c3c3437182f5777cfa3e
ms.sourcegitcommit: 007b331b6974983ee614db0406f00777da359ecb
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/10/2020
ms.locfileid: "3677210"
---
# <a name="activate-sepa-payments"></a><span data-ttu-id="41cbd-103">SEPA-betalingen activeren</span><span class="sxs-lookup"><span data-stu-id="41cbd-103">Activate SEPA Payments</span></span>
<span data-ttu-id="41cbd-104">Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen.</span><span class="sxs-lookup"><span data-stu-id="41cbd-104">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments.</span></span>  

<span data-ttu-id="41cbd-105">In de volgende procedures beschrijven de eerste vier hoe u SEPA-betalingen activeert. De twee overige procedures hebben betrekking op de afzonderlijke leveranciers.</span><span class="sxs-lookup"><span data-stu-id="41cbd-105">In the following procedures, the first four describe how to enable SEPA payments, and the remaining two relate to the individual vendors.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="41cbd-106">Landen/regio's activeren voor SEPA</span><span class="sxs-lookup"><span data-stu-id="41cbd-106">To enable countries/regions for SEPA</span></span>  

1.  <span data-ttu-id="41cbd-107">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Landen/regio's** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-107">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-108">Kies de actie **Lijst bewerken**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-108">Choose the **Edit List** action.</span></span>  
3.  <span data-ttu-id="41cbd-109">Schakel het selectievakje **SEPA toegestaan** in voor elk land/regio dat u wilt activeren voor SEPA.</span><span class="sxs-lookup"><span data-stu-id="41cbd-109">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4.  <span data-ttu-id="41cbd-110">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-110">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="41cbd-111">Bankrekeningen activeren voor SEPA</span><span class="sxs-lookup"><span data-stu-id="41cbd-111">To enable bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="41cbd-112">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-113">Selecteer de bankrekening die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-113">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="41cbd-114">Selecteer in het veld **Land-/regiocode** van het sneltabblad **Algemeen** de gewenste code.</span><span class="sxs-lookup"><span data-stu-id="41cbd-114">On the **General** FastTab, in the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="41cbd-115">De opgegeven land-/regiocode moet zijn geactiveerd voor SEPA, zoals is beschreven in de vorige procedure.</span><span class="sxs-lookup"><span data-stu-id="41cbd-115">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4.  <span data-ttu-id="41cbd-116">Geef een waarde op in het veld **Minimumsaldo**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-116">Enter a value in the **Min. Balance** field.</span></span>  
5.  <span data-ttu-id="41cbd-117">Geef in het veld **SWIFT-code** van het sneltabblad **Transfer** een code op.</span><span class="sxs-lookup"><span data-stu-id="41cbd-117">On the **Transfer** FastTab, in the **SWIFT Code** field, enter a code.</span></span>  
6.  <span data-ttu-id="41cbd-118">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-118">Choose the **OK** button.</span></span>  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a><span data-ttu-id="41cbd-119">Een SEPA ISO 20022-exportprotocol instellen</span><span class="sxs-lookup"><span data-stu-id="41cbd-119">To set up a SEPA ISO 20022 export protocol</span></span>  

1.  <span data-ttu-id="41cbd-120">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Exportprotocollen** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-120">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Export Protocols**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-121">Kies op de pagina **Exportprotocollen** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-121">On the **Export Protocols** page, choose the **New** action.</span></span>  
3.  <span data-ttu-id="41cbd-122">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="41cbd-122">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="41cbd-123">Veld</span><span class="sxs-lookup"><span data-stu-id="41cbd-123">Field</span></span>|<span data-ttu-id="41cbd-124">Description</span><span class="sxs-lookup"><span data-stu-id="41cbd-124">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="41cbd-125">**Code**</span><span class="sxs-lookup"><span data-stu-id="41cbd-125">**Code**</span></span>|<span data-ttu-id="41cbd-126">Hier stelt u de exportprotocolcode in, zoals **SEPA ISO20022**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-126">Sets the export protocol code, such as **SEPA ISO20022**.</span></span>|  
    |<span data-ttu-id="41cbd-127">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="41cbd-127">**Description**</span></span>|<span data-ttu-id="41cbd-128">Hier wordt een omschrijving weergegeven voor het exportprotocol.</span><span class="sxs-lookup"><span data-stu-id="41cbd-128">Provides the description for the export protocol.</span></span>|  
    |<span data-ttu-id="41cbd-129">**Controle-id**</span><span class="sxs-lookup"><span data-stu-id="41cbd-129">**Check ID**</span></span>|<span data-ttu-id="41cbd-130">Hier wordt de id ingesteld voor de code-unit om de betaling te controleren, bijvoorbeeld **11000010**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-130">Sets the ID for the codeunit to check payment, such as **11000010**.</span></span>|  
    |<span data-ttu-id="41cbd-131">**Controlenaam**</span><span class="sxs-lookup"><span data-stu-id="41cbd-131">**Check Name**</span></span>|<span data-ttu-id="41cbd-132">Hier wordt de naam van de code-unit ingesteld.</span><span class="sxs-lookup"><span data-stu-id="41cbd-132">Sets the name of the codeunit.</span></span>|  
    |<span data-ttu-id="41cbd-133">**Soort exportprotocol**</span><span class="sxs-lookup"><span data-stu-id="41cbd-133">**Export Protocol Type**</span></span>|<span data-ttu-id="41cbd-134">Hiermee wordt het soort exportprotocol opgegeven:</span><span class="sxs-lookup"><span data-stu-id="41cbd-134">Specifies the type of the export protocol:</span></span><br /><br /> <span data-ttu-id="41cbd-135">-   **Rapport**</span><span class="sxs-lookup"><span data-stu-id="41cbd-135">-   **Report**</span></span><br /><span data-ttu-id="41cbd-136">-   **XMLPort**</span><span class="sxs-lookup"><span data-stu-id="41cbd-136">-   **XMLPort**</span></span>|  
    |<span data-ttu-id="41cbd-137">**Export-id**</span><span class="sxs-lookup"><span data-stu-id="41cbd-137">**Export ID**</span></span>|<span data-ttu-id="41cbd-138">Hier wordt de id ingesteld voor de batchverwerking om betalingen te exporteren, bijvoorbeeld **11000011**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-138">Sets the ID for the batch job to export payment, such as **11000011**.</span></span><br /><br /> <span data-ttu-id="41cbd-139">Als u XMLPort als uw exportprotocolsoort selecteert, kiest u een id zoals **1000**</span><span class="sxs-lookup"><span data-stu-id="41cbd-139">If you select XMLPort as your export protocol type, then choose an ID such as **1000**.</span></span>|  
    |<span data-ttu-id="41cbd-140">**Exportnaam**</span><span class="sxs-lookup"><span data-stu-id="41cbd-140">**Export Name**</span></span>|<span data-ttu-id="41cbd-141">De naam van de batchverwerking.</span><span class="sxs-lookup"><span data-stu-id="41cbd-141">The name of the batch job.</span></span>|  
    |<span data-ttu-id="41cbd-142">**Borderel-id**</span><span class="sxs-lookup"><span data-stu-id="41cbd-142">**Docket ID**</span></span>|<span data-ttu-id="41cbd-143">Hier wordt de id ingesteld voor de batchverwerking om de contactpersoon op de hoogte te brengen van gecombineerde betalingen, zoals **11000004**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-143">Sets the ID for the batch job to inform the contact on combined payments, such as **11000004**.</span></span><br /><br /> <span data-ttu-id="41cbd-144">Dit is niet van toepassing op XMLPort-protocolsoorten.</span><span class="sxs-lookup"><span data-stu-id="41cbd-144">This does not apply to XMLPort protocol types.</span></span>|  
    |<span data-ttu-id="41cbd-145">**Borderelnaam**</span><span class="sxs-lookup"><span data-stu-id="41cbd-145">**Docket Name**</span></span>|<span data-ttu-id="41cbd-146">De naam van het borderelrapport.</span><span class="sxs-lookup"><span data-stu-id="41cbd-146">The name of the docket report.</span></span>|  
    |<span data-ttu-id="41cbd-147">**Standaardbestandsnamen**</span><span class="sxs-lookup"><span data-stu-id="41cbd-147">**Default File Names**</span></span>|<span data-ttu-id="41cbd-148">Hier wordt de locatie ingesteld voor het exporteren van betalings- en inningsgegevens.</span><span class="sxs-lookup"><span data-stu-id="41cbd-148">Sets the location to export payment and collection data.</span></span>|  

4.  <span data-ttu-id="41cbd-149">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-149">Choose the **OK** button.</span></span>  

## <a name="to-enable-transaction-modes-for-sepa"></a><span data-ttu-id="41cbd-150">Transactiewijzen activeren voor SEPA</span><span class="sxs-lookup"><span data-stu-id="41cbd-150">To enable transaction modes for SEPA</span></span>  

1.  <span data-ttu-id="41cbd-151">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transactiewijzen** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-151">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Transaction Modes**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-152">Selecteer de transactiewijze die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-152">Select the transaction mode that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3.  <span data-ttu-id="41cbd-153">Selecteer in het veld **Exportprotocol** op het sneltabblad **Betalingsvoorstel** van de pagina **Transactiewijzekaart** het SEPA-exportprotocol dat u hebt gemaakt, bijvoorbeeld **SEPA ISO20022**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-153">On the **Transaction Mode Card** page, on the **Paym. Proposal** FastTab, in the **Export Protocol** field, select the SEPA export protocol that you have created, such as **SEPA ISO20022**.</span></span>  
4.  <span data-ttu-id="41cbd-154">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-154">Choose the **OK** button.</span></span>  

## <a name="to-verify-vendor-payment-transaction-modes-for-sepa"></a><span data-ttu-id="41cbd-155">Transactiewijzen voor leveranciersbetalingen voor SEPA verifiëren</span><span class="sxs-lookup"><span data-stu-id="41cbd-155">To verify vendor payment transaction modes for SEPA</span></span>  

1.  <span data-ttu-id="41cbd-156">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-156">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-157">Selecteer de leverancier waarvoor u de transactiewijze wilt verifiëren en kies de actie **Weergave**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-157">Select the vendor that you want to verify the transaction mode for, and then choose the **View** action.</span></span>  
3.  <span data-ttu-id="41cbd-158">Controleer of de transactiewijze voor de leveranciersbetalingen in het veld **Code transactiewijze** van het sneltabblad **Betalingen** een transactiewijze is die is geactiveerd voor SEPA.</span><span class="sxs-lookup"><span data-stu-id="41cbd-158">On the **Payments** FastTab, in the **Transaction Mode Code** field, verify that the vendor payment transaction mode is one that has been enabled for SEPA.</span></span>  
4.  <span data-ttu-id="41cbd-159">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-159">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="41cbd-160">Bankrekeningen van leveranciers instellen voor SEPA</span><span class="sxs-lookup"><span data-stu-id="41cbd-160">To set up vendor bank accounts for SEPA</span></span>  

1.  <span data-ttu-id="41cbd-161">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="41cbd-161">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="41cbd-162">Selecteer de betreffende leverancier en kies vervolgens de actie **Bankrekeningen**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-162">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3.  <span data-ttu-id="41cbd-163">Selecteer de bankrekening van de leverancier die u wilt instellen voor SEPA, en kies vervolgens de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-163">Select the vendor bank account to set up for SEPA, and then choose the **Edit** action.</span></span>  
4.  <span data-ttu-id="41cbd-164">Geef in de velden **IBAN** en **SWIFT-code** van het sneltabblad **Transfer** de internationale bankidentificatiecode op van de bank waarbij de leverancier de rekening heeft.</span><span class="sxs-lookup"><span data-stu-id="41cbd-164">On the **Transfer** FastTab, in the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5.  <span data-ttu-id="41cbd-165">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="41cbd-165">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="41cbd-166">Zie ook</span><span class="sxs-lookup"><span data-stu-id="41cbd-166">See Also</span></span>  
 <span data-ttu-id="41cbd-167">[Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md) </span><span class="sxs-lookup"><span data-stu-id="41cbd-167">[Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md) </span></span>  
 [<span data-ttu-id="41cbd-168">Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling</span><span class="sxs-lookup"><span data-stu-id="41cbd-168">Submit Vendor Payments Electronically in SEPA ISO 20022 Payment Format</span></span>](how-to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format.md) 
