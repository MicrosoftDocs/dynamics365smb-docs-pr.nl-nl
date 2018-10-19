---
title: 'Procedure: een offerte maken voor een op-order-assembleren-verkoop | Microsoft Docs'
description: U kunt assemblagebeheer gebruiken om een assemblageartikel op verzoek van een klant aan te passen tijdens het verkoopproces.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: kit, kitting
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: be0a80ea66dea634a37cb187408c7142d70af011
ms.contentlocale: nl-nl
ms.lasthandoff: 09/28/2018

---
# <a name="quote-an-assemble-to-order-sale"></a><span data-ttu-id="2f57d-103">Een offerte maken voor een assembleren voor order-verkoop</span><span class="sxs-lookup"><span data-stu-id="2f57d-103">Quote an Assemble-to-Order Sale</span></span>
<span data-ttu-id="2f57d-104">U kunt assemblagebeheer gebruiken om een assemblageartikel op verzoek van een klant aan te passen tijdens het verkoopproces.</span><span class="sxs-lookup"><span data-stu-id="2f57d-104">You can use assembly management to customize an assembly item to a customer’s request during the sales process.</span></span> <span data-ttu-id="2f57d-105">Zie voor meer informatie [Op order geassembleerde artikelen verkopen](assembly-how-to-sell-items-assembled-to-order.md).</span><span class="sxs-lookup"><span data-stu-id="2f57d-105">For more information, see [Sell Items Assembled to Order](assembly-how-to-sell-items-assembled-to-order.md).</span></span>  

<span data-ttu-id="2f57d-106">Als u een ander soort artikel verkoopt, kunt u ook een verkoopofferte maken voor een aangepast assemblageartikel voordat u deze omzet in een verkooporder.</span><span class="sxs-lookup"><span data-stu-id="2f57d-106">As when you sell any other type of item, you can also create a sales quote for a customized assembly item before converting it to a sales order.</span></span> <span data-ttu-id="2f57d-107">Dit proces omvat verschillende extra stappen wanneer u het vergelijkt met het maken van een normale verkoopofferte, en gebruikt assemblageoffertes, een variatie van een gekoppelde assemblageorder.</span><span class="sxs-lookup"><span data-stu-id="2f57d-107">This process involves several extra steps when you compare it to creating a regular sales quote, and it uses a variation of a linked assembly order, which is an assembly quote.</span></span>

> [!NOTE]  
>  <span data-ttu-id="2f57d-108">Zoals alle soorten van offertes worden de aantallen op assemblageoffertes niet gebruikt in beschikbaarheid, plannen of reserveringen.</span><span class="sxs-lookup"><span data-stu-id="2f57d-108">Like all types of quotes, the quantities on assembly quotes are not used in availability, planning, or reservations.</span></span>  

## <a name="to-create-a-sales-quote-for-an-assemble-to-order-item"></a><span data-ttu-id="2f57d-109">Een verkoopofferte voor een op-order-assembleren-artikel maken</span><span class="sxs-lookup"><span data-stu-id="2f57d-109">To create a sales quote for an assemble-to-order item</span></span>  
1.  <span data-ttu-id="2f57d-110">Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Verkoopofferte** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2f57d-110">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Sales Quote**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="2f57d-111">Maak een nieuwe verkoopofferteregel met één regel voor een assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="2f57d-111">Create a sales quote line with one line for an assembly item.</span></span> <span data-ttu-id="2f57d-112">Zie voor meer informatie [Verkoopoffertes maken](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="2f57d-112">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span>  
3.  <span data-ttu-id="2f57d-113">Voer de volledige aantal het in veld **Aantal voor op order assembleren** in.</span><span class="sxs-lookup"><span data-stu-id="2f57d-113">In the **Qty. to Assemble to Order** field, enter the full quantity.</span></span>

    > [!NOTE]  
    >  <span data-ttu-id="2f57d-114">U moet geen offerte maken voor een gedeeltelijke hoeveelheid.</span><span class="sxs-lookup"><span data-stu-id="2f57d-114">You should not quote a partial quantity.</span></span> <span data-ttu-id="2f57d-115">Daarom moet u dezelfde hoeveelheid invoeren die u hebt ingevoerd in het veld **Hoeveelheid** op de verkoopofferteregel.</span><span class="sxs-lookup"><span data-stu-id="2f57d-115">Therefore, you must enter the same quantity that you entered in the **Quantity** field on the sales quote line.</span></span>  

