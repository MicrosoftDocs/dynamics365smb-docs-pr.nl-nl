---
title: Aangepaste configuratiepakketten voor bedrijven maken | Microsoft Docs
description: Naarmate uw bedrijf groeit, zult u waarschijnlijk gaan vertrouwen op een set bedrijfstypen die u met de meeste van uw klanten gebruikt. U kunt uw implementatieproces stroomlijnen door van deze typen configuratiepakketten voor bedrijven te maken die beschikbaar zijn voor hergebruik.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 99fad48961dc201a25af061cf982a1c65d9446bd
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2878862"
---
# <a name="create-custom-company-configuration-packages"></a><span data-ttu-id="93945-104">Aangepaste configuratiepakketten voor bedrijven maken</span><span class="sxs-lookup"><span data-stu-id="93945-104">Create Custom Company Configuration Packages</span></span>
<span data-ttu-id="93945-105">Naarmate uw bedrijf groeit, zult u waarschijnlijk gaan vertrouwen op een set bedrijfstypen die u met de meeste van uw klanten gebruikt.</span><span class="sxs-lookup"><span data-stu-id="93945-105">As you grow your business, you will likely come to rely on a set of company types that you use with most of your customers.</span></span> <span data-ttu-id="93945-106">U kunt uw implementatieproces stroomlijnen door van deze typen configuratiepakketten voor bedrijven te maken die beschikbaar zijn voor hergebruik.</span><span class="sxs-lookup"><span data-stu-id="93945-106">You can streamline your implementation process by turning these types into company configuration packages that are available for reuse.</span></span>  

<span data-ttu-id="93945-107">In het algemeen maakt u een configuratiepakket per functiegebied. Zo kunt u bijvoorbeeld een pakket maken voor uw productiefunctionaliteit.</span><span class="sxs-lookup"><span data-stu-id="93945-107">In general, create a configuration package per functional area, for example, create a package for your manufacturing functionality.</span></span> <span data-ttu-id="93945-108">Dat kunt u vervolgens toepassen en nieuwe gebieden in een bedrijf instellen als u ze nodig hebt</span><span class="sxs-lookup"><span data-stu-id="93945-108">That lets you apply and set up new areas in a company as you need them</span></span>  

<span data-ttu-id="93945-109">Een andere benadering zou zijn om een pakket te maken dat de tabellen bevat waarin de instellingen worden gedefinieerd, zoals de volgende:</span><span class="sxs-lookup"><span data-stu-id="93945-109">Another approach would be to create a package that includes the tables that define setup, such as the following:</span></span>  

-   <span data-ttu-id="93945-110">VA-instellingen</span><span class="sxs-lookup"><span data-stu-id="93945-110">Fixed Asset Setup</span></span>  
-   <span data-ttu-id="93945-111">Grootboekinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-111">General Ledger Setup</span></span>  
-   <span data-ttu-id="93945-112">Voorraadinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-112">Inventory Setup</span></span>  
-   <span data-ttu-id="93945-113">Productie-instellingen</span><span class="sxs-lookup"><span data-stu-id="93945-113">Manufacturing Setup</span></span>  
-   <span data-ttu-id="93945-114">Inkoopinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-114">Purchases and Payables Setup</span></span>  
-   <span data-ttu-id="93945-115">Marketinginstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-115">Marketing Setup</span></span>  
-   <span data-ttu-id="93945-116">Service-instellingen</span><span class="sxs-lookup"><span data-stu-id="93945-116">Service Setup</span></span>  
-   <span data-ttu-id="93945-117">Verkoopinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-117">Sales and Receivables Setup</span></span>  
-   <span data-ttu-id="93945-118">Magazijninstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-118">Warehouse Setup</span></span>  
-   <span data-ttu-id="93945-119">Boekingsgroepinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-119">General Posting Setup</span></span>  
-   <span data-ttu-id="93945-120">Btw-boekingsgroepinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-120">VAT Posting Setup</span></span>  
-   <span data-ttu-id="93945-121">Voorraadboekingsinstellingen</span><span class="sxs-lookup"><span data-stu-id="93945-121">Inventory Posting Setup</span></span>  

<span data-ttu-id="93945-122">Als u een complete lijst met instellingstabellen wilt zien, kiest u het pictogram Lampje dat de functie ![Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voert u **Handmatige instelling** in en kiest u vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="93945-122">To see a complete list of setup tables, Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Manual Setup**, and then choose the related link.</span></span>  

## <a name="to-create-a-custom-company-configuration-package"></a><span data-ttu-id="93945-123">Een aangepast configuratiepakket voor een bedrijf maken</span><span class="sxs-lookup"><span data-stu-id="93945-123">To create a custom company configuration package</span></span>  
1.  <span data-ttu-id="93945-124">Maak een nieuw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="93945-124">Create a new company.</span></span> <span data-ttu-id="93945-125">Zie voor meer informatie [Nieuwe bedrijven maken in Business Central](about-new-company.md).</span><span class="sxs-lookup"><span data-stu-id="93945-125">For more information, see [Creating New Companies in Business Central](about-new-company.md).</span></span>  
3.  <span data-ttu-id="93945-126">Stel het nieuwe bedrijf in op de door u benodigde wijze.</span><span class="sxs-lookup"><span data-stu-id="93945-126">Set up the new company in the way you need.</span></span> <span data-ttu-id="93945-127">Vul alle vereiste instellingentabellen in.</span><span class="sxs-lookup"><span data-stu-id="93945-127">Fill in all required setup tables.</span></span>  
4.  <span data-ttu-id="93945-128">Open het nieuwe bedrijf.</span><span class="sxs-lookup"><span data-stu-id="93945-128">Open the new company.</span></span>
5. <span data-ttu-id="93945-129">Open de pagina **Configuratiewerkblad**.</span><span class="sxs-lookup"><span data-stu-id="93945-129">Open the **Configuration Worksheet** page.</span></span>  
6.  <span data-ttu-id="93945-130">Voeg de tabellen die u wilt overbrengen naar een ander bedrijf toe aan het werkblad.</span><span class="sxs-lookup"><span data-stu-id="93945-130">Add the tables that you want to transfer to another company to the worksheet.</span></span> <span data-ttu-id="93945-131">Wijs de werkbladregels toe aan het pakket.</span><span class="sxs-lookup"><span data-stu-id="93945-131">Assign the worksheet lines to the package.</span></span>  
7.  <span data-ttu-id="93945-132">Maak een vragenlijst voor de meest gebruikte instellingentabel.</span><span class="sxs-lookup"><span data-stu-id="93945-132">Create a questionnaire for the most frequently used setup tables.</span></span>  
8.  <span data-ttu-id="93945-133">Stel configuratiesjablonen op om het gemakkelijker te maken om hoofdgegevens, zoals klanten of artikelen, te definiëren.</span><span class="sxs-lookup"><span data-stu-id="93945-133">Create configuration templates to make it easier to create master data, such as customers or items.</span></span>  
9.  <span data-ttu-id="93945-134">Exporteer uw pakket als een .rapidstart-bestand.</span><span class="sxs-lookup"><span data-stu-id="93945-134">Export your package as a .rapidstart file.</span></span>  

## <a name="see-also"></a><span data-ttu-id="93945-135">Zie ook</span><span class="sxs-lookup"><span data-stu-id="93945-135">See Also</span></span>  
[<span data-ttu-id="93945-136">Een bedrijf instellen met RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="93945-136">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="93945-137">Beheer</span><span class="sxs-lookup"><span data-stu-id="93945-137">Administration</span></span>](admin-setup-and-administration.md)
