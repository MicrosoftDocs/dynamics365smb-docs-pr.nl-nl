---
title: Kosten rapporteren en afstemmen met het grootboek | Microsoft Docs
description: Aan het einde van boekhoudperioden (maandelijks, jaarlijks of anderszins) moet een reeks kostenbeheersings- en audittaken worden uitgevoerd om een juiste en gebalanceerde voorraadwaarde te rapporteren aan de financiële afdeling. Naast de boekingsroutine waarmee de afzonderlijke artikelwaardeposten worden overgebracht naar speciale grootboekrekeningen, zijn diverse lijsten, traceerfuncties en een speciaal reconciliatiehulpmiddel beschikbaar voor de auditor of controller die verantwoordelijk is voor dit bedrijfskritieke werk.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 1b2a83ddbac54d5034b043c3124f698613be4642
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "794901"
---
# <a name="reporting-costs-and-reconciling-with-the-general-ledger"></a><span data-ttu-id="7039a-104">Kosten rapporteren en afstemmen met het grootboek</span><span class="sxs-lookup"><span data-stu-id="7039a-104">Reporting Costs and Reconciling with the General Ledger</span></span>
<span data-ttu-id="7039a-105">Aan het einde van boekhoudperioden (maandelijks, jaarlijks of anderszins) moet een reeks kostenbeheersings- en audittaken worden uitgevoerd om een juiste en gebalanceerde voorraadwaarde te rapporteren aan de financiële afdeling.</span><span class="sxs-lookup"><span data-stu-id="7039a-105">At the end of accounting periods, monthly, yearly or other, a sequence of cost control and auditing tasks must be performed to report a correct and balanced inventory value to the finance department.</span></span> <span data-ttu-id="7039a-106">Naast de boekingsroutine waarmee de afzonderlijke artikelwaardeposten worden overgebracht naar speciale grootboekrekeningen, zijn diverse lijsten, traceerfuncties en een speciaal reconciliatiehulpmiddel beschikbaar voor de auditor of controller die verantwoordelijk is voor dit bedrijfskritieke werk.</span><span class="sxs-lookup"><span data-stu-id="7039a-106">Apart from the posting routine that transfers the individual item value entries to dedicated general ledger accounts, several reports, tracing functions, and a special reconciliation tool are available to the auditor or controller responsible for this business-critical work.</span></span>  

 <span data-ttu-id="7039a-107">In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.</span><span class="sxs-lookup"><span data-stu-id="7039a-107">The following table describes a sequence of tasks, with links to the topics that describe them.</span></span>   

