---
title: "Een vestigingskaart instellen en transferroutes definiëren| Microsoft Docs"
description: U maakt een vestigingskaart voor elke plaats waar u voorraadartikelen opslaat, bijvoorbeeld een magazijn of een distributiecentrum, en u stelt routes in om artikelen tussen vestigingen over te brengen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: warehouse, distribution center
ms.date: 06/02/2017
ms.author: SorenGP
ms.translationtype: Human Translation
ms.sourcegitcommit: 81636fc2e661bd9b07c54da1cd5d0d27e30d01a2
ms.openlocfilehash: 146fc08f389a5c068044358c59b7d8911f0b3343
ms.contentlocale: nl-nl
ms.lasthandoff: 09/11/2017

---
# <a name="how-to-set-up-locations"></a><span data-ttu-id="e1ab8-103">Procedure: vestigingen instellen</span><span class="sxs-lookup"><span data-stu-id="e1ab8-103">How to: Set Up Locations</span></span>
<span data-ttu-id="e1ab8-104">Als u artikelen op meer dan één plaats of magazijn koopt, opslaat of verkoopt, moet u elke vestiging instellen met een vestigingskaart en transferroutes definiëren.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-104">If you buy, store, or sell items at more than one place or warehouse, you must set each location up with a location card and define transfer routes.</span></span>

<span data-ttu-id="e1ab8-105">U kunt vervolgens documentregels voor een bepaalde vestiging maken, beschikbaarheid per locatie weergeven en voorraad tussen locaties overbrengen.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-105">You can then create document lines for a specific location, view availability by location, and transfer inventory between locations.</span></span> <span data-ttu-id="e1ab8-106">Zie [Voorraad beheren](inventory-manage-inventory.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-106">For more information, see [Manage Inventory](inventory-manage-inventory.md).</span></span>

> [!NOTE]  
>   <span data-ttu-id="e1ab8-107">Deze functionaliteit vereist dat uw ervaring is ingesteld op **Pakket**.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-107">This functionality requires that your experience is set to **Suite**.</span></span> <span data-ttu-id="e1ab8-108">Zie voor meer informatie [Uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-ervaring aanpassen](ui-experiences.md).</span><span class="sxs-lookup"><span data-stu-id="e1ab8-108">For more information, see [Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md).</span></span>

## <a name="to-create-a-location-card"></a><span data-ttu-id="e1ab8-109">Een vestigingskaart maken</span><span class="sxs-lookup"><span data-stu-id="e1ab8-109">To create a location card</span></span>
1. <span data-ttu-id="e1ab8-110">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Vestigingen** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-110">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Locations**, and then choose the related link.</span></span>
2. <span data-ttu-id="e1ab8-111">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-111">Choose the **New** action.</span></span>
3. <span data-ttu-id="e1ab8-112">Vul indien nodig de velden in het venster **Vestigingskaart** in.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-112">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="e1ab8-113">Herhaal stap 2 en 3 voor elke locatie waar u voorraad wilt houden.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-113">Repeat steps 2 and 3 for every location where you want to keep inventory.</span></span>

## <a name="to-create-a-transfer-route"></a><span data-ttu-id="e1ab8-114">Een transferroute maken</span><span class="sxs-lookup"><span data-stu-id="e1ab8-114">To create a transfer route</span></span>
1. <span data-ttu-id="e1ab8-115">Kies het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Transferroutes** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-115">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Transfer Routes**, and then choose the related link.</span></span>
2. <span data-ttu-id="e1ab8-116">U kunt ook vanuit elk **Vestiging**-venster de actie **Transferroutes** kiezen.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-116">Alternatively, from any **Location Card** window, choose the **Transfer Routes** action.</span></span>
3. <span data-ttu-id="e1ab8-117">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-117">Choose the **New** action.</span></span>
4. <span data-ttu-id="e1ab8-118">Vul indien nodig de velden in het venster **Vestigingskaart** in.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-118">In the **Location Card** window, fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

<span data-ttu-id="e1ab8-119">U kunt nu voorraadartikelen tussen twee vestigingen overbrengen.</span><span class="sxs-lookup"><span data-stu-id="e1ab8-119">You can now transfer inventory items between two locations.</span></span> <span data-ttu-id="e1ab8-120">Zie voor meer informatie [Procedure: Voorraad overbrengen tussen vestigingen](inventory-how-transfer-between-locations.md).</span><span class="sxs-lookup"><span data-stu-id="e1ab8-120">For more information, see [How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md).</span></span>    

## <a name="see-also"></a><span data-ttu-id="e1ab8-121">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e1ab8-121">See Also</span></span>
[<span data-ttu-id="e1ab8-122">Voorraad beheren</span><span class="sxs-lookup"><span data-stu-id="e1ab8-122">Manage Inventory</span></span>](inventory-manage-inventory.md)  
[<span data-ttu-id="e1ab8-123">Toeleveringsketen</span><span class="sxs-lookup"><span data-stu-id="e1ab8-123">Supply Chain</span></span>](madeira-supply-chain.md)  
<span data-ttu-id="e1ab8-124">[Procedure: Voorraad overbrengen tussen vestigingen](inventory-how-transfer-between-locations.md)  </span><span class="sxs-lookup"><span data-stu-id="e1ab8-124">[How to: Transfer Inventory Between Locations](inventory-how-transfer-between-locations.md)  </span></span>  
<span data-ttu-id="e1ab8-125">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="e1ab8-125">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
<span data-ttu-id="e1ab8-126">[Uw [!INCLUDE[d365fin](includes/d365fin_md.md)]-ervaring aanpassen](ui-experiences.md)</span><span class="sxs-lookup"><span data-stu-id="e1ab8-126">[Customizing Your [!INCLUDE[d365fin](includes/d365fin_md.md)] Experience](ui-experiences.md)</span></span>  
[<span data-ttu-id="e1ab8-127">Algemene bedrijfsfunctionaliteit</span><span class="sxs-lookup"><span data-stu-id="e1ab8-127">General Business Functionality</span></span>](ui-across-business-areas.md)

