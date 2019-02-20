---
title: Inkoopbedragen controleren
description: Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkooporderdocument, gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 1acac32a417f794801da50c866db2643ea0a4c2d
ms.openlocfilehash: 68e4c1b65de4a978a752ee3b0bbd87a724b340e0
ms.contentlocale: nl-nl
ms.lasthandoff: 01/22/2019

---
# <a name="check-purchase-amounts"></a><span data-ttu-id="9c9de-103">Inkoopbedragen controleren</span><span class="sxs-lookup"><span data-stu-id="9c9de-103">Check Purchase Amounts</span></span>
<span data-ttu-id="9c9de-104">Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkooporderdocument, gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels.</span><span class="sxs-lookup"><span data-stu-id="9c9de-104">Before posting a purchase invoice or credit memo, the program checks if the amount including VAT and the VAT amount stated on the purchase document is equal to the total amount of the inserted purchase lines.</span></span> <span data-ttu-id="9c9de-105">Hiervoor moeten de velden **Documentbedrag incl. btw** en **Btw documentbedrag** ingevuld zijn op de pagina **Inkoopfactuur** of **Inkoopcreditnota**.</span><span class="sxs-lookup"><span data-stu-id="9c9de-105">To do this, the **Doc. Amount Incl. VAT** and **Doc. Amount VAT** fields must be filled in in the **Purchase Invoice** or **Purchase Credit Memo** page.</span></span>  

 <span data-ttu-id="9c9de-106">Als er slechts één inkoopregel is of als alle regels vallen onder hetzelfde btw-percentage, wordt het juiste **Btw documentbedrag**-veld automatisch berekend wanneer u de inkoopregels en het veld **Documentbedrag incl. btw** hebt ingevoegd.</span><span class="sxs-lookup"><span data-stu-id="9c9de-106">In case there is only one purchase line or in case all lines are subject to the same VAT %, the correct **Doc. Amount VAT Field** will be calculated automatically when you have inserted the purchase lines and the **Doc. Amount Incl. VAT Field**.</span></span> <span data-ttu-id="9c9de-107">In het geval dat verschillende regels met verschillende btw-percentages bestaan, moet het veld **Documentbedrag incl. btw** handmatig worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="9c9de-107">In case several lines exist with different VAT percentages, the **Doc. Amount VAT Field** must be changed manually.</span></span>  

 <span data-ttu-id="9c9de-108">De totaalbedragen van het inkoopdocument worden standaard gecontroleerd, maar u kunt dit uitschakelen door het selectievakje **Totaalbedragen documenten controleren** op de pagina **Inkoopinstellingen** uit te schakelen.</span><span class="sxs-lookup"><span data-stu-id="9c9de-108">Default the program will check the purchase document total amounts, but you can switch it off by deselecting the **Check Doc. Total Amounts** check box on the **Purchases & Payables Setup** page.</span></span>  

 <span data-ttu-id="9c9de-109">Als u wilt weten waarom er een verschil is tussen de totaalbedragen van het document en de totaalbedragen van de ingevoegde inkoopregels, hebt u de mogelijkheid om het totaalbedrag, het totale basisbedrag, het totale btw-bedrag en het totaalbedrag inclusief btw van de ingevoegde inkoopregels te laten berekenen en deze onder aan de inkoopfactuur- of inkoopcreditnotapagina weer te geven.</span><span class="sxs-lookup"><span data-stu-id="9c9de-109">To determine the reason of the difference between the document total amounts and the total amounts of the inserted purchase lines, you have the possibility to let the program calculate the total amount, total base amount, total VAT amount and total amount including VAT of the inserted purchase lines and show them at the bottom of the purchase invoice or purchase credit memo page.</span></span>  

 <span data-ttu-id="9c9de-110">Deze totaalbedragen worden standaard niet weergegeven, maar u kunt dit inschakelen door het selectievakje **Totale op inkoopfactuur/CR-nota weergeven** in te schakelen</span><span class="sxs-lookup"><span data-stu-id="9c9de-110">Default the program will not show these total amounts, but you can switch it on by selecting the **Show Totals on Purch. Inv.-CM.**</span></span> <span data-ttu-id="9c9de-111">op de pagina **Inkoopinstellingen**.</span><span class="sxs-lookup"><span data-stu-id="9c9de-111">check box on the **Purchases & Payables Setup** page.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="9c9de-112">Als u dit veld activeert, moeten de totalen van alle inkoopfacturen en creditnota's worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="9c9de-112">If you activate this field, totals on all purchase invoices and credit memos must be recalculated.</span></span> <span data-ttu-id="9c9de-113">Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.</span><span class="sxs-lookup"><span data-stu-id="9c9de-113">This can be a time-consuming process depending on the number of documents that must be recalculated.</span></span> <span data-ttu-id="9c9de-114">U kunt dit veld niet activeren als er inkoopfacturen en/of creditnota's zijn zonder inkoopregels of als u inkoopfacturen en/of inkoopcreditnota's hebt waarbij geen aantal is opgegeven op de regels.</span><span class="sxs-lookup"><span data-stu-id="9c9de-114">You can not activate this field in case purchase invoices and/or credit memos exist without any purchase lines or in case you have purchase invoices and/or purchase credit memos with no quantity specified on the lines.</span></span>  

## <a name="see-also"></a><span data-ttu-id="9c9de-115">Zie ook</span><span class="sxs-lookup"><span data-stu-id="9c9de-115">See Also</span></span>  
 [<span data-ttu-id="9c9de-116">Validatie van inkoopbedragen instellen</span><span class="sxs-lookup"><span data-stu-id="9c9de-116">Set Up Validation of Purchase Amounts</span></span>](how-to-set-up-validation-of-purchase-amounts.md)

