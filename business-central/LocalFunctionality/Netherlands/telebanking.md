---
title: Telebankieren
description: Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7b6adaeb184b7dee4cfe2c698011e91facac4783
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780110"
---
# <a name="telebanking"></a><span data-ttu-id="d4f8f-103">Telebankieren</span><span class="sxs-lookup"><span data-stu-id="d4f8f-103">Telebanking</span></span>
<span data-ttu-id="d4f8f-104">Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-104">Based on both sales and purchase transactions, telebanking enables you to generate your payments and collections and interchange them with your bank electronically.</span></span> <span data-ttu-id="d4f8f-105">Hieronder vallen ook de export van betalings- en incassogegevens die naar de bank moeten worden doorgestuurd en de import van bankafschriften die door de bank naar u worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-105">This includes the export of payment and collection data that need to be forwarded to the bank as well as the import of bank statements sent to you by the bank.</span></span>  

## <a name="transactions"></a><span data-ttu-id="d4f8f-106">Transacties</span><span class="sxs-lookup"><span data-stu-id="d4f8f-106">Transactions</span></span>  
<span data-ttu-id="d4f8f-107">Over het algemeen worden alle financiële interacties met leveranciers en klanten uitgevoerd door middel van inkoop- of verkoopfacturen en creditnota's.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-107">In general, all financial interactions with vendors and customers are done through either purchase or sales invoices and credit memos.</span></span> <span data-ttu-id="d4f8f-108">Zodra deze transacties zijn geregistreerd en geboekt, kunnen betalingen of incasso's door uw bedrijf worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-108">As soon as these transactions have been registered and posted, payments or collections can be carried out by your company.</span></span>  

## <a name="proposals"></a><span data-ttu-id="d4f8f-109">Voorstellen</span><span class="sxs-lookup"><span data-stu-id="d4f8f-109">Proposals</span></span>  
<span data-ttu-id="d4f8f-110">Op basis van leveranciers- en klantenposten kunt u met telebankieren betalings- en incassovoorstellen genereren.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-110">Based on vendor and customer ledger entries, telebanking enables you to generate payment and collection proposals.</span></span> <span data-ttu-id="d4f8f-111">Dit kan voor elke bank worden gedaan die voor uw bedrijf is ingesteld.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-111">This can be done for any bank that has been set up for your company.</span></span> <span data-ttu-id="d4f8f-112">Zowel binnen- als buitenlandse betalingen en incasso's zijn mogelijk.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-112">Both domestic and foreign payments and collections are possible.</span></span>  

<span data-ttu-id="d4f8f-113">U kunt [!INCLUDE[prod_short](../../includes/prod_short.md)] zodanig instellen dat betalingen aan of incasso's van dezelfde bankrekening automatisch worden gecombineerd.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-113">You can set up [!INCLUDE[prod_short](../../includes/prod_short.md)] to combine payments to or collections from the same bank account automatically.</span></span>  

<span data-ttu-id="d4f8f-114">Als u akkoord gaat met het voorstel, moet het in een betaalrun worden verwerkt.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-114">When a proposal has been agreed upon, it should be processed into a payment history.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="d4f8f-115">Over het algemeen kan voor alle openstaande leveranciers- en klantenposten een voorstel worden gegenereerd als dat aan een aantal criteria voldoet.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-115">In general, for any open vendor and customer ledger entries, a proposal can be generated if it meets a number of criteria.</span></span> <span data-ttu-id="d4f8f-116">Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-116">For more information, see [Create Proposals](how-to-create-proposals.md).</span></span>  

## <a name="payment-histories"></a><span data-ttu-id="d4f8f-117">Betaalruns</span><span class="sxs-lookup"><span data-stu-id="d4f8f-117">Payment Histories</span></span>  
<span data-ttu-id="d4f8f-118">Een betaalrun is eigenlijk precies hetzelfde als een voorstel, het enige verschil is dat gegevens in een betaalrun niet kunnen worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-118">A payment history is nothing more than a proposal except for the fact that data on a payment history cannot be modified.</span></span> <span data-ttu-id="d4f8f-119">De betalings- of incassogegevens zijn gereed om naar de bank te worden geëxporteerd en verzonden.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-119">The payment or collection data is ready to be exported and forwarded to the bank.</span></span>  

 <span data-ttu-id="d4f8f-120">Zie voor meer informatie [Betaalrun maken en exporteren](how-to-create-and-export-payment-history.md).</span><span class="sxs-lookup"><span data-stu-id="d4f8f-120">For more information, see [Create and Export Payment History](how-to-create-and-export-payment-history.md).</span></span>  

