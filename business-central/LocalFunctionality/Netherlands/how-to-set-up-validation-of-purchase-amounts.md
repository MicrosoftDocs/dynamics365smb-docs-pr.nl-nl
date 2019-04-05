---
title: Validatie van inkoopbedragen instellen
description: In Business Central kunt u de functie Totaalbedragen documenten controleren activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 38fbf38851c788c850fec9d6cd656829b6554f33
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "826911"
---
# <a name="set-up-validation-of-purchase-amounts"></a><span data-ttu-id="ec29f-103">Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="ec29f-103">Set Up Validation of Purchase Amounts</span></span>
<span data-ttu-id="ec29f-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="ec29f-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can activate the **Check Doc. Total Amounts** function to validate the total amount of purchase documents before posting a purchase invoice and purchase credit memo.</span></span> <span data-ttu-id="ec29f-105">Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt.</span><span class="sxs-lookup"><span data-stu-id="ec29f-105">By default, the purchase document total amount is validated when you post.</span></span> <span data-ttu-id="ec29f-106">Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag.</span><span class="sxs-lookup"><span data-stu-id="ec29f-106">The total amount of the inserted purchase lines must be equal to the amount including VAT and the VAT amount.</span></span> <span data-ttu-id="ec29f-107">Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag op de pagina **Inkoopfactuur** of **Inkoopcreditnota** invoeren.</span><span class="sxs-lookup"><span data-stu-id="ec29f-107">To validate the purchase document amount automatically, you must enter the document amount including VAT and the document amount VAT in the **Purchase Invoice** or **Purchase Credit Memo** page.</span></span>  

<span data-ttu-id="ec29f-108">Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt.</span><span class="sxs-lookup"><span data-stu-id="ec29f-108">If you have only one purchase line or several purchase lines with the same VAT percentage, the correct document amount VAT is calculated automatically when you insert the purchase lines and the document amount including VAT.</span></span> <span data-ttu-id="ec29f-109">Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="ec29f-109">If you have several purchase lines with different VAT percentages, the document amount VAT value must be changed manually.</span></span>  

<span data-ttu-id="ec29f-110">U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen.</span><span class="sxs-lookup"><span data-stu-id="ec29f-110">You can also locate when the document total amounts and the total amounts of the inserted purchase lines are different.</span></span> <span data-ttu-id="ec29f-111">U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven**</span><span class="sxs-lookup"><span data-stu-id="ec29f-111">You can activate the **Show Totals on Purch. Inv./CM.**</span></span> <span data-ttu-id="ec29f-112">activeren om het volgende weer te geven in de ingevoegde inkoopregels:</span><span class="sxs-lookup"><span data-stu-id="ec29f-112">option to view the following in the inserted purchase lines:</span></span>  

- <span data-ttu-id="ec29f-113">Totaalbedrag</span><span class="sxs-lookup"><span data-stu-id="ec29f-113">Total amount</span></span>  
- <span data-ttu-id="ec29f-114">Totaalbasisbedrag</span><span class="sxs-lookup"><span data-stu-id="ec29f-114">Total base amount</span></span>  
- <span data-ttu-id="ec29f-115">Totaal btw-bedrag</span><span class="sxs-lookup"><span data-stu-id="ec29f-115">Total VAT amount</span></span>  
- <span data-ttu-id="ec29f-116">Totaalbedrag incl. btw</span><span class="sxs-lookup"><span data-stu-id="ec29f-116">Total amount including VAT</span></span>  

<span data-ttu-id="ec29f-117">De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota.</span><span class="sxs-lookup"><span data-stu-id="ec29f-117">The calculated amounts are displayed in the purchase invoice or purchase credit memo.</span></span> <span data-ttu-id="ec29f-118">Standaard wordt dit totaalbedrag niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="ec29f-118">By default, this total amount is not displayed.</span></span>  

<span data-ttu-id="ec29f-119">U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:</span><span class="sxs-lookup"><span data-stu-id="ec29f-119">You can activate this option only if the purchase invoice or purchase credit memo has:</span></span>  

- <span data-ttu-id="ec29f-120">Een minimum van één inkoopregel.</span><span class="sxs-lookup"><span data-stu-id="ec29f-120">A minimum of one purchase line.</span></span>  
- <span data-ttu-id="ec29f-121">Het aantalveld opgegeven.</span><span class="sxs-lookup"><span data-stu-id="ec29f-121">The quantity field specified.</span></span>  

## <a name="to-set-up-validation-of-total-amounts-for-purchase-documents"></a><span data-ttu-id="ec29f-122">Validatie van totaalbedragen voor inkoopdocumenten instellen</span><span class="sxs-lookup"><span data-stu-id="ec29f-122">To set up validation of total amounts for purchase documents</span></span>  

1.  <span data-ttu-id="ec29f-123">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="ec29f-123">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="ec29f-124">Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="ec29f-124">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="ec29f-125">Veld</span><span class="sxs-lookup"><span data-stu-id="ec29f-125">Field</span></span>|<span data-ttu-id="ec29f-126">Description</span><span class="sxs-lookup"><span data-stu-id="ec29f-126">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="ec29f-127">**Totale op inkoopfactuur/CR-nota weergeven.**</span><span class="sxs-lookup"><span data-stu-id="ec29f-127">**Show Totals on Purch. Inv./CM.**</span></span>|<span data-ttu-id="ec29f-128">Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's.</span><span class="sxs-lookup"><span data-stu-id="ec29f-128">Select to recalculate the totals on all purchase invoices and credit memos.</span></span> <span data-ttu-id="ec29f-129">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="ec29f-129">This can take more time depending on the number of documents that must be recalculated.</span></span>|  
    |<span data-ttu-id="ec29f-130">**Totaalbedragen documenten controleren**</span><span class="sxs-lookup"><span data-stu-id="ec29f-130">**Check Doc. Total Amounts**</span></span>|<span data-ttu-id="ec29f-131">Selecteer om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** op de pagina's **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="ec29f-131">Select to modify the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields in the **Purchase Invoice** and **Purchase Credit Memo** pages.</span></span>|  

3.  <span data-ttu-id="ec29f-132">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="ec29f-132">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="ec29f-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="ec29f-133">See Also</span></span>  
[<span data-ttu-id="ec29f-134">Nederlandse lokale functionaliteit</span><span class="sxs-lookup"><span data-stu-id="ec29f-134">Netherlands Local Functionality</span></span>](netherlands-local-functionality.md)  
[<span data-ttu-id="ec29f-135">Inkopen instellen</span><span class="sxs-lookup"><span data-stu-id="ec29f-135">Setting Up Purchases</span></span>](../../sales-how-work-standard-lines.md)
