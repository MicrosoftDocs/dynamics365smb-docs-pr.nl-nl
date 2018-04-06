---
title: Elektronische btw- en ICP-aangiften maken
description: Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**. Vervolgens kunt u ze naar de belastingdienst verzenden.
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
ms.openlocfilehash: 34520c70c0871c9bd1624b3f331834d5b3094f71
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="create-electronic-vat-and-icp-declarations"></a><span data-ttu-id="bfb86-104">Elektronische btw- en ICP-aangiften maken</span><span class="sxs-lookup"><span data-stu-id="bfb86-104">Create Electronic VAT and ICP Declarations</span></span>
<span data-ttu-id="bfb86-105">Als u elektronische btw- en ICP-aangiften wilt maken, moet u eerst de aangifte instellen met het venster **Elek. aangifte-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="bfb86-105">To create electronic VAT and ICP declarations, you must first set up the declaration using the **Elec. Tax Declaration Setup** window.</span></span> <span data-ttu-id="bfb86-106">Vervolgens kunt u ze naar de belastingdienst verzenden.</span><span class="sxs-lookup"><span data-stu-id="bfb86-106">Then you can submit them to the tax authorities.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="bfb86-107">Als u het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen** hebt geselecteerd, kunt u een elektronische aangifte voor slechts één bedrijf maken.</span><span class="sxs-lookup"><span data-stu-id="bfb86-107">If you have selected the **Part of Fiscal Entity** field in the **Elec. Tax Declaration Setup** window, then you can create an electronic declaration for only one company.</span></span> <span data-ttu-id="bfb86-108">Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen.</span><span class="sxs-lookup"><span data-stu-id="bfb86-108">If you want to combine the tax information for all subsidiaries of a holding company, you must create a VAT statement on paper for each subsidiary company and manually calculate the total amounts for the holding company.</span></span> <span data-ttu-id="bfb86-109">Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="bfb86-109">These total amounts of the holding company must be entered on the website of the tax authorities.</span></span> <span data-ttu-id="bfb86-110">U kunt geen belastinggegevens van ICP-aangiften combineren.</span><span class="sxs-lookup"><span data-stu-id="bfb86-110">You cannot combine tax information for ICP declarations.</span></span> <span data-ttu-id="bfb86-111">ICP-aangiften moeten altijd afzonderlijk worden ingediend.</span><span class="sxs-lookup"><span data-stu-id="bfb86-111">ICP declarations must always be submitted individually.</span></span>  

<span data-ttu-id="bfb86-112">Als er geen intracommunautaire leveringen zijn geweest in de aangifteperiode, dan wordt er een elektronische ICP-aangifte aangemaakt zonder XML-elementen voor de leveringen.</span><span class="sxs-lookup"><span data-stu-id="bfb86-112">If there are no intra-community deliveries in the declaration period, then an electronic ICP declaration is created without XML elements for the deliveries.</span></span> <span data-ttu-id="bfb86-113">Als u een dergelijke aangifte verzendt, wordt een foutbericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="bfb86-113">If you submit such a declaration, an error message will be displayed.</span></span>  

## <a name="to-create-an-electronic-vat-or-icp-declaration"></a><span data-ttu-id="bfb86-114">Een elektronische btw- of ICP-aangifte maken</span><span class="sxs-lookup"><span data-stu-id="bfb86-114">To create an electronic VAT or ICP declaration</span></span>  

1.  <span data-ttu-id="bfb86-115">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="bfb86-115">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Declarations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="bfb86-116">Kies in het venster **Overzicht elektronische aangiften** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="bfb86-116">In the **Elec. Tax Declaration List** window, choose the **New** action.</span></span>  
3.  <span data-ttu-id="bfb86-117">Vul in het venster **Elektronische aangiftekaart** op het sneltabblad **Algemeen** de vereiste velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="bfb86-117">In the **Elec. Tax Declaration Card** window, on the **General** FastTab, fill in the required fields as described in the following table.</span></span>  

    |<span data-ttu-id="bfb86-118">Veld</span><span class="sxs-lookup"><span data-stu-id="bfb86-118">Field</span></span>|<span data-ttu-id="bfb86-119">Description</span><span class="sxs-lookup"><span data-stu-id="bfb86-119">Description</span></span>|  
    |-----------------------------------|---------------------------------------|  
    |<span data-ttu-id="bfb86-120">**Sjabloonnaam**</span><span class="sxs-lookup"><span data-stu-id="bfb86-120">**Template Name**</span></span>|<span data-ttu-id="bfb86-121">De naam van de sjabloon die wordt gebruikt om de elektronische aangifte te maken.</span><span class="sxs-lookup"><span data-stu-id="bfb86-121">The name of the template that will be used to create the electronic declaration.</span></span>|  
    |<span data-ttu-id="bfb86-122">**Aangifte**</span><span class="sxs-lookup"><span data-stu-id="bfb86-122">**Statement Name**</span></span>|<span data-ttu-id="bfb86-123">De naam van het afschrift dat wordt gebruikt om de elektronische aangifte te maken.</span><span class="sxs-lookup"><span data-stu-id="bfb86-123">The name of the statement that will be used to create the electronic declaration.</span></span>|  

6.  <span data-ttu-id="bfb86-124">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="bfb86-124">Choose the **OK** button.</span></span>  

<span data-ttu-id="bfb86-125">De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** in het venster **Elektronische aangiftekaart**.</span><span class="sxs-lookup"><span data-stu-id="bfb86-125">The XML elements and the accompanying data of the electronic declaration are displayed on the **Lines** FastTab in the **Elec. Tax Declaration Card** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="bfb86-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="bfb86-126">See Also</span></span>  
 <span data-ttu-id="bfb86-127">[Elektronische belastingaangiften](electronic-tax-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="bfb86-127">[Electronic Tax Declarations](electronic-tax-declarations.md) </span></span>  
 <span data-ttu-id="bfb86-128">[Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="bfb86-128">[Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md) </span></span>  
 [<span data-ttu-id="bfb86-129">Btw-categorieën instellen</span><span class="sxs-lookup"><span data-stu-id="bfb86-129">Set Up VAT Categories</span></span>](how-to-set-up-vat-categories.md)

