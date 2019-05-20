---
title: Validatie van inkoopbedragen instellen
description: In Business Central kunt u de functie Totaalbedragen documenten controleren activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: adeb99d6e35162c700ef446f74c6c89ba36f1d9f
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241773"
---
# <a name="set-up-validation-of-purchase-amounts"></a><span data-ttu-id="e07e4-103">Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="e07e4-103">Set Up Validation of Purchase Amounts</span></span>
<span data-ttu-id="e07e4-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.</span><span class="sxs-lookup"><span data-stu-id="e07e4-104">In [!INCLUDE[d365fin](../../includes/d365fin_md.md)], you can activate the **Check Doc. Total Amounts** function to validate the total amount of purchase documents before posting a purchase invoice and purchase credit memo.</span></span> <span data-ttu-id="e07e4-105">Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt.</span><span class="sxs-lookup"><span data-stu-id="e07e4-105">By default, the purchase document total amount is validated when you post.</span></span> <span data-ttu-id="e07e4-106">Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag.</span><span class="sxs-lookup"><span data-stu-id="e07e4-106">The total amount of the inserted purchase lines must be equal to the amount including VAT and the VAT amount.</span></span> <span data-ttu-id="e07e4-107">Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag op de pagina **Inkoopfactuur** of **Inkoopcreditnota** invoeren.</span><span class="sxs-lookup"><span data-stu-id="e07e4-107">To validate the purchase document amount automatically, you must enter the document amount including VAT and the document amount VAT in the **Purchase Invoice** or **Purchase Credit Memo** page.</span></span>  

<span data-ttu-id="e07e4-108">Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt.</span><span class="sxs-lookup"><span data-stu-id="e07e4-108">If you have only one purchase line or several purchase lines with the same VAT percentage, the correct document amount VAT is calculated automatically when you insert the purchase lines and the document amount including VAT.</span></span> <span data-ttu-id="e07e4-109">Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="e07e4-109">If you have several purchase lines with different VAT percentages, the document amount VAT value must be changed manually.</span></span>  

<span data-ttu-id="e07e4-110">U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen.</span><span class="sxs-lookup"><span data-stu-id="e07e4-110">You can also locate when the document total amounts and the total amounts of the inserted purchase lines are different.</span></span> <span data-ttu-id="e07e4-111">U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven**</span><span class="sxs-lookup"><span data-stu-id="e07e4-111">You can activate the **Show Totals on Purch. Inv./CM.**</span></span> <span data-ttu-id="e07e4-112">activeren om het volgende weer te geven in de ingevoegde inkoopregels:</span><span class="sxs-lookup"><span data-stu-id="e07e4-112">option to view the following in the inserted purchase lines:</span></span>  

- <span data-ttu-id="e07e4-113">Totaalbedrag</span><span class="sxs-lookup"><span data-stu-id="e07e4-113">Total amount</span></span>  
- <span data-ttu-id="e07e4-114">Totaalbasisbedrag</span><span class="sxs-lookup"><span data-stu-id="e07e4-114">Total base amount</span></span>  
- <span data-ttu-id="e07e4-115">Totaal btw-bedrag</span><span class="sxs-lookup"><span data-stu-id="e07e4-115">Total VAT amount</span></span>  
- <span data-ttu-id="e07e4-116">Totaalbedrag incl. btw</span><span class="sxs-lookup"><span data-stu-id="e07e4-116">Total amount including VAT</span></span>  

<span data-ttu-id="e07e4-117">De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota.</span><span class="sxs-lookup"><span data-stu-id="e07e4-117">The calculated amounts are displayed in the purchase invoice or purchase credit memo.</span></span> <span data-ttu-id="e07e4-118">Standaard wordt dit totaalbedrag niet weergegeven.</span><span class="sxs-lookup"><span data-stu-id="e07e4-118">By default, this total amount is not displayed.</span></span>  

<span data-ttu-id="e07e4-119">U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:</span><span class="sxs-lookup"><span data-stu-id="e07e4-119">You can activate this option only if the purchase invoice or purchase credit memo has:</span></span>  

- <span data-ttu-id="e07e4-120">Een minimum van één inkoopregel.</span><span class="sxs-lookup"><span data-stu-id="e07e4-120">A minimum of one purchase line.</span></span>  
- <span data-ttu-id="e07e4-121">Het aantalveld opgegeven.</span><span class="sxs-lookup"><span data-stu-id="e07e4-121">The quantity field specified.</span></span>  

## <a name="to-set-up-validation-of-total-amounts-for-purchase-documents"></a><span data-ttu-id="e07e4-122">Validatie van totaalbedragen voor inkoopdocumenten instellen</span><span class="sxs-lookup"><span data-stu-id="e07e4-122">To set up validation of total amounts for purchase documents</span></span>  

1.  <span data-ttu-id="e07e4-123">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Inkoopinstellingen** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="e07e4-123">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Purchases & Payables Setup**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="e07e4-124">Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="e07e4-124">On the **General** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="e07e4-125">Veld</span><span class="sxs-lookup"><span data-stu-id="e07e4-125">Field</span></span>|<span data-ttu-id="e07e4-126">Description</span><span class="sxs-lookup"><span data-stu-id="e07e4-126">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="e07e4-127">**Totale op inkoopfactuur/CR-nota weergeven.**</span><span class="sxs-lookup"><span data-stu-id="e07e4-127">**Show Totals on Purch. Inv./CM.**</span></span>|<span data-ttu-id="e07e4-128">Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's.</span><span class="sxs-lookup"><span data-stu-id="e07e4-128">Select to recalculate the totals on all purchase invoices and credit memos.</span></span> <span data-ttu-id="e07e4-129">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="e07e4-129">This can take more time depending on the number of documents that must be recalculated.</span></span>|  
    |<span data-ttu-id="e07e4-130">**Totaalbedragen documenten controleren**</span><span class="sxs-lookup"><span data-stu-id="e07e4-130">**Check Doc. Total Amounts**</span></span>|<span data-ttu-id="e07e4-131">Selecteer om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** op de pagina's **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="e07e4-131">Select to modify the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields in the **Purchase Invoice** and **Purchase Credit Memo** pages.</span></span>|  

3.  <span data-ttu-id="e07e4-132">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="e07e4-132">Choose the **OK** button.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e07e4-133">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e07e4-133">See Also</span></span>  
[<span data-ttu-id="e07e4-134">Nederlandse lokale functionaliteit</span><span class="sxs-lookup"><span data-stu-id="e07e4-134">Netherlands Local Functionality</span></span>](netherlands-local-functionality.md)  
[<span data-ttu-id="e07e4-135">Inkopen instellen</span><span class="sxs-lookup"><span data-stu-id="e07e4-135">Setting Up Purchases</span></span>](../../sales-how-work-standard-lines.md)
