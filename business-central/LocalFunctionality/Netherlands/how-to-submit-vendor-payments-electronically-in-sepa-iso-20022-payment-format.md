---
title: Leveranciersbetalingen elektronisch versturen in de betalingsindeling SEPA ISO 20022
description: In Business Central kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.
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
ms.openlocfilehash: a367c4d952c7bfdcfac1ac9513edc5e038b38b21
ms.contentlocale: nl-nl
ms.lasthandoff: 09/28/2018

---
# <a name="submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a><span data-ttu-id="6d5e4-103">Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling</span><span class="sxs-lookup"><span data-stu-id="6d5e4-103">Submit Vendor Payments Electronically in SEPA ISO 20022 Payment Format</span></span>
<span data-ttu-id="6d5e4-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can create and submit Single Euro Payments Area (SEPA) ISO 20022 vendor payments electronically.</span></span>  

<span data-ttu-id="6d5e4-105">Voordat u SEPA-leveranciersbetalingen kunt maken en verzenden, moet u SEPA-betalingen activeren.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-105">Before you can create and submit SEPA vendor payments, you must enable SEPA payments.</span></span> <span data-ttu-id="6d5e4-106">Zie [SEPA-betalingen activeren](how-to-activate-sepa-payments.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-106">For more information, see [Activate SEPA Payments](how-to-activate-sepa-payments.md).</span></span>  

## <a name="to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a><span data-ttu-id="6d5e4-107">Leverancierbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling</span><span class="sxs-lookup"><span data-stu-id="6d5e4-107">To submit vendor payments electronically in SEPA ISO 20022 payment format</span></span>  

1.  <span data-ttu-id="6d5e4-108">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank-Bank Overview**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="6d5e4-109">Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-109">Select the relevant bank account, and then choose the **Proposal** action.</span></span>  
3.  <span data-ttu-id="6d5e4-110">Selecteer de betreffende leveranciersbankrekening en kies vervolgens de actie **Posten ophalen**.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-110">Select the relevant vendor bank account, and then choose the **Get Entries** action.</span></span>  
4.  <span data-ttu-id="6d5e4-111">Vul op het sneltabblad **Opties** van de batchverwerking **Voorstelposten ophalen** de velden in, zoals wordt beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-111">In the **Get Proposal Entries** batch job, on the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="6d5e4-112">Veld</span><span class="sxs-lookup"><span data-stu-id="6d5e4-112">Field</span></span>|<span data-ttu-id="6d5e4-113">Description</span><span class="sxs-lookup"><span data-stu-id="6d5e4-113">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="6d5e4-114">**Valutadatum**</span><span class="sxs-lookup"><span data-stu-id="6d5e4-114">**Currency Date**</span></span>|<span data-ttu-id="6d5e4-115">Hier geeft u de valutadatum op.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-115">Specify the currency date.</span></span>|  
    |<span data-ttu-id="6d5e4-116">**Vervaldatum contantkort.**</span><span class="sxs-lookup"><span data-stu-id="6d5e4-116">**Pmt. Discount Date**</span></span>|<span data-ttu-id="6d5e4-117">Hier geeft u de vervaldatum voor de contantkorting op.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-117">Specify the payment discount date.</span></span>|  

5.  <span data-ttu-id="6d5e4-118">Selecteer in het sneltabblad **Transactiemodus** de gewenste filters.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-118">On the **Transaction Mode** FastTab, select the appropriate filters.</span></span>  
6.  <span data-ttu-id="6d5e4-119">Selecteer in het sneltabblad **Klantenpost** de gewenste filters.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-119">On the **Cust. Ledger Entry** FastTab, select the appropriate filters.</span></span>  
7.  <span data-ttu-id="6d5e4-120">Selecteer op het sneltabblad **Leverancierspost** het filter **Leveranciersnr.** en selecteer een leveranciersnummer.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-120">On the **Vendor Ledger Entry** FastTab, select the **Vendor No.** filter, and then select a vendor number.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="6d5e4-121">Selecteer eventuele overige vereiste filters.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-121">Select other appropriate filters if required.</span></span>  

8.  <span data-ttu-id="6d5e4-122">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-122">Choose the **OK** button.</span></span>  

<span data-ttu-id="6d5e4-123">De voorstelregels worden opgenomen in het venster **Telebankierenvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="6d5e4-123">The proposal lines populate in the **Telebank Proposal** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="6d5e4-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="6d5e4-124">See Also</span></span>  
 <span data-ttu-id="6d5e4-125">[SEPA-betalingen activeren](how-to-activate-sepa-payments.md) </span><span class="sxs-lookup"><span data-stu-id="6d5e4-125">[Activate SEPA Payments](how-to-activate-sepa-payments.md) </span></span>  
 [<span data-ttu-id="6d5e4-126">Single EURO Payments Area (SEPA)</span><span class="sxs-lookup"><span data-stu-id="6d5e4-126">Single EURO Payments Area (SEPA)</span></span>](single-euro-payments-area-sepa-.md)   