## <a name="bank-statements"></a><span data-ttu-id="d4f8f-121">Bankafschriften</span><span class="sxs-lookup"><span data-stu-id="d4f8f-121">Bank Statements</span></span>  
 <span data-ttu-id="d4f8f-122">Voor alle financiële interacties die via uw bank plaatsvinden, kan de bank u elektronische bankafschriften toesturen.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-122">For all your financial interactions through your bank, the bank can send you electronic bank statements.</span></span> <span data-ttu-id="d4f8f-123">Deze afschriften kunnen in de Bank-/Giroboeken worden geïmporteerd.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-123">These statements can be imported into the Bank/Giro Journals.</span></span> <span data-ttu-id="d4f8f-124">Als u wilt kunt u [!INCLUDE[prod_short](../../includes/prod_short.md)] deze afschriften tijdens het importproces automatisch laten reconciliëren en kan worden vastgesteld of een afschrift kan worden vereffend met openstaande posten voor de betreffende leverancier/klant.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-124">If you want, you can have [!INCLUDE[prod_short](../../includes/prod_short.md)] automatically reconcile these statements during this import process and determine whether a statement can be applied to open ledger entries for the relevant vendor/customer.</span></span>  

 <span data-ttu-id="d4f8f-125">Zie [Bankafschriften importeren en reconciliëren](how-to-import-and-reconcile-bank-statements.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-125">For more information, see [Import and Reconcile Bank Statements](how-to-import-and-reconcile-bank-statements.md).</span></span>  
 
 > [!NOTE]  
>  <span data-ttu-id="d4f8f-126">De valuta van de geïmporteerde transacties moet overeenkomen met de valuta die is opgegeven op de bankrekening in [!INCLUDE[prod_short](../../includes/prod_short.md)].</span><span class="sxs-lookup"><span data-stu-id="d4f8f-126">The currency of the imported transactions must match the currency that is specified on the bank account in [!INCLUDE[prod_short](../../includes/prod_short.md)].</span></span>  

## <a name="exchange-protocols"></a><span data-ttu-id="d4f8f-127">Uitwisselingsprotocollen</span><span class="sxs-lookup"><span data-stu-id="d4f8f-127">Exchange Protocols</span></span>  
 <span data-ttu-id="d4f8f-128">Voor zowel het exporteren als importeren is een aantal protocollen gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-128">For both exporting and importing, a number of protocols have been defined.</span></span> [!INCLUDE[prod_short](../../includes/prod_short.md)] <span data-ttu-id="d4f8f-129">ondersteunt de volgende protocollen:</span><span class="sxs-lookup"><span data-stu-id="d4f8f-129">supports the following protocols:</span></span>  

- <span data-ttu-id="d4f8f-130">BTL91 (export).</span><span class="sxs-lookup"><span data-stu-id="d4f8f-130">BTL91 (export).</span></span> <span data-ttu-id="d4f8f-131">Dit grensoverschrijdende protocol wordt niet langer geaccepteerd in Nederland vanaf 1 mei 2019.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-131">This cross-border protocol is no longer accepted in the Netherlands as of May 1st 2019.</span></span> <span data-ttu-id="d4f8f-132">Dit protocol wordt vervangen door het Algemeen betalingsbestand-protocol.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-132">This protocol is replaced by the Generic Payment File protocol.</span></span>
- <span data-ttu-id="d4f8f-133">BBV (exporteren)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-133">BBV (export)</span></span>  
- <span data-ttu-id="d4f8f-134">PAYMUL (exporteren)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-134">PAYMUL (export)</span></span>  
- <span data-ttu-id="d4f8f-135">Algemeen betalingsbestand (export).</span><span class="sxs-lookup"><span data-stu-id="d4f8f-135">Generic Payment File (export).</span></span> <span data-ttu-id="d4f8f-136">Kan worden gebruikt voor grensoverschrijdende overdrachten buiten de EU.</span><span class="sxs-lookup"><span data-stu-id="d4f8f-136">Can be used for cross-border Non-EUR transfers.</span></span>
- <span data-ttu-id="d4f8f-137">Rabobank mut.asc (importeren)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-137">Rabobank mut.asc (import)</span></span>  
- <span data-ttu-id="d4f8f-138">Rabobank vvmut.asc (importeren)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-138">Rabobank vvmut.asc (import)</span></span>  
- <span data-ttu-id="d4f8f-139">Rabobank ASCII (importeren)</span><span class="sxs-lookup"><span data-stu-id="d4f8f-139">Rabobank ASCII (import)</span></span>  
- <span data-ttu-id="d4f8f-140">SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="d4f8f-140">SEPA CAMT</span></span>  

## <a name="see-also"></a><span data-ttu-id="d4f8f-141">Zie ook</span><span class="sxs-lookup"><span data-stu-id="d4f8f-141">See Also</span></span>  
 <span data-ttu-id="d4f8f-142">[Verkopen factureren](../../sales-how-invoice-sales.md) </span><span class="sxs-lookup"><span data-stu-id="d4f8f-142">[Invoice Sales](../../sales-how-invoice-sales.md) </span></span>  
 <span data-ttu-id="d4f8f-143">[Inkopen vastleggen](../../purchasing-how-record-purchases.md) </span><span class="sxs-lookup"><span data-stu-id="d4f8f-143">[Record Purchases](../../purchasing-how-record-purchases.md) </span></span>  
 <span data-ttu-id="d4f8f-144">[Voorstellen maken.](how-to-create-proposals.md) </span><span class="sxs-lookup"><span data-stu-id="d4f8f-144">[Create Proposals](how-to-create-proposals.md) </span></span>  
 [<span data-ttu-id="d4f8f-145">Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="d4f8f-145">Create and Export Payment History</span></span>](how-to-create-and-export-payment-history.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]