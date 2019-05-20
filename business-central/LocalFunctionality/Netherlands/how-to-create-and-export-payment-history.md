---
title: Betalingsrun maken en exporteren
description: Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken. Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.
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
ms.openlocfilehash: 94d5e8e9019556ae5a39c6e1967f6b7d46094d68
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/29/2019
ms.locfileid: "1246042"
---
# <a name="create-and-export-payment-history"></a><span data-ttu-id="9f17c-104">Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="9f17c-104">Create and Export Payment History</span></span>
<span data-ttu-id="9f17c-105">Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken.</span><span class="sxs-lookup"><span data-stu-id="9f17c-105">After you have created a proposal and made any modifications, you can process the proposal to create a payment history.</span></span> <span data-ttu-id="9f17c-106">Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.</span><span class="sxs-lookup"><span data-stu-id="9f17c-106">Proposals can be created manually or automatically from a vendor or customer ledger entry.</span></span> <span data-ttu-id="9f17c-107">Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="9f17c-107">For more information, see [Create Proposals](how-to-create-proposals.md).</span></span>  

 <span data-ttu-id="9f17c-108">Voor het exporteren van betaalruns worden de volgende protocollen ondersteund:</span><span class="sxs-lookup"><span data-stu-id="9f17c-108">For exporting payment histories, the following protocols are supported:</span></span>  

- <span data-ttu-id="9f17c-109">BTL91 $)</span><span class="sxs-lookup"><span data-stu-id="9f17c-109">BTL91 $)</span></span>  
- <span data-ttu-id="9f17c-110">BBV</span><span class="sxs-lookup"><span data-stu-id="9f17c-110">BBV</span></span>  
- <span data-ttu-id="9f17c-111">PAYMUL</span><span class="sxs-lookup"><span data-stu-id="9f17c-111">PAYMUL</span></span>  

## <a name="to-create-a-payment-history-for-a-proposal"></a><span data-ttu-id="9f17c-112">Een betaalrun voor een voorstel maken</span><span class="sxs-lookup"><span data-stu-id="9f17c-112">To create a payment history for a proposal</span></span>  

1.  <span data-ttu-id="9f17c-113">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Telebankieren - bankoverzicht** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="9f17c-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  

    <span data-ttu-id="9f17c-114">Als u het voorstel wilt afdrukken voordat u het verwerkt, kiest u de knop **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="9f17c-114">If you want to print the proposal before you process it, choose the **Print** button.</span></span>  

2.  <span data-ttu-id="9f17c-115">Als u het voorstel wilt verwerken, kiest u de actie **Verwerken**.</span><span class="sxs-lookup"><span data-stu-id="9f17c-115">To process the proposal, choose the **Process** action.</span></span>  
3.  <span data-ttu-id="9f17c-116">Als u de betaalrun wilt bekijken, sluit u de pagina **Telebankierenvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="9f17c-116">To view the payment history, close the **Telebank Proposal** page.</span></span> <span data-ttu-id="9f17c-117">Zorg dat dezelfde bankrekening op de pagina **Telebankieren - bankoverzicht** is geselecteerd en kies vervolgens de actie **Betaalrun**.</span><span class="sxs-lookup"><span data-stu-id="9f17c-117">Make sure the same bank account on the **Telebank – Bank Overview** page is selected, and then choose the **Payment History** action.</span></span>  

<span data-ttu-id="9f17c-118">De pagina **Betaalrunlijst** verschijnt met de betaalrun die u zojuist hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="9f17c-118">The **Payment History List** page displays the payment history that you just created.</span></span>  

## <a name="to-export-a-payment-history"></a><span data-ttu-id="9f17c-119">Een betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="9f17c-119">To export a payment history</span></span>  

- <span data-ttu-id="9f17c-120">Kies op de pagina **Betaalrunlijst** de actie **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="9f17c-120">On the **Payment History List** page, choose the **Export** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="9f17c-121">Er wordt een tekstbestand gemaakt.</span><span class="sxs-lookup"><span data-stu-id="9f17c-121">A text file will be created.</span></span> <span data-ttu-id="9f17c-122">Dit bestand bevat het pad en de bestandsnaam zoals die in het veld **Standaardbestandsnamen** van het exportprotocol zijn gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="9f17c-122">This file contains the path and file name as defined in the **Default File Names Field** field of the export protocol.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9f17c-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9f17c-123">See Also</span></span>  
 [<span data-ttu-id="9f17c-124">Voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="9f17c-124">Create Proposals</span></span>](how-to-create-proposals.md)
