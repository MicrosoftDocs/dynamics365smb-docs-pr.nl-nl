---
title: Records handmatig koppelen en synchroniseren | Microsoft Docs
description: Als een integratietabeltoewijzing wordt gesynchroniseerd, kunnen gegevens in alle records in een tabel in Business Central en Dynamics 365 Sales worden gesynchroniseerd die zijn gekoppeld.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: crm, sales, couple, decouple, synchronize
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: d8140f71709208a271eff5c8de415b0e95736072
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3911402"
---
# <a name="couple-and-synchronize-records-manually"></a><span data-ttu-id="b9029-103">Records handmatig koppelen en synchroniseren</span><span class="sxs-lookup"><span data-stu-id="b9029-103">Couple and Synchronize Records Manually</span></span>
<span data-ttu-id="b9029-104">In dit onderwerp wordt beschreven hoe u een of meer records in [!INCLUDE[d365fin](includes/d365fin_md.md)] koppelt aan records in Common Data Service of [!INCLUDE[crm_md](includes/crm_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b9029-104">This topic describes how to couple one or more records in [!INCLUDE[d365fin](includes/d365fin_md.md)] with records in Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="b9029-105">Door records te koppelen kunt u Common Data Service-informatie vanuit [!INCLUDE[d365fin](includes/d365fin_md.md)]bekijken en andersom.</span><span class="sxs-lookup"><span data-stu-id="b9029-105">Coupling records lets you view Common Data Service information from [!INCLUDE[d365fin](includes/d365fin_md.md)], and vice versa.</span></span> <span data-ttu-id="b9029-106">Door de koppeling kunt u ook gegevens synchroniseren tussen de records.</span><span class="sxs-lookup"><span data-stu-id="b9029-106">The coupling also enables you to synchronize data between the records.</span></span> <span data-ttu-id="b9029-107">U kunt bestaande records koppelen of nieuwe records maken en koppelen.</span><span class="sxs-lookup"><span data-stu-id="b9029-107">You can couple existing records, or create and couple new records.</span></span>

> [!Note]
> <span data-ttu-id="b9029-108">Gegevens koppelen en synchroniseren is alleen beschikbaar als de systeembeheerder een verbinding tussen [!INCLUDE[d365fin](includes/d365fin_md.md)] en Common Data Service of [!INCLUDE[crm_md](includes/crm_md.md)] heeft gemaakt.</span><span class="sxs-lookup"><span data-stu-id="b9029-108">Coupling and synchronizing data is available only if your system administrator has created a connection between [!INCLUDE[d365fin](includes/d365fin_md.md)] and Common Data Service or [!INCLUDE[crm_md](includes/crm_md.md)].</span></span> <span data-ttu-id="b9029-109">Een snelle manier om dat te controleren is de **Klant**-kaart te openen en de actie **Koppeling instellen** te zoeken.</span><span class="sxs-lookup"><span data-stu-id="b9029-109">A quick way to check is to open the **Customer** card and look for the **Set Up Coupling** action.</span></span> <span data-ttu-id="b9029-110">Als de actie beschikbaar is, zijn de apps verbonden.</span><span class="sxs-lookup"><span data-stu-id="b9029-110">If the action is available, the apps are connected.</span></span>   

## <a name="video-example"></a><span data-ttu-id="b9029-111">Videovoorbeeld</span><span class="sxs-lookup"><span data-stu-id="b9029-111">Video Example</span></span>

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098376]

## <a name="to-couple-a-record"></a><span data-ttu-id="b9029-112">Een record koppelen</span><span class="sxs-lookup"><span data-stu-id="b9029-112">To couple a record</span></span>  
1.  <span data-ttu-id="b9029-113">In [!INCLUDE[d365fin](includes/d365fin_md.md)] opent u de kaart voor de record die moeten worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="b9029-113">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="b9029-114">Bijvoorbeeld de klant- of contactkaart.</span><span class="sxs-lookup"><span data-stu-id="b9029-114">For example, the Customer or Contact card.</span></span>  

    <span data-ttu-id="b9029-115">U kunt ook slechts de lijstpagina openen en de record selecteren die u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="b9029-115">You can also just open the list page and select the record that you want to couple.</span></span>  

2.  <span data-ttu-id="b9029-116">Kies de actie **Koppeling instellen**.</span><span class="sxs-lookup"><span data-stu-id="b9029-116">Choose the **Set Up Coupling** action.</span></span>  
3.  <span data-ttu-id="b9029-117">Vul de velden in en kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9029-117">Fill in the fields, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record"></a><span data-ttu-id="b9029-118">Eén record synchroniseren</span><span class="sxs-lookup"><span data-stu-id="b9029-118">To synchronize a single record</span></span>  
1.  <span data-ttu-id="b9029-119">In [!INCLUDE[d365fin](includes/d365fin_md.md)] opent u de kaart voor de record die moeten worden gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="b9029-119">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the card for the record you want to couple.</span></span> <span data-ttu-id="b9029-120">Bijvoorbeeld de klant- of contactkaart.</span><span class="sxs-lookup"><span data-stu-id="b9029-120">For example, the Customer or Contact card.</span></span>  
2.  <span data-ttu-id="b9029-121">Kies de actie **Nu synchroniseren**.</span><span class="sxs-lookup"><span data-stu-id="b9029-121">Choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="b9029-122">Als een record in één richting kan worden gesynchroniseerd, selecteert u de optie die de richting van de gegevensupdate opgeeft, en kiest u vervolgens **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9029-122">If a record can be synchronized in one direction, select the option that specifies the direction of data update, and then choose **OK**.</span></span>  

## <a name="to-synchronize-a-single-record-from-crm_md"></a><span data-ttu-id="b9029-123">Eén record synchroniseren vanuit [!INCLUDE[crm_md](includes/crm_md.md)]</span><span class="sxs-lookup"><span data-stu-id="b9029-123">To synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)]</span></span>  
1.  <span data-ttu-id="b9029-124">In [!INCLUDE[crm_md](includes/crm_md.md)] opent u het formulier voor de record die u wilt koppelen.</span><span class="sxs-lookup"><span data-stu-id="b9029-124">In [!INCLUDE[crm_md](includes/crm_md.md)], open the form for the record you want to couple.</span></span> <span data-ttu-id="b9029-125">Bijvoorbeeld het formulier Accountkaart of Contactkaart.</span><span class="sxs-lookup"><span data-stu-id="b9029-125">For example, the Account card or Contact card form.</span></span>  
2.  <span data-ttu-id="b9029-126">Kies de actie **[!INCLUDE[d365fin](includes/d365fin_md.md)]** op het lint om een record automatisch te openen en te koppelen.</span><span class="sxs-lookup"><span data-stu-id="b9029-126">Choose the **[!INCLUDE[d365fin](includes/d365fin_md.md)]** action in the ribbon to open and couple record automatically.</span></span>

> [!Note]
> <span data-ttu-id="b9029-127">U kunt één record alleen automatisch synchroniseren vanuit [!INCLUDE[crm_md](includes/crm_md.md)] wanneer **Alleen gekoppelde records synchr.** is uitgeschakeld en de synchronisatierichting is ingesteld op Bidirectioneel of Van integratietabel op de pagina **Toewijzing van integratietabel** voor de record.</span><span class="sxs-lookup"><span data-stu-id="b9029-127">You can synchronize a single record from [!INCLUDE[crm_md](includes/crm_md.md)] automatically only when **Sync. Only Coupled Records** is disabled and the synchronization direction is set to Bidirectional or From Integration Table on the **Integration Table Mapping** page for the record.</span></span> <span data-ttu-id="b9029-128">Zie voor meer informatie [De tabellen en velden toewijzen voor synchronisatie](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span><span class="sxs-lookup"><span data-stu-id="b9029-128">For more information, see [Mapping the Tables and Fields to Synchronize](admin-how-to-modify-table-mappings-for-synchronization.md#creating-new-records).</span></span>     

## <a name="to-synchronize-multiple-records"></a><span data-ttu-id="b9029-129">Meerdere records synchroniseren</span><span class="sxs-lookup"><span data-stu-id="b9029-129">To synchronize multiple records</span></span>  
1.  <span data-ttu-id="b9029-130">Open in [!INCLUDE[d365fin](includes/d365fin_md.md)] de lijstpagina voor de record, zoals lijstpagina Klanten of Contact.</span><span class="sxs-lookup"><span data-stu-id="b9029-130">In [!INCLUDE[d365fin](includes/d365fin_md.md)], open the list page for the record, such as the Customers or Contacts list pages.</span></span>  
2.  <span data-ttu-id="b9029-131">Selecteer de records die u wilt synchroniseren en kies vervolgens de actie **Nu synchroniseren**.</span><span class="sxs-lookup"><span data-stu-id="b9029-131">Select the records that you want to synchronize, and then choose the **Synchronize Now** action.</span></span>  
3.  <span data-ttu-id="b9029-132">Als records in één richting kunnen worden gesynchroniseerd, selecteert u de optie die de richting opgeeft, en kiest u vervolgens **OK**.</span><span class="sxs-lookup"><span data-stu-id="b9029-132">If records can be synchronized in one direction, select the option that specifies the direction, and then choose **OK**.</span></span>  

## <a name="see-also"></a><span data-ttu-id="b9029-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b9029-133">See Also</span></span>  
[<span data-ttu-id="b9029-134">Microsoft Dynamics 365 Sales gebruiken vanuit Business Central</span><span class="sxs-lookup"><span data-stu-id="b9029-134">Using Dynamics 365 Sales from Business Central</span></span>](marketing-integrate-dynamicscrm.md)
