---
title: "Bankafschriften importeren en reconciliëren"
description: "Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren."
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
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: d5e785cb349d1eb73eeecabf961c94a5e2b0f9c8
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="import-and-reconcile-bank-statements"></a><span data-ttu-id="cc012-104">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="cc012-104">Import and Reconcile Bank Statements</span></span>
<span data-ttu-id="cc012-105">Banken bieden elektronische bankafschriften voor al uw financiële interacties.</span><span class="sxs-lookup"><span data-stu-id="cc012-105">Banks provide electronic bank statements for all your financial interactions.</span></span> <span data-ttu-id="cc012-106">U kunt deze afschriften in het bank- of giroboek importeren.</span><span class="sxs-lookup"><span data-stu-id="cc012-106">You can import these statements into the bank or giro journals.</span></span>  

<span data-ttu-id="cc012-107">Het importbankafschrift wordt ondersteund door de volgende protocollen:</span><span class="sxs-lookup"><span data-stu-id="cc012-107">The import bank statement is supported by the following protocols:</span></span>  

- <span data-ttu-id="cc012-108">Rabobank mut.asc</span><span class="sxs-lookup"><span data-stu-id="cc012-108">Rabobank mut.asc</span></span>  
- <span data-ttu-id="cc012-109">Rabobank vvmut.ac</span><span class="sxs-lookup"><span data-stu-id="cc012-109">Rabobank vvmut.ac</span></span>  
- <span data-ttu-id="cc012-110">Rabobank ASCII</span><span class="sxs-lookup"><span data-stu-id="cc012-110">Rabobank ASCII</span></span>  
- <span data-ttu-id="cc012-111">SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="cc012-111">SEPA CAMT</span></span>  

## <a name="to-import-and-reconcile-bank-statements"></a><span data-ttu-id="cc012-112">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="cc012-112">To import and reconcile bank statements</span></span>  

1.  <span data-ttu-id="cc012-113">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bankafschrift importeren** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="cc012-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Import Bank Statement**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="cc012-114">Selecteer in het venster **Importprotocoloverzicht** het vereiste importprotocol en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="cc012-114">In the **Import Protocol List** window, select the required import protocol, and then choose the **OK** button.</span></span>  
3.  <span data-ttu-id="cc012-115">Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.</span><span class="sxs-lookup"><span data-stu-id="cc012-115">To reconcile the bank statements automatically when importing, on the **Options** FastTab, select the **Automatic Reconciliation** check box.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="cc012-116">Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT.</span><span class="sxs-lookup"><span data-stu-id="cc012-116">This function does not work for bank statement files of type SEPA CAMT.</span></span> <span data-ttu-id="cc012-117">Gebruik in plaats daarvan de actie **Automatisch afstemmen** in het venster **Bankreconciliatie**.</span><span class="sxs-lookup"><span data-stu-id="cc012-117">Instead, use the **Match Automatically** action in the **Bank Acc. Reconciliation** window.</span></span> <span data-ttu-id="cc012-118">Zie voor meer informatie [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="cc012-118">For more information, see [Applying Payments Automatically and Reconcile Bank Accounts](../../receivables-apply-payments-auto-reconcile-bank-accounts.md).</span></span>  

4.  <span data-ttu-id="cc012-119">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="cc012-119">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="cc012-120">Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="cc012-120">To import the file that contains the electronic bank statement, specify the file name and path, and then choose the **Open** button.</span></span>  

<span data-ttu-id="cc012-121">Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek.</span><span class="sxs-lookup"><span data-stu-id="cc012-121">The electronic bank statement is imported into the bank or giro journals.</span></span> <span data-ttu-id="cc012-122">Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).</span><span class="sxs-lookup"><span data-stu-id="cc012-122">For more information, see [Dutch Electronic Banking](dutch-electronic-banking.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="cc012-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="cc012-123">See Also</span></span>  
 <span data-ttu-id="cc012-124">[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="cc012-124">[Dutch Electronic Banking](dutch-electronic-banking.md) </span></span>  
 [<span data-ttu-id="cc012-125">Betalingen automatisch vereffenen en bankrekeningen reconciliëren</span><span class="sxs-lookup"><span data-stu-id="cc012-125">Applying Payments Automatically and Reconcile Bank Accounts</span></span>](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)

