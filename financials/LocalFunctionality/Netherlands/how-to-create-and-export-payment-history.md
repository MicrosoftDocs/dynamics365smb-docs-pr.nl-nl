---
title: Betalingsrun maken en exporteren
description: Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken. Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.
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
ms.openlocfilehash: 4f890992cc6982ee20741fda53e6fa27f92b035e
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="create-and-export-payment-history"></a><span data-ttu-id="ba78e-104">Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="ba78e-104">Create and Export Payment History</span></span>
<span data-ttu-id="ba78e-105">Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken.</span><span class="sxs-lookup"><span data-stu-id="ba78e-105">After you have created a proposal and made any modifications, you can process the proposal to create a payment history.</span></span> <span data-ttu-id="ba78e-106">Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.</span><span class="sxs-lookup"><span data-stu-id="ba78e-106">Proposals can be created manually or automatically from a vendor or customer ledger entry.</span></span> <span data-ttu-id="ba78e-107">Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="ba78e-107">For more information, see [Create Proposals](how-to-create-proposals.md).</span></span>  

 <span data-ttu-id="ba78e-108">Voor het exporteren van betaalruns worden de volgende protocollen ondersteund:</span><span class="sxs-lookup"><span data-stu-id="ba78e-108">For exporting payment histories, the following protocols are supported:</span></span>  

- <span data-ttu-id="ba78e-109">BTL91 $)</span><span class="sxs-lookup"><span data-stu-id="ba78e-109">BTL91 $)</span></span>  
- <span data-ttu-id="ba78e-110">BBV</span><span class="sxs-lookup"><span data-stu-id="ba78e-110">BBV</span></span>  
- <span data-ttu-id="ba78e-111">PAYMUL</span><span class="sxs-lookup"><span data-stu-id="ba78e-111">PAYMUL</span></span>  

## <a name="to-create-a-payment-history-for-a-proposal"></a><span data-ttu-id="ba78e-112">Een betaalrun voor een voorstel maken</span><span class="sxs-lookup"><span data-stu-id="ba78e-112">To create a payment history for a proposal</span></span>  

1.  <span data-ttu-id="ba78e-113">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="ba78e-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  

    <span data-ttu-id="ba78e-114">Als u het voorstel wilt afdrukken voordat u het verwerkt, kiest u de knop **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="ba78e-114">If you want to print the proposal before you process it, choose the **Print** button.</span></span>  

2.  <span data-ttu-id="ba78e-115">Als u het voorstel wilt verwerken, kiest u de actie **Verwerken**.</span><span class="sxs-lookup"><span data-stu-id="ba78e-115">To process the proposal, choose the **Process** action.</span></span>  
3.  <span data-ttu-id="ba78e-116">Als u de betaalrun wilt bekijken, sluit u het venster **Telebankierenvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="ba78e-116">To view the payment history, close the **Telebank Proposal** window.</span></span> <span data-ttu-id="ba78e-117">Zorg dat dezelfde bankrekening in het venster **Telebankieren - bankoverzicht** is geselecteerd en kies vervolgens de actie **Betaalrun**.</span><span class="sxs-lookup"><span data-stu-id="ba78e-117">Make sure the same bank account in the **Telebank – Bank Overview** window is selected, and then choose the **Payment History** action.</span></span>  

<span data-ttu-id="ba78e-118">Het venster **Betaalrunlijst** verschijnt met de betaalrun die u zojuist hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="ba78e-118">The **Payment History List** window displays the payment history that you just created.</span></span>  

## <a name="to-export-a-payment-history"></a><span data-ttu-id="ba78e-119">Een betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="ba78e-119">To export a payment history</span></span>  

- <span data-ttu-id="ba78e-120">Kies in het venster **Betaalrunlijst** de actie **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="ba78e-120">In the **Payment History List** window, choose the **Export** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="ba78e-121">Er wordt een tekstbestand gemaakt.</span><span class="sxs-lookup"><span data-stu-id="ba78e-121">A text file will be created.</span></span> <span data-ttu-id="ba78e-122">Dit bestand bevat het pad en de bestandsnaam zoals die in het veld **Standaardbestandsnamen** van het exportprotocol zijn gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="ba78e-122">This file contains the path and file name as defined in the **Default File Names Field** field of the export protocol.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ba78e-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="ba78e-123">See Also</span></span>  
 [<span data-ttu-id="ba78e-124">Voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="ba78e-124">Create Proposals</span></span>](how-to-create-proposals.md)

