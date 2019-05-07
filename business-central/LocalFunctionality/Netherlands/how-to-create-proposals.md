---
title: Voorstellen maken
description: Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.
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
ms.openlocfilehash: 06a11f484f813b0f889982ed4f4511891c0d2542
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2019
ms.locfileid: "932713"
---
# <a name="create-proposals"></a><span data-ttu-id="52e41-103">Voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="52e41-103">Create Proposals</span></span>
<span data-ttu-id="52e41-104">Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.</span><span class="sxs-lookup"><span data-stu-id="52e41-104">Proposals can be generated manually or automatically based on either vendor or customer ledger entries.</span></span>  

> [!IMPORTANT]  
>  <span data-ttu-id="52e41-105">Als u een voorstel maakt, moet u het veld **Rekeninghouder** op de pagina's Bankrekening leverancier en Bankrekening klant gebruiken.</span><span class="sxs-lookup"><span data-stu-id="52e41-105">To create a proposal, you must use the **Owner Information** field in the Vendor Bank Account Card and Customer Bank Account Card pages.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="52e41-106">U kunt op elk moment en op elk niveau, voorafgaand aan de verwerking van een voorstel, de transactiewijze en bankrekening wijzigen.</span><span class="sxs-lookup"><span data-stu-id="52e41-106">At any time and at any level, before processing a proposal, the transaction mode and bank account can be modified.</span></span> <span data-ttu-id="52e41-107">Op het laagste niveau in de desbetreffende leveranciers- of klantenposten.</span><span class="sxs-lookup"><span data-stu-id="52e41-107">At the lowest level on the relevant vendor or customer ledger entries.</span></span>  

## <a name="to-create-proposals-manually"></a><span data-ttu-id="52e41-108">Handmatig voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="52e41-108">To create proposals manually</span></span>  

1.  <span data-ttu-id="52e41-109">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="52e41-109">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="52e41-110">Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="52e41-110">Select the relevant bank account and then choose the **Proposal** action.</span></span>  
3.  <span data-ttu-id="52e41-111">U moet minimaal de velden **Rekeningsoort**, **Rekeningnr.**, **Transactiewijze**, **Bankrekeningnr.** en **Bedrag** invullen.</span><span class="sxs-lookup"><span data-stu-id="52e41-111">At a minimum, you must fill in the **Account Type**, **Account No.**, **Transaction Mode**, **Bank Account No.**, and **Amount** fields.</span></span>  

4.  <span data-ttu-id="52e41-112">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="52e41-112">If you want to view or adjust the proposal's detail lines, choose the **Detail Information** action.</span></span> <span data-ttu-id="52e41-113">U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.</span><span class="sxs-lookup"><span data-stu-id="52e41-113">To return to the proposal, close the **Proposal Detail Line** page.</span></span>  

## <a name="to-create-proposals-automatically-from-sales"></a><span data-ttu-id="52e41-114">Automatisch voorstellen maken op basis van verkoop</span><span class="sxs-lookup"><span data-stu-id="52e41-114">To create proposals automatically from sales</span></span>  

1. <span data-ttu-id="52e41-115">Stel voor de klant die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="52e41-115">Set up a card for the customer who sent the invoice with appropriate values for the **Currency Code**, **Transaction Mode**, and **Bank Account** fields.</span></span>
2. <span data-ttu-id="52e41-116">Maak een verkoopfactuur of creditnota, vul de klant en relevante items in en boek de factuur.</span><span class="sxs-lookup"><span data-stu-id="52e41-116">Create a sales invoice or credit memo, enter the customer and relevant items and post the invoice.</span></span>
3. <span data-ttu-id="52e41-117">Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten.</span><span class="sxs-lookup"><span data-stu-id="52e41-117">Check whether the **Currency Code**, **Transaction Mode**, and **Bank Account** fields of the invoice/credit memo contain appropriate values.</span></span> <span data-ttu-id="52e41-118">Standaard worden deze gekopieerd vanuit de klantenkaart.</span><span class="sxs-lookup"><span data-stu-id="52e41-118">By default, they will be copied from the customer card.</span></span>  

4.  <span data-ttu-id="52e41-119">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="52e41-119">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
5.  <span data-ttu-id="52e41-120">Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="52e41-120">Select the relevant bank account, and then choose the **Proposal** action.</span></span>  
6.  <span data-ttu-id="52e41-121">Kies de actie **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="52e41-121">Choose the **Get Entries** action.</span></span>  

    <span data-ttu-id="52e41-122">U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante klantenposten.</span><span class="sxs-lookup"><span data-stu-id="52e41-122">You can use the Get Proposal Entries Batch Job batch job to generate proposal lines based on relevant customer ledger entries.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="52e41-123">Alleen voor posten die een transactiewijze van het rekeningsoort **Klant** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.</span><span class="sxs-lookup"><span data-stu-id="52e41-123">Only proposal lines will be created for ledger entries that have a transaction mode of account type **Customer** and a link to the active bank account.</span></span>  

