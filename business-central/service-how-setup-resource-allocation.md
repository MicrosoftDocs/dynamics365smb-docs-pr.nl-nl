---
title: Resourcetoewijzing instellen | Microsoft Docs
description: Leer hoe u er met het systeem voor kunt zorgen dat u iemand toewijst die over de vereiste vaardigheden beschikt om een service te bieden.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: resource, skill, service, zones
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 6cd246809d6b05f87c131c584267551938f74810
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5392521"
---
# <a name="set-up-resource-allocation"></a><span data-ttu-id="18702-103">Resourcetoewijzing instellen</span><span class="sxs-lookup"><span data-stu-id="18702-103">Set Up Resource Allocation</span></span>
<span data-ttu-id="18702-104">Om ervoor te zorgen dat een servicetaak goed wordt uitgevoerd, is het belangrijk een resource te vinden die gekwalificeerd is om het werk uit te voeren.</span><span class="sxs-lookup"><span data-stu-id="18702-104">To ensure that a service task is performed well, it's important to find a resource who is qualified to do the work.</span></span> <span data-ttu-id="18702-105">U kunt [!INCLUDE[prod_short](includes/prod_short.md)] zo instellen dat het eenvoudig is om iemand toe te wijzen die over de juiste bekwaamheden voor het project beschikt.</span><span class="sxs-lookup"><span data-stu-id="18702-105">You can set up [!INCLUDE[prod_short](includes/prod_short.md)] so that it's easy to allocate someone who has the right skills for the job.</span></span> <span data-ttu-id="18702-106">In [!INCLUDE[prod_short](includes/prod_short.md)] noemen we dit _resourcetoewijzing_.</span><span class="sxs-lookup"><span data-stu-id="18702-106">In [!INCLUDE[prod_short](includes/prod_short.md)], we call this _resource allocation_.</span></span> <span data-ttu-id="18702-107">U kunt resources toewijzen op basis van hun vaardigheden, beschikbaarheid en locatie (of ze zich in dezelfde serviceregio als de klant bevinden).</span><span class="sxs-lookup"><span data-stu-id="18702-107">You can allocate resources based on their skill, availability, or whether they are in the same service zone as the customer.</span></span> 

<span data-ttu-id="18702-108">U moet het volgende instellen om resourcetoewijzing te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="18702-108">To use resource allocation, you must set up:</span></span>  
  
* <span data-ttu-id="18702-109">De benodigde bekwaamheden om serviceartikelen te repareren en te onderhouden.</span><span class="sxs-lookup"><span data-stu-id="18702-109">The skills required to repair and maintain service items.</span></span> <span data-ttu-id="18702-110">U wijst deze toe aan serviceartikelen en resources.</span><span class="sxs-lookup"><span data-stu-id="18702-110">You assign these to service items and resources.</span></span>  
* <span data-ttu-id="18702-111">Geografische gebieden, regio's, die u voor de markt definieert.</span><span class="sxs-lookup"><span data-stu-id="18702-111">Geographic regions, called zones, that you define for your market.</span></span> <span data-ttu-id="18702-112">Dit kunnen bijvoorbeeld Oost, West, Centraal, enzovoort zijn.</span><span class="sxs-lookup"><span data-stu-id="18702-112">For example, East, West, Central, and so on.</span></span> <span data-ttu-id="18702-113">U wijst deze toe aan klanten en resources.</span><span class="sxs-lookup"><span data-stu-id="18702-113">You assign these to customers and resources.</span></span>  
* <span data-ttu-id="18702-114">Of er resourcebekwaamheden en -regio's moeten worden weergegeven en of er een waarschuwing moet worden weergegeven als iemand een ongeschikte resource kiest of een resource die zich niet in de klantregio bevindt.</span><span class="sxs-lookup"><span data-stu-id="18702-114">Whether to display resource skills and zones, and whether to display a warning if someone chooses unqualified resource, or a resource that is not in the customer zone.</span></span>  

## <a name="to-set-up-skills"></a><span data-ttu-id="18702-115">Bekwaamheden instellen</span><span class="sxs-lookup"><span data-stu-id="18702-115">To set up skills</span></span>
1. <span data-ttu-id="18702-116">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bekwaamheden** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-116">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Skills**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-117">Vul de vereiste velden in.</span><span class="sxs-lookup"><span data-stu-id="18702-117">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-skills-to-service-items-and-resources"></a><span data-ttu-id="18702-118">Bekwaamheden toewijzen aan serviceartikelen en resources</span><span class="sxs-lookup"><span data-stu-id="18702-118">To assign skills to service items and resources</span></span>
1. <span data-ttu-id="18702-119">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Serviceartikelen** of **Resources** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-119">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Items** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-120">Open de kaart voor het serviceartikel of de resource en kies een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="18702-120">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="18702-121">Voor serviceartikelen kiest u **Resourcebekwaamheden**.</span><span class="sxs-lookup"><span data-stu-id="18702-121">For service items, choose **Resource Skills**.</span></span>  
    * <span data-ttu-id="18702-122">Voor resources kiest u **Bekwaamheden**.</span><span class="sxs-lookup"><span data-stu-id="18702-122">For resources, choose **Skills**.</span></span>  