4.  <span data-ttu-id="2f57d-116">Kies op het sneltabblad **Regels** de optie **Regel** en vervolgens **Op order assembleren** en **Op orderregels assembleren**.</span><span class="sxs-lookup"><span data-stu-id="2f57d-116">On the **Lines** FastTab, choose **Line**, choose **Assemble to Order**, and then choose **Assemble-to-Order Lines**.</span></span> <span data-ttu-id="2f57d-117">Of kies het veld **Aant. op order assembleren** op de regel.</span><span class="sxs-lookup"><span data-stu-id="2f57d-117">Alternatively, choose the **Qty. to Assemble to Order** field on the line.</span></span>  
5.  <span data-ttu-id="2f57d-118">Bekijk of wijzig de assemblageorderregels volgens de offerte die de klant heeft aangevraagd in het venster **Op orderregels assembleren**.</span><span class="sxs-lookup"><span data-stu-id="2f57d-118">In the **Assemble-to-Order Lines** window, review or modify the assembly order lines according to the quote that the customer is requesting.</span></span> <span data-ttu-id="2f57d-119">Als u meer informatie wilt, kiest u de actie **Document weergeven** om het volledige offerteraamcontract te openen.</span><span class="sxs-lookup"><span data-stu-id="2f57d-119">If you want to view more information, choose the **Show Document** action to open the complete blanket quote order.</span></span> <span data-ttu-id="2f57d-120">U kunt de inhoud van de meeste velden niet wijzigen en u kunt niet boeken.</span><span class="sxs-lookup"><span data-stu-id="2f57d-120">You cannot change the contents of most fields, and you cannot post.</span></span>  
6.  <span data-ttu-id="2f57d-121">Wanneer u de assemblageorderregels hebt bijgewerkt volgens de offerte sluit u het venster **Op orderregels assembleren** om terug te keren naar het venster **Verkoopofferte**.</span><span class="sxs-lookup"><span data-stu-id="2f57d-121">When you have adjusted the assembly order lines according to the quote, close the **Assemble-to-Order Lines** window to return to the **Sales Quote** window.</span></span>  
7.  <span data-ttu-id="2f57d-122">Als de klant de offerte heeft geaccepteerd, maakt u een verkooporder voor het genoteerde assemblageartikel.</span><span class="sxs-lookup"><span data-stu-id="2f57d-122">If the customer accepts the quote, then create a sales order for the quoted assembly item.</span></span> <span data-ttu-id="2f57d-123">Zie voor meer informatie [Verkoopoffertes maken](sales-how-make-offers.md).</span><span class="sxs-lookup"><span data-stu-id="2f57d-123">For more information, see [Make Sales Quotes](sales-how-make-offers.md).</span></span> <span data-ttu-id="2f57d-124">De gekoppelde assemblageofferte en eventuele aanpassingen zijn gekoppeld aan die nieuwe verkooporder, als voorbereiding op de assemblage van het artikel of de artikelen die verkocht worden.</span><span class="sxs-lookup"><span data-stu-id="2f57d-124">The linked assembly quote and any customizations are linked to that new sales order to prepare for assembly of the item or items to be sold.</span></span>  

## <a name="see-also"></a><span data-ttu-id="2f57d-125">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2f57d-125">See Also</span></span>  
[<span data-ttu-id="2f57d-126">Assemblagebeheer</span><span class="sxs-lookup"><span data-stu-id="2f57d-126">Assembly Management</span></span>](assembly-assemble-items.md)  
[<span data-ttu-id="2f57d-127">Werken met stuklijsten</span><span class="sxs-lookup"><span data-stu-id="2f57d-127">Work with Bills of Material</span></span>](inventory-how-work-BOMs.md)  
[<span data-ttu-id="2f57d-128">Voorraad</span><span class="sxs-lookup"><span data-stu-id="2f57d-128">Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="2f57d-129">Ontwerpdetails: Magazijnbeheer</span><span class="sxs-lookup"><span data-stu-id="2f57d-129">Design Details: Warehouse Management</span></span>](design-details-warehouse-management.md)  
<span data-ttu-id="2f57d-130">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="2f57d-130">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

