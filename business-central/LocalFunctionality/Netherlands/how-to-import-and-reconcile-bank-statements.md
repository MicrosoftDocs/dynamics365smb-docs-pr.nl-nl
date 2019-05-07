---
title: Bankafschriften importeren en reconciliëren
description: Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.
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
ms.openlocfilehash: 85d2eb3a2518dcf19934651a40db4edb74134ec6
ms.sourcegitcommit: bd78a5d990c9e83174da1409076c22df8b35eafd
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2019
ms.locfileid: "933772"
---
# <a name="import-and-reconcile-bank-statements"></a><span data-ttu-id="4fef1-104">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4fef1-104">Import and Reconcile Bank Statements</span></span>
<span data-ttu-id="4fef1-105">Banken bieden elektronische bankafschriften voor al uw financiële interacties.</span><span class="sxs-lookup"><span data-stu-id="4fef1-105">Banks provide electronic bank statements for all your financial interactions.</span></span> <span data-ttu-id="4fef1-106">U kunt deze afschriften in het bank- of giroboek importeren.</span><span class="sxs-lookup"><span data-stu-id="4fef1-106">You can import these statements into the bank or giro journals.</span></span>  

<span data-ttu-id="4fef1-107">Het importbankafschrift wordt ondersteund door de volgende protocollen:</span><span class="sxs-lookup"><span data-stu-id="4fef1-107">The import bank statement is supported by the following protocols:</span></span>  

- <span data-ttu-id="4fef1-108">Rabobank mut.asc</span><span class="sxs-lookup"><span data-stu-id="4fef1-108">Rabobank mut.asc</span></span>  
- <span data-ttu-id="4fef1-109">Rabobank vvmut.ac</span><span class="sxs-lookup"><span data-stu-id="4fef1-109">Rabobank vvmut.ac</span></span>  
- <span data-ttu-id="4fef1-110">Rabobank ASCII</span><span class="sxs-lookup"><span data-stu-id="4fef1-110">Rabobank ASCII</span></span>  
- <span data-ttu-id="4fef1-111">SEPA CAMT</span><span class="sxs-lookup"><span data-stu-id="4fef1-111">SEPA CAMT</span></span>  

## <a name="to-import-and-reconcile-bank-statements"></a><span data-ttu-id="4fef1-112">Bankafschriften importeren en reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4fef1-112">To import and reconcile bank statements</span></span>  

1.  <span data-ttu-id="4fef1-113">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bank-/giroboek** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="4fef1-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Bank/Giro Journal**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="4fef1-114">Kies de actie **Bankafschrift importeren**, selecteer het vereiste importprotocol en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4fef1-114">Choose the **Import Bank Statement** action, select the required import protocol, and then choose the **OK** button.</span></span>  
3.  <span data-ttu-id="4fef1-115">Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.</span><span class="sxs-lookup"><span data-stu-id="4fef1-115">To reconcile the bank statements automatically when importing, on the **Options** FastTab, select the **Automatic Reconciliation** check box.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="4fef1-116">Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT.</span><span class="sxs-lookup"><span data-stu-id="4fef1-116">This function does not work for bank statement files of type SEPA CAMT.</span></span> <span data-ttu-id="4fef1-117">Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**.</span><span class="sxs-lookup"><span data-stu-id="4fef1-117">Instead, use the **Match Automatically** action on the **Bank Acc. Reconciliation** page.</span></span> <span data-ttu-id="4fef1-118">Zie [Bankrekeningen apart reconciliëren](../../bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="4fef1-118">For more information, see [Reconcile Bank Accounts Separately](../../bank-how-reconcile-bank-accounts-separately.md).</span></span>  

4.  <span data-ttu-id="4fef1-119">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="4fef1-119">Choose the **OK** button.</span></span>  
5.  <span data-ttu-id="4fef1-120">Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.</span><span class="sxs-lookup"><span data-stu-id="4fef1-120">To import the file that contains the electronic bank statement, specify the file name and path, and then choose the **Open** button.</span></span>  

<span data-ttu-id="4fef1-121">Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek.</span><span class="sxs-lookup"><span data-stu-id="4fef1-121">The electronic bank statement is imported into the bank or giro journals.</span></span> <span data-ttu-id="4fef1-122">Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).</span><span class="sxs-lookup"><span data-stu-id="4fef1-122">For more information, see [Dutch Electronic Banking](dutch-electronic-banking.md).</span></span>  

## <a name="see-also"></a><span data-ttu-id="4fef1-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="4fef1-123">See Also</span></span>  
<span data-ttu-id="4fef1-124">[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md) </span><span class="sxs-lookup"><span data-stu-id="4fef1-124">[Dutch Electronic Banking](dutch-electronic-banking.md) </span></span>  
[<span data-ttu-id="4fef1-125">Betalingen automatisch vereffenen en bankrekeningen reconciliëren</span><span class="sxs-lookup"><span data-stu-id="4fef1-125">Applying Payments Automatically and Reconciling Bank Accounts</span></span>](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)