## <a name="to-set-up-zones"></a><span data-ttu-id="18702-123">Regio's instellen</span><span class="sxs-lookup"><span data-stu-id="18702-123">To set up zones</span></span>
1. <span data-ttu-id="18702-124">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Zones** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-124">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Zones**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-125">Vul de vereiste velden in.</span><span class="sxs-lookup"><span data-stu-id="18702-125">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

## <a name="to-assign-zones-to-customers-and-resources"></a><span data-ttu-id="18702-126">Regio's toewijzen aan klanten en resources</span><span class="sxs-lookup"><span data-stu-id="18702-126">To assign zones to customers and resources</span></span> 
1. <span data-ttu-id="18702-127">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Klanten** of **Resources** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-127">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers** or **Resources**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-128">Open de kaart voor het serviceartikel of de resource en kies een van de volgende opties:</span><span class="sxs-lookup"><span data-stu-id="18702-128">Open the card for the service item or resource, and then choose one of the following:</span></span>  
  
    * <span data-ttu-id="18702-129">Voor klanten kiest u een regio in het veld **Serviceregiocode**.</span><span class="sxs-lookup"><span data-stu-id="18702-129">For customers, choose a zone in the **Service Zone Code** field.</span></span>  
    * <span data-ttu-id="18702-130">Voor resources kiest u de actie **Serviceregio's**.</span><span class="sxs-lookup"><span data-stu-id="18702-130">For resources, choose the **Service Zones** action.</span></span>  

## <a name="to-specify-what-to-show-when-a-resource-is-chosen"></a><span data-ttu-id="18702-131">Opgeven wat er moet worden weergegeven wanneer een resource is gekozen</span><span class="sxs-lookup"><span data-stu-id="18702-131">To specify what to show when a resource is chosen</span></span>
1. <span data-ttu-id="18702-132">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Servicebeheerinstellingen** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-132">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Service Management Setup**, and then choose the related link.</span></span> 
2. <span data-ttu-id="18702-133">Kies in het veld **Optie resourcebekwaamheden** een van de opties die in de volgende tabel worden beschreven.</span><span class="sxs-lookup"><span data-stu-id="18702-133">In the **Resource Skills Option** field, choose one of the options described in the following table.</span></span>  
  
    |<span data-ttu-id="18702-134">**Optie**</span><span class="sxs-lookup"><span data-stu-id="18702-134">**Option**</span></span>|<span data-ttu-id="18702-135">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="18702-135">**Description**</span></span>|  
    |------------|-------------|  
    |<span data-ttu-id="18702-136">Code getoond</span><span class="sxs-lookup"><span data-stu-id="18702-136">Code Shown</span></span> | <span data-ttu-id="18702-137">Alleen de code wordt weergegeven.</span><span class="sxs-lookup"><span data-stu-id="18702-137">Displays the code only.</span></span>|  
    |<span data-ttu-id="18702-138">Waarschuwing getoond</span><span class="sxs-lookup"><span data-stu-id="18702-138">Warning Displayed</span></span> | <span data-ttu-id="18702-139">De informatie wordt weergegeven en er wordt een waarschuwing weergegeven als u een resource kiest die niet geschikt is.</span><span class="sxs-lookup"><span data-stu-id="18702-139">Shows the information and displays a warning if you choose a resource that is not qualified.</span></span>|  
    |<span data-ttu-id="18702-140">Niet gebruikt.</span><span class="sxs-lookup"><span data-stu-id="18702-140">Not Used</span></span> | <span data-ttu-id="18702-141">Geef deze gegevens niet weer.</span><span class="sxs-lookup"><span data-stu-id="18702-141">Does not show this information.</span></span>|  

## <a name="to-update-resource-capacity"></a><span data-ttu-id="18702-142">Resourcecapaciteit bijwerken</span><span class="sxs-lookup"><span data-stu-id="18702-142">To update resource capacity</span></span>  
<span data-ttu-id="18702-143">U kunt de resourcecapaciteit desgewenst wijzigen.</span><span class="sxs-lookup"><span data-stu-id="18702-143">You may need to change the capacity of resources.</span></span>  
  