6.  <span data-ttu-id="52e41-124">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="52e41-124">If you want to view or adjust the proposal's detail lines, choose the **Detail Information** action.</span></span> <span data-ttu-id="52e41-125">U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.</span><span class="sxs-lookup"><span data-stu-id="52e41-125">To return to the proposal, close the **Proposal Detail Line** page.</span></span>  

## <a name="to-create-proposals-automatically-from-purchases"></a><span data-ttu-id="52e41-126">Automatisch voorstellen maken op basis van inkoop</span><span class="sxs-lookup"><span data-stu-id="52e41-126">To create proposals automatically from purchases</span></span>  

1.  <span data-ttu-id="52e41-127">Stel voor de leverancier die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.</span><span class="sxs-lookup"><span data-stu-id="52e41-127">Set up a card for the vendor that sent the invoice with appropriate values for **Currency Code**, **Transaction Mode**, and **Bank Account** fields.</span></span>  
2.  <span data-ttu-id="52e41-128">Maak een inkoopfactuur of creditnota en voer de leverancier en relevante items in.</span><span class="sxs-lookup"><span data-stu-id="52e41-128">Create a purchase invoice or credit memo, enter the vendor and relevant items.</span></span>
3. <span data-ttu-id="52e41-129">Boek de factuur.</span><span class="sxs-lookup"><span data-stu-id="52e41-129">Post the invoice.</span></span>
4. <span data-ttu-id="52e41-130">Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten.</span><span class="sxs-lookup"><span data-stu-id="52e41-130">Check whether the **Currency Code**, **Transaction Mode**, and **Bank Account** fields of the invoice/credit memo contain appropriate values.</span></span> <span data-ttu-id="52e41-131">Standaard worden deze gekopieerd vanuit de leverancierskaart.</span><span class="sxs-lookup"><span data-stu-id="52e41-131">By default, they will be copied from the vendor card.</span></span>  
5.  <span data-ttu-id="52e41-132">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="52e41-132">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  
6.  <span data-ttu-id="52e41-133">Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="52e41-133">Select the relevant bank account, and then choose the **Proposal** action.</span></span>  
7.  <span data-ttu-id="52e41-134">Kies de actie **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="52e41-134">Choose the **Get Entries** action.</span></span>  

    <span data-ttu-id="52e41-135">U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante leveranciersposten.</span><span class="sxs-lookup"><span data-stu-id="52e41-135">You can use the Get Proposal Entries Batch Job batch job to generate proposal lines based on relevant vendor ledger entries.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="52e41-136">Alleen voor posten die een transactiewijze van het rekeningsoort **Leverancier** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.</span><span class="sxs-lookup"><span data-stu-id="52e41-136">Only proposal lines will be created for ledger entries that have a transaction mode of account type **Vendor** and a link to the active bank account.</span></span>  

6.  <span data-ttu-id="52e41-137">Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**.</span><span class="sxs-lookup"><span data-stu-id="52e41-137">If you want to view or adjust the proposal's detail lines, choose the **Detail Information** action.</span></span> <span data-ttu-id="52e41-138">U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.</span><span class="sxs-lookup"><span data-stu-id="52e41-138">To return to the proposal, close the **Proposal Detail Line** page.</span></span>  

## <a name="see-also"></a><span data-ttu-id="52e41-139">Zie ook</span><span class="sxs-lookup"><span data-stu-id="52e41-139">See Also</span></span>  
 <span data-ttu-id="52e41-140">[Nieuwe klanten registreren](../../sales-how-register-new-customers.md) </span><span class="sxs-lookup"><span data-stu-id="52e41-140">[Register New Customers](../../sales-how-register-new-customers.md) </span></span>  
 <span data-ttu-id="52e41-141">[Verkopen factureren](../../sales-how-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="52e41-141">[Invoice Sales](../../sales-how-invoice-sales.md) </span></span>  
 <span data-ttu-id="52e41-142">[Inkopen vastleggen](../../purchasing-how-record-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="52e41-142">[Record Purchases](../../purchasing-how-record-purchases.md) </span></span>  
 [<span data-ttu-id="52e41-143">Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="52e41-143">Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)
