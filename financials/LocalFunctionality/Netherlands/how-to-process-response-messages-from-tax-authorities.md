---
title: Responsberichten van de belastingdienst verwerken
description: Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.
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
ms.openlocfilehash: b2e741b314579c371205748836a6d986b6e1d0af
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="process-response-messages-from-tax-authorities"></a><span data-ttu-id="43fdd-103">Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="43fdd-103">Process Response Messages from Tax Authorities</span></span>
<span data-ttu-id="43fdd-104">Als u een elektronische btw- of ICP-aangifte verzendt naar de belastingdienst, wordt de aangifte verwerkt en wordt u in reactie een bericht gestuurd.</span><span class="sxs-lookup"><span data-stu-id="43fdd-104">When you submit a VAT or ICP declaration to the tax authorities electronically, they will process the declaration and send you a message in response.</span></span>  

<span data-ttu-id="43fdd-105">U kunt de respons in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] importeren met de batchverwerking **Responsberichten ontvangen**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-105">You can import the response into [!INCLUDE[d365fin](../../includes/d365fin_md.md)] by using the **Receive Response Messages** batch job.</span></span> <span data-ttu-id="43fdd-106">Het responsbericht bevat de status van de aangifte.</span><span class="sxs-lookup"><span data-stu-id="43fdd-106">The response message will contain the status of the declaration.</span></span>  

## <a name="to-import-messages-from-the-tax-authorities-server"></a><span data-ttu-id="43fdd-107">Berichten importeren van de server van de belastingdienst</span><span class="sxs-lookup"><span data-stu-id="43fdd-107">To import messages from the tax authorities' server</span></span>  

1.  <span data-ttu-id="43fdd-108">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="43fdd-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Decl. Response Msgs.**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="43fdd-109">Kies de actie **Responsberichten ontvangen**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-109">Choose the **Receive Response Messages** action.</span></span>  
3.  <span data-ttu-id="43fdd-110">Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="43fdd-110">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="43fdd-111">Veld</span><span class="sxs-lookup"><span data-stu-id="43fdd-111">Field</span></span>|<span data-ttu-id="43fdd-112">Description</span><span class="sxs-lookup"><span data-stu-id="43fdd-112">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="43fdd-113">**Wachtwoord versleuteling CA-certificaat**</span><span class="sxs-lookup"><span data-stu-id="43fdd-113">**CA Certificate Encryption Password**</span></span>|<span data-ttu-id="43fdd-114">Het wachtwoord dat is gebruikt wordt om de CA-certificaten te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="43fdd-114">The password that was used to encrypt the Certificate Authorities' certificates.</span></span>|  
    |<span data-ttu-id="43fdd-115">**Wachtwoord gebruikerscertificaat**</span><span class="sxs-lookup"><span data-stu-id="43fdd-115">**User Certificate Password**</span></span>|<span data-ttu-id="43fdd-116">Het wachtwoord dat gebruikt wordt om de gebruikerscertificaten te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="43fdd-116">The password that is used to encrypt the user certificates.</span></span>|  

4.  <span data-ttu-id="43fdd-117">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-117">Choose the **OK** button.</span></span>  

## <a name="to-process-the-response-messages-from-the-tax-authorities"></a><span data-ttu-id="43fdd-118">Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="43fdd-118">To process the response messages from the tax authorities</span></span>  

1.  <span data-ttu-id="43fdd-119">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Responsberichten elektronische aangiften** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="43fdd-119">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Decl. Response Msgs.**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="43fdd-120">Kies de actie **Responsberichten verwerken**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-120">Choose the **Process Response Messages** action.</span></span>  
3.  <span data-ttu-id="43fdd-121">Selecteer in het venster **Batchverwerking Responsberichten verwerken** op het sneltabblad **Elek. aangifteresponsbericht** de juiste filters.</span><span class="sxs-lookup"><span data-stu-id="43fdd-121">In the **Process Response Messages Batch Job** window, on the **Elec. Tax Decl. Response Msg**. FastTab, select the appropriate filters.</span></span>  
4.  <span data-ttu-id="43fdd-122">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-122">Choose the **OK** button.</span></span>  

    <span data-ttu-id="43fdd-123">De verwerkte gegevens over het responsbericht wordt weergegeven in het **Responsberichten elektronische aangiften**</span><span class="sxs-lookup"><span data-stu-id="43fdd-123">The processed information about the response message is displayed in the **Elec. Tax Decl. Response Msgs.**.</span></span> <span data-ttu-id="43fdd-124">in.</span><span class="sxs-lookup"><span data-stu-id="43fdd-124">window.</span></span>  

5.  <span data-ttu-id="43fdd-125">Als u een bericht of bijlage wilt exporteren, kiest u op het tabblad **Responsbericht exporteren** de actie **Responsbijlage exporteren**.</span><span class="sxs-lookup"><span data-stu-id="43fdd-125">To export a message or attachment, choose the **Export Response Message** action or the **Export Response Attachment** action.</span></span>  

## <a name="see-also"></a><span data-ttu-id="43fdd-126">Zie ook</span><span class="sxs-lookup"><span data-stu-id="43fdd-126">See Also</span></span>  
 <span data-ttu-id="43fdd-127">[Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="43fdd-127">[Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md) </span></span>  
<span data-ttu-id="43fdd-128"><<<<<<< HEAD:financials/LocalFunctionality/Netherlands/how-to-process-response-messages-from-tax-authorities.md [Btw-categorieën instellen](how-to-set-up-vat-categories.md) </span><span class="sxs-lookup"><span data-stu-id="43fdd-128"><<<<<<< HEAD:financials/LocalFunctionality/Netherlands/how-to-process-response-messages-from-tax-authorities.md [Set Up VAT Categories](how-to-set-up-vat-categories.md) </span></span>  
 <span data-ttu-id="43fdd-129">[Elektronische btw- en ICP-aangiften maken](how-to-create-electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="43fdd-129">[Create Electronic VAT and ICP Declarations](how-to-create-electronic-vat-and-icp-declarations.md) </span></span>  
<span data-ttu-id="43fdd-130">=======
 [Btw-categorieën instellen](how-to-set-up-vat-categories.md) </span><span class="sxs-lookup"><span data-stu-id="43fdd-130">=======
 [Set Up VAT Categories](how-to-set-up-vat-categories.md) </span></span>  
 [<span data-ttu-id="43fdd-131">Elektronische btw- en ICP-aangiften maken</span><span class="sxs-lookup"><span data-stu-id="43fdd-131">Create Electronic VAT and ICP Declarations</span></span>](how-to-create-electronic-vat-and-icp-declarations.md)   
 
>>>>>>> <span data-ttu-id="43fdd-132">refs/remotes/origin/Update13:archive/LocalFunctionality/Netherlands/how-to-process-response-messages-from-tax-authorities.md</span><span class="sxs-lookup"><span data-stu-id="43fdd-132">refs/remotes/origin/Update13:archive/LocalFunctionality/Netherlands/how-to-process-response-messages-from-tax-authorities.md</span></span>