1. <span data-ttu-id="18702-144">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Resourcecapaciteit** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-144">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Resource Capacity**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-145">Kies de resource en kies vervolgens de actie **Capaciteit instellen**.</span><span class="sxs-lookup"><span data-stu-id="18702-145">Choose the resource, and then choose the **Set Capacity** action.</span></span>  
3. <span data-ttu-id="18702-146">Breng de wijzigingen aan en kies **Capaciteit bijwerken**.</span><span class="sxs-lookup"><span data-stu-id="18702-146">Make the changes, and then choose **Update Capacity**.</span></span>  

## <a name="to-update-skills-for-items-service-items-or-service-item-groups"></a><span data-ttu-id="18702-147">Bekwaamheden voor artikelen, serviceartikelen of serviceartikelgroepen bijwerken</span><span class="sxs-lookup"><span data-stu-id="18702-147">To update skills for items, service items, or service item groups</span></span>
<span data-ttu-id="18702-148">Wilt u de bekwaamheidscodes wijzigen die aan artikelen zijn toegewezen, bijvoorbeeld van **PC** in **STUKS**, dan kunt u dit voor een artikel, serviceartikel of alle items in een serviceartikelgroep doen.</span><span class="sxs-lookup"><span data-stu-id="18702-148">If you want to change the skill codes assigned to items, for example from **PC** to **PCS**, you can do so either for an item, service item, or for all items in a service item group.</span></span>  
  
1. <span data-ttu-id="18702-149">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikelen** of **Serviceartikelen** of **Serviceartikelgroep** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="18702-149">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Items** or **Service Item**, or **Service Item Group**, and then choose the related link.</span></span>  
2. <span data-ttu-id="18702-150">Kies de entiteit die u wilt bijwerken en kies vervolgens de actie **Resourcebekwaamheden**.</span><span class="sxs-lookup"><span data-stu-id="18702-150">Choose the entity to update, and then choose the **Resource Skills** action.</span></span>  
3. <span data-ttu-id="18702-151">Op de regel met de code die u wilt wijzigen, selecteert u de betreffende bekwaamheidscode in het veld **Bekwaamheidscode**.</span><span class="sxs-lookup"><span data-stu-id="18702-151">On the line with the code to be changed, in the **Skill Code** field, choose the relevant skill code.</span></span>  
4.  <span data-ttu-id="18702-152">Als er serviceartikelen aan het artikel zijn gekoppeld, wordt er een dialoogvenster geopend met de volgende twee opties:</span><span class="sxs-lookup"><span data-stu-id="18702-152">If the item has associated service items, a dialog box opens with the following two options:</span></span>  
  
    * <span data-ttu-id="18702-153">De bekwaamheidscodes wijzigen in de geselecteerde waarde: selecteer deze optie als u de oude bekwaamheidscode voor alle gerelateerde serviceartikelen wilt vervangen door de nieuwe code.</span><span class="sxs-lookup"><span data-stu-id="18702-153">Change the skill codes to the selected value: Select this option if you want to replace the old skill code with the new one on all the related service items.</span></span>  
    * <span data-ttu-id="18702-154">De bekwaamheidscodes verwijderen of hun relatie bijwerken: selecteer deze optie als u alleen voor dit artikel de bekwaamheidscode wilt wijzigen.</span><span class="sxs-lookup"><span data-stu-id="18702-154">Delete the skill codes or update their relation: Select this option if you want to change the skill code on this item only.</span></span> <span data-ttu-id="18702-155">De bekwaamheidscode voor de gerelateerde serviceartikelen wordt opnieuw toegewezen, dat wil zeggen dat het veld **Toegewezen vanuit** wordt bijgewerkt.</span><span class="sxs-lookup"><span data-stu-id="18702-155">The skill code on the related service items will be reassigned, that is, the **Assigned From** field will be updated.</span></span>  
  
## <a name="see-also"></a><span data-ttu-id="18702-156">Zie ook</span><span class="sxs-lookup"><span data-stu-id="18702-156">See Also</span></span>
[<span data-ttu-id="18702-157">Resources toewijzen</span><span class="sxs-lookup"><span data-stu-id="18702-157">Allocate Resources</span></span>](service-how-to-allocate-resources.md)  
[<span data-ttu-id="18702-158">Service- en werkuren instellen</span><span class="sxs-lookup"><span data-stu-id="18702-158">Set Up Work Hours and Service Hours</span></span>](service-how-setup-work-service-hours.md)  
[<span data-ttu-id="18702-159">Foutrapportage instellen</span><span class="sxs-lookup"><span data-stu-id="18702-159">Set Up Fault Reporting</span></span>](service-how-setup-fault-reporting.md)  
[<span data-ttu-id="18702-160">Codes voor standaardservices instellen</span><span class="sxs-lookup"><span data-stu-id="18702-160">Set Up Codes for Standard Services</span></span>](service-how-setup-service-coding.md)  
 



[!INCLUDE[footer-include](includes/footer-banner.md)]