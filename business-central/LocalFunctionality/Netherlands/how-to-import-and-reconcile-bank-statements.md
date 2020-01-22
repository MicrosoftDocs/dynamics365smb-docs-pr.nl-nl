---
title: Bankafschriften importeren en reconciliëren
description: Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 849ee1e0115f9defe4694995050c7b2147299a21
ms.sourcegitcommit: 3d128a00358668b3fdd105ebf4604ca4e2b6743c
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/20/2019
ms.locfileid: "2910655"
---
# <a name="import-and-reconcile-bank-statements"></a><span data-ttu-id="b59b6-104">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="b59b6-104">Import and Reconcile Bank Statements</span></span>
<span data-ttu-id="b59b6-105">Banken bieden elektronische bankafschriften voor al uw financiële interacties.</span><span class="sxs-lookup"><span data-stu-id="b59b6-105">Banks provide electronic bank statements for all your financial interactions.</span></span> <span data-ttu-id="b59b6-106">U kunt deze afschriften in het bank- of giroboek importeren.</span><span class="sxs-lookup"><span data-stu-id="b59b6-106">You can import these statements into the bank or giro journals.</span></span>  

<span data-ttu-id="b59b6-107">Het importbankafschrift wordt ondersteund door de volgende protocollen:</span><span class="sxs-lookup"><span data-stu-id="b59b6-107">The import bank statement is supported by the following protocols:</span></span>  

- <span data-ttu-id="b59b6-108">Rabobank mut.asc</span><span class="sxs-lookup"><span data-stu-id="b59b6-108">Rabobank mut.asc</span></span>  
- <span data-ttu-id="b59b6-109">Rabobank vvmut.ac</span><span class="sxs-lookup"><span data-stu-id="b59b6-109">Rabobank vvmut.ac</span></span>  
- <span data-ttu-id="b59b6-110">Rabobank ASCII</span><span class="sxs-lookup"><span data-stu-id="b59b6-110">Rabobank ASCII</span></span>  
- <span data-ttu-id="b59b6-111">SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="b59b6-111">SEPA CAMT</span></span>  

## <a name="to-import-and-reconcile-bank-statements"></a><span data-ttu-id="b59b6-112">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="b59b6-112">To import and reconcile bank statements</span></span>  

1.  <span data-ttu-id="b59b6-113">Kies het pictogram ![Pagina of rapport zoeken](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Bank-/giroboek** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="b59b6-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank/Giro Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="b59b6-114">Kies de actie **Bankafschrift importeren**, selecteer het vereiste importprotocol en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="b59b6-114">Choose the **Import Bank Statement** action, select the required import protocol, and then choose the **OK** button.</span></span>  
3.  <span data-ttu-id="b59b6-115">Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.</span><span class="sxs-lookup"><span data-stu-id="b59b6-115">To reconcile the bank statements automatically when importing, on the **Options** FastTab, select the **Automatic Reconciliation** check box.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="b59b6-116">Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT.</span><span class="sxs-lookup"><span data-stu-id="b59b6-116">This function does not work for bank statement files of type SEPA CAMT.</span></span> <span data-ttu-id="b59b6-117">Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**.</span><span class="sxs-lookup"><span data-stu-id="b59b6-117">Instead, use the **Match Automatically** action on the **Bank Acc. Reconciliation** page.</span></span> <span data-ttu-id="b59b6-118">Zie [Bankrekeningen reconciliëren](../../bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="b59b6-118">For more information, see [Reconcile Bank Accounts](../../bank-how-reconcile-bank-accounts-separately.md).</span></span>  

4.  <span data-ttu-id="b59b6-119">Kies de knop **Ok**.</span><span class="sxs-lookup"><span data-stu-id="b59b6-119">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="b59b6-120">Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="b59b6-120">To import the file that contains the electronic bank statement, specify the file name and path, and then choose the **Open** button.</span></span>  

<span data-ttu-id="b59b6-121">Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek.</span><span class="sxs-lookup"><span data-stu-id="b59b6-121">The electronic bank statement is imported into the bank or giro journals.</span></span> <span data-ttu-id="b59b6-122">Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).</span><span class="sxs-lookup"><span data-stu-id="b59b6-122">For more information, see [Dutch Electronic Banking](dutch-electronic-banking.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="b59b6-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b59b6-123">See Also</span></span>  
<span data-ttu-id="b59b6-124">[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="b59b6-124">[Dutch Electronic Banking](dutch-electronic-banking.md) </span></span>  
[<span data-ttu-id="b59b6-125">Betalingen automatisch vereffenen en bankrekeningen reconciliëren</span><span class="sxs-lookup"><span data-stu-id="b59b6-125">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)
