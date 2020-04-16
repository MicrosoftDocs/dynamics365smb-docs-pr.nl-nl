---
title: Betalingsrun maken en exporteren
description: Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken. Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: aec16043be113ce157b3c36dcc4158d7ec0e3e8b
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2020
ms.locfileid: "3181087"
---
# <a name="create-and-export-payment-history"></a><span data-ttu-id="fbc83-104">Betalingsrun maken en exporteren</span><span class="sxs-lookup"><span data-stu-id="fbc83-104">Create and Export Payment History</span></span>
<span data-ttu-id="fbc83-105">Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken.</span><span class="sxs-lookup"><span data-stu-id="fbc83-105">After you have created a proposal and made any modifications, you can process the proposal to create a payment history.</span></span> <span data-ttu-id="fbc83-106">Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.</span><span class="sxs-lookup"><span data-stu-id="fbc83-106">Proposals can be created manually or automatically from a vendor or customer ledger entry.</span></span> <span data-ttu-id="fbc83-107">Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="fbc83-107">For more information, see [Create Proposals](how-to-create-proposals.md).</span></span>  

 <span data-ttu-id="fbc83-108">Voor het exporteren van betaalruns worden de volgende protocollen ondersteund:</span><span class="sxs-lookup"><span data-stu-id="fbc83-108">For exporting payment histories, the following protocols are supported:</span></span>  

- <span data-ttu-id="fbc83-109">BTL91 $)</span><span class="sxs-lookup"><span data-stu-id="fbc83-109">BTL91 $)</span></span>  
- <span data-ttu-id="fbc83-110">BBV</span><span class="sxs-lookup"><span data-stu-id="fbc83-110">BBV</span></span>  
- <span data-ttu-id="fbc83-111">PAYMUL</span><span class="sxs-lookup"><span data-stu-id="fbc83-111">PAYMUL</span></span>  

## <a name="to-create-a-payment-history-for-a-proposal"></a><span data-ttu-id="fbc83-112">Een betaalrun voor een voorstel maken</span><span class="sxs-lookup"><span data-stu-id="fbc83-112">To create a payment history for a proposal</span></span>  

1.  <span data-ttu-id="fbc83-113">Kies het pictogram ![Pagina of rapport zoeken](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Telebank - bankoverzicht** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="fbc83-113">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Telebank - Bank Overview**, and then choose the related link.</span></span>  

    <span data-ttu-id="fbc83-114">Als u het voorstel wilt afdrukken voordat u het verwerkt, kiest u de knop **Afdrukken**.</span><span class="sxs-lookup"><span data-stu-id="fbc83-114">If you want to print the proposal before you process it, choose the **Print** button.</span></span>  

2.  <span data-ttu-id="fbc83-115">Als u het voorstel wilt verwerken, kiest u de actie **Verwerken**.</span><span class="sxs-lookup"><span data-stu-id="fbc83-115">To process the proposal, choose the **Process** action.</span></span>  
3.  <span data-ttu-id="fbc83-116">Als u de betaalrun wilt bekijken, sluit u de pagina **Telebankierenvoorstel**.</span><span class="sxs-lookup"><span data-stu-id="fbc83-116">To view the payment history, close the **Telebank Proposal** page.</span></span> <span data-ttu-id="fbc83-117">Zorg dat dezelfde bankrekening op de pagina **Telebankieren - bankoverzicht** is geselecteerd en kies vervolgens de actie **Betaalrun**.</span><span class="sxs-lookup"><span data-stu-id="fbc83-117">Make sure the same bank account on the **Telebank – Bank Overview** page is selected, and then choose the **Payment History** action.</span></span>  

<span data-ttu-id="fbc83-118">De pagina **Betaalrunlijst** verschijnt met de betaalrun die u zojuist hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="fbc83-118">The **Payment History List** page displays the payment history that you just created.</span></span>  

## <a name="to-export-a-payment-history"></a><span data-ttu-id="fbc83-119">Een betaalrun exporteren</span><span class="sxs-lookup"><span data-stu-id="fbc83-119">To export a payment history</span></span>  

- <span data-ttu-id="fbc83-120">Kies op de pagina **Betaalrunlijst** de actie **Exporteren**.</span><span class="sxs-lookup"><span data-stu-id="fbc83-120">On the **Payment History List** page, choose the **Export** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="fbc83-121">Er wordt een tekstbestand gemaakt.</span><span class="sxs-lookup"><span data-stu-id="fbc83-121">A text file will be created.</span></span> <span data-ttu-id="fbc83-122">Dit bestand bevat het pad en de bestandsnaam zoals die in het veld **Standaardbestandsnamen** van het exportprotocol zijn gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="fbc83-122">This file contains the path and file name as defined in the **Default File Names Field** field of the export protocol.</span></span>  

## <a name="see-also"></a><span data-ttu-id="fbc83-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="fbc83-123">See Also</span></span>  
 [<span data-ttu-id="fbc83-124">Voorstellen maken</span><span class="sxs-lookup"><span data-stu-id="fbc83-124">Create Proposals</span></span>](how-to-create-proposals.md)