|<span data-ttu-id="7039a-108">**Als u dit wilt doen**</span><span class="sxs-lookup"><span data-stu-id="7039a-108">**To**</span></span>|<span data-ttu-id="7039a-109">**Zie**</span><span class="sxs-lookup"><span data-stu-id="7039a-109">**See**</span></span>|  
|------------|-------------|  
|<span data-ttu-id="7039a-110">De voorraadwaarde van geselecteerde artikelen te bekijken, inclusief informatie over de hoeveelheden en waarden van toenames en afnames van de voorraad in een geselecteerde periode.</span><span class="sxs-lookup"><span data-stu-id="7039a-110">View the inventory value of selected items, including information about the quantities and values of increases and decreases in inventory over a selected period.</span></span>|<span data-ttu-id="7039a-111">Rapport **Voorraadwaardering**</span><span class="sxs-lookup"><span data-stu-id="7039a-111">**Inventory Valuation** report</span></span>|  
|<span data-ttu-id="7039a-112">De voorraadwaarde te bekijken van geselecteerde productieorders in uw OHW-voorraad (onderhanden werk), zoals de hoeveelheden en waarden van verbruik, capaciteitgebruik en output in lopende productieorders.</span><span class="sxs-lookup"><span data-stu-id="7039a-112">View the inventory value of selected production orders in your WIP (work in process) inventory, such as the quantities and values of consumption, capacity usage, and output in ongoing production orders.</span></span>|<span data-ttu-id="7039a-113">Rapport **Voorraadwaardering - OHW**</span><span class="sxs-lookup"><span data-stu-id="7039a-113">**Inventory Valuation - WIP** report</span></span>|  
|<span data-ttu-id="7039a-114">De voorraadwaarde te bekijken van geselecteerde artikelen, inclusief de werkelijke en verwachte kostprijs op de gespecificeerde datum.</span><span class="sxs-lookup"><span data-stu-id="7039a-114">View the inventory value of selected items, including their actual and expected cost on the date specified.</span></span>|<span data-ttu-id="7039a-115">Rapport **Voorraadwaard. - Kostenspec.**</span><span class="sxs-lookup"><span data-stu-id="7039a-115">**Invt. Valuation - Cost Spec.** report</span></span>|  
|<span data-ttu-id="7039a-116">Een lijst te gebruiken om de redenen voor kostenvariaties te analyseren of om inzicht te krijgen in de kostenaandelen van verkochte goederen (KPV).</span><span class="sxs-lookup"><span data-stu-id="7039a-116">Use a report to analyze the reasons for cost variances or to gain insight into the cost shares of sold items (COGS).</span></span>|<span data-ttu-id="7039a-117">Rapport **Analyse aandeel in kosten**</span><span class="sxs-lookup"><span data-stu-id="7039a-117">**Cost Shares Breakdown** report</span></span>|  
|<span data-ttu-id="7039a-118">De waardeposten van artikeltransacties periodiek te boeken van voorraadgrootboek naar de gerelateerde grootboekrekeningen om de twee grootboeken in overeenstemming te brengen.</span><span class="sxs-lookup"><span data-stu-id="7039a-118">Periodically post the value entries of item transactions from the inventory ledger to the related G/L accounts to reconcile the two ledgers.</span></span>|[<span data-ttu-id="7039a-119">Voorraadkosten reconciliëren met het grootboek</span><span class="sxs-lookup"><span data-stu-id="7039a-119">Reconcile Inventory Costs with the General Ledger</span></span>](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|<span data-ttu-id="7039a-120">Gebruik één pagina om de reconciliatie tussen het voorraadgrootboek en het grootboek te controleren.</span><span class="sxs-lookup"><span data-stu-id="7039a-120">Use one page to audit the reconciliation between the inventory ledger and the general ledger.</span></span>|[<span data-ttu-id="7039a-121">Voorraadkosten reconciliëren met het grootboek</span><span class="sxs-lookup"><span data-stu-id="7039a-121">Reconcile Inventory Costs with the General Ledger</span></span>](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|<span data-ttu-id="7039a-122">Het OHW-bedrag te bepalen dat geboekt moet worden naar balansrekeningen voor eindrapportage van een periode.</span><span class="sxs-lookup"><span data-stu-id="7039a-122">Determine the WIP amount that needs to be posted to balance sheet accounts for period-end reporting.</span></span>|[<span data-ttu-id="7039a-123">Voortgang en prestaties van projecten bewaken</span><span class="sxs-lookup"><span data-stu-id="7039a-123">Monitor Job Progress and Performance</span></span>](projects-how-monitor-progress-performance.md)|

## <a name="see-also"></a><span data-ttu-id="7039a-124">Zie ook</span><span class="sxs-lookup"><span data-stu-id="7039a-124">See Also</span></span>  
[<span data-ttu-id="7039a-125">Voorraadwaardering en kostprijsberekening instellen</span><span class="sxs-lookup"><span data-stu-id="7039a-125">Setting Up Inventory Valuation and Costing</span></span>](finance-set-up-inventory-valuation-and-costing.md)  
[<span data-ttu-id="7039a-126">Voorraadkosten beheren</span><span class="sxs-lookup"><span data-stu-id="7039a-126">Managing Inventory Costs</span></span>](finance-manage-inventory-costs.md)  
[<span data-ttu-id="7039a-127">Financiën</span><span class="sxs-lookup"><span data-stu-id="7039a-127">Finance</span></span>](finance.md)  
<span data-ttu-id="7039a-128">[Voorraad](inventory-manage-inventory.md) </span><span class="sxs-lookup"><span data-stu-id="7039a-128">[Inventory](inventory-manage-inventory.md) </span></span>  
<span data-ttu-id="7039a-129">[Verkoop](sales-manage-sales.md) </span><span class="sxs-lookup"><span data-stu-id="7039a-129">[Sales](sales-manage-sales.md) </span></span>  
[<span data-ttu-id="7039a-130">Inkoop</span><span class="sxs-lookup"><span data-stu-id="7039a-130">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="7039a-131">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="7039a-131">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>