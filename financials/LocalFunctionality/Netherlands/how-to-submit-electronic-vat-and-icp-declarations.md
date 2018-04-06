---
title: Elektronische btw- en ICP-aangiften verzenden
description: Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden. Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd in het venster Elek. aangifte-instellingen.
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
ms.openlocfilehash: d02d7f96957a31f9891f38660a256c71d89fdab1
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="submit-electronic-vat-and-icp-declarations"></a><span data-ttu-id="c1cf8-104">Elektronische btw- en ICP-aangiften verzenden</span><span class="sxs-lookup"><span data-stu-id="c1cf8-104">Submit Electronic VAT and ICP Declarations</span></span>
<span data-ttu-id="c1cf8-105">Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-105">With the eXtensible Business Reporting Language (XBRL) reporter, you can submit the Intracommunautaire Leveringen (ICP) declaration or the VAT declaration in the required XML format.</span></span> <span data-ttu-id="c1cf8-106">Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd in het venster Elek. aangifte-instellingen.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-106">When it is submitted, the file is sent to the tax authorities as defined in the Elec. Tax Declaration Setup Window.</span></span>  

<span data-ttu-id="c1cf8-107">De XBRL Reporter zorgt ervoor dat alle rekeningnummers die worden geïmporteerd van [!INCLUDE[d365fin](../../includes/d365fin_md.md)], aan de XBRL-elementen in een rapport worden toegewezen.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-107">The XBRL reporter ensures that all account numbers that are imported from [!INCLUDE[d365fin](../../includes/d365fin_md.md)] are mapped to the XBRL elements in a report.</span></span> <span data-ttu-id="c1cf8-108">De XBRL Reporter geeft ook een lijst weer met fouten wegens niet-toegewezen elementen of rekeningen.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-108">The XBRL reporter also displays a list of errors of unmapped elements or accounts.</span></span>  

<span data-ttu-id="c1cf8-109">Als u elektronische btw- en ICP-aangiften naar de belastingdienst wilt sturen, voert u respectievelijk de batchverwerking **Elektronische btw-aangifte versturen** en **Elektronische ICP-aangifte versturen** uit.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-109">To submit electronic VAT and ICP declarations to the tax authorities, you can use the **Submit electronic VAT Declaration** batch job and **Submit electronic ICP Declaration** batch job, respectively.</span></span> <span data-ttu-id="c1cf8-110">Voordat de batchverwerking de elektronische aangifte naar de belastingdienst verzendt, wordt deze eerst ondertekend, gecomprimeerd en gecodeerd.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-110">The batch job will sign, compress, and encrypt the electronic declaration before submitting it to the tax authorities.</span></span>  

## <a name="to-submit-an-electronic-vat-or-icp-declaration"></a><span data-ttu-id="c1cf8-111">Een elektronische btw- of ICP-aangifte verzenden</span><span class="sxs-lookup"><span data-stu-id="c1cf8-111">To submit an electronic VAT or ICP declaration</span></span>  

1.  <span data-ttu-id="c1cf8-112">Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-112">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Elec. Tax Declarations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="c1cf8-113">Selecteer de elektronische aangifte die u wilt verzenden en kies de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-113">Select the electronic declaration that you want to submit, and then choose the **Edit** action.</span></span>  

    > [!NOTE]  
    >  <span data-ttu-id="c1cf8-114">U kunt alleen een elektronische aangifte verzenden die de status **Gemaakt** heeft.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-114">You can only submit an electronic declaration that has the status **Created**.</span></span> <span data-ttu-id="c1cf8-115">Voor meer informatie over de status van de elektronische aangifte, zie het veld Status.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-115">For more information about the status of the electronic declaration, see Status Field.</span></span>  

3.  <span data-ttu-id="c1cf8-116">Kies de actie **Elektronische aangifte versturen**.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-116">Choose the **Submit Electronic Tax Declaration** action.</span></span>  
4.  <span data-ttu-id="c1cf8-117">Vul de velden in zoals beschreven in de volgende tabel.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-117">Fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="c1cf8-118">Veld</span><span class="sxs-lookup"><span data-stu-id="c1cf8-118">Field</span></span>|<span data-ttu-id="c1cf8-119">Description</span><span class="sxs-lookup"><span data-stu-id="c1cf8-119">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="c1cf8-120">**PIN**</span><span class="sxs-lookup"><span data-stu-id="c1cf8-120">**PIN**</span></span>|<span data-ttu-id="c1cf8-121">Het unieke identificatienummer van het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-121">The personal identification number of the company.</span></span><br /><br /> <span data-ttu-id="c1cf8-122">U kunt alleen een waarde invoeren in dit veld als u het veld **Tekenmethode** op **PIN** hebt ingesteld in het venster **Elek. aangifte-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-122">You can enter a value in this field only if you have set the **Sign Method** field to **PIN** in the **Elec. Tax Declaration Setup** window.</span></span>|  
    |<span data-ttu-id="c1cf8-123">**Wachtwoord gebruikerscertificaat**</span><span class="sxs-lookup"><span data-stu-id="c1cf8-123">**User Certificate Password**</span></span>|<span data-ttu-id="c1cf8-124">Het wachtwoord dat gebruikt wordt om de gebruikerscertificaten te versleutelen.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-124">The password that will encrypt the user certificates.</span></span><br /><br /> <span data-ttu-id="c1cf8-125">U kunt alleen een waarde invoeren in dit veld als u het veld **Tekenmethode** op **PKI** hebt ingesteld in het venster **Elek. aangifte-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-125">You can enter a value in this field only if you have set the **Sign Method**  field to **PKI** in the **Elec. Tax Declaration Setup** window.</span></span>|  

5.  <span data-ttu-id="c1cf8-126">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-126">Choose the **OK** button.</span></span>  

<span data-ttu-id="c1cf8-127">De elektronische aangifte wordt verstuurd naar de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="c1cf8-127">The electronic declaration is submitted to the tax authorities.</span></span>  

## <a name="see-also"></a><span data-ttu-id="c1cf8-128">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c1cf8-128">See Also</span></span>  
[<span data-ttu-id="c1cf8-129">Lijsten met XBRL maken</span><span class="sxs-lookup"><span data-stu-id="c1cf8-129">Create Reports with XBRL</span></span>](../../bi-create-reports-with-xbrl.md)

