---
title: Inkomende documenten instellen| Microsoft Docs
description: Gebruik de functie inkomende documenten om elektronische documenten te maken, OCR-taken te beheren, facturen te importeren en afbeeldingsbestanden te converteren.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, e-invoice, incoming document, OCR, ecommerce, document exchange, import invoice
ms.date: 06/02/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 6381fc0949c3f6789a6b3387d119051403bcbb4a
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="set-up-incoming-documents"></a><span data-ttu-id="09b94-103">Inkomende documenten instellen</span><span class="sxs-lookup"><span data-stu-id="09b94-103">Set Up Incoming Documents</span></span>
<span data-ttu-id="09b94-104">Als u dagboekregels van inkomende documentrecords maakt, moet u in het venster **Instellingen van inkomende documenten** vastleggen welke dagboeksjabloon en batch moeten worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="09b94-104">If you create general journal lines from incoming document records, you must specify in the **Incoming Documents Setup** window which journal template and batch to use.</span></span>

<span data-ttu-id="09b94-105">Als u niet wilt dat gebruikers facturen of dagboekregels maken van inkomende documentrecords, tenzij de documenten zijn goedgekeurd, moet u fiatteurs instellen in het venster **Fiatteurs inkomende documenten**.</span><span class="sxs-lookup"><span data-stu-id="09b94-105">If you do not want users to create invoices or general journal lines from incoming document records unless the documents are first approved, you must set up approvers in the **Incoming Document Approvers** window.</span></span>

<span data-ttu-id="09b94-106">Als u PDF- en afbeeldingsbestanden naar elektronische documenten wilt omzetten waarnaar u kunt converteren, bijvoorbeeld inkoopfacturen in [!INCLUDE[d365fin](includes/d365fin_md.md)], moet u eerst de OCR-functie instellen en de service inschakelen.</span><span class="sxs-lookup"><span data-stu-id="09b94-106">To turn PDF and image files into electronic documents that you can convert to, for example, purchase invoices inside [!INCLUDE[d365fin](includes/d365fin_md.md)], you must first set up the OCR feature and enable the service.</span></span>

<span data-ttu-id="09b94-107">Wanneer de functie Inkomende documenten is ingesteld, kunt u verschillende functies gebruiken om onkostenbewijzen te controleren, OCR-taken te beheren en inkomende documentbestanden handmatig of automatisch te converteren naar de relevante documenten of dagboekregels.</span><span class="sxs-lookup"><span data-stu-id="09b94-107">When the Incoming Documents feature is set up, you can use different functions to review expense receipts, manage OCR tasks, and convert incoming document files, manually or automatically, to the relevant documents or journal lines.</span></span> <span data-ttu-id="09b94-108">De externe bestanden kunnen worden gekoppeld in elke procesfase, inclusief naar geboekte documenten en naar de resulterende leverancier, klant en grootboekposten.</span><span class="sxs-lookup"><span data-stu-id="09b94-108">The external files can be attached at any process stage, including to posted documents and to the resulting vendor, customer, and general ledger entries.</span></span> <span data-ttu-id="09b94-109">Zie [Inkomende documenten verwerken](across-process-income-documents.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="09b94-109">For more information, see [Processing Incoming Documents](across-process-income-documents.md).</span></span>

## <a name="to-set-up-the-incoming-documents-feature"></a><span data-ttu-id="09b94-110">De functie Inkomende documenten instellen</span><span class="sxs-lookup"><span data-stu-id="09b94-110">To set up the Incoming Documents feature</span></span>
1. <span data-ttu-id="09b94-111">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen inkomende documenten** en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="09b94-111">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="09b94-112">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="09b94-112">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-set-up-approvers-of-incoming-document-records"></a><span data-ttu-id="09b94-113">Fiatteurs van inkomende documentrecords instellen</span><span class="sxs-lookup"><span data-stu-id="09b94-113">To set up approvers of incoming document records</span></span>
1. <span data-ttu-id="09b94-114">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen inkomende documenten** en klik op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="09b94-114">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Incoming Document Setup**, and then choose the related link.</span></span>  
2. <span data-ttu-id="09b94-115">Kies in het venster **Instellingen van inkomende documenten** de actie **Fiatteurs**.</span><span class="sxs-lookup"><span data-stu-id="09b94-115">In the **Incoming Documents Setup** window, choose the **Approvers** action.</span></span>

    <span data-ttu-id="09b94-116">Het venster **Fiatteurs inkomende documenten** bevat alle gebruikers die zijn ingesteld in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="09b94-116">The **Incoming Document Approvers** window shows all users that are set up in [!INCLUDE[d365fin](includes/d365fin_md.md)].</span></span>  
3. <span data-ttu-id="09b94-117">Selecteer een of meer gebruikers die een inkomend document kunnen goedkeuren voordat een verwant document of verwante dagboekregel kan worden gemaakt.</span><span class="sxs-lookup"><span data-stu-id="09b94-117">Select one or more users that can approve an incoming document before a related document or journal line can be created.</span></span>

<span data-ttu-id="09b94-118">Wanneer fiatteurs zijn ingesteld in het venster **Fiatteurs inkomende documenten**, kunnen alleen die gebruikers een inkomend document goedkeuren als het selectievakje **Goedkeuring vereist voor maken** is ingeschakeld in het venster **Instellingen inkomende documenten**.</span><span class="sxs-lookup"><span data-stu-id="09b94-118">When approvers have been set up in the **Incoming Document Approvers** window, only those users can approve an incoming document if the **Require Approval To Create** check box in the **Incoming Documents Setup** window is selected.</span></span>

> [!NOTE]  
>   <span data-ttu-id="09b94-119">Deze goedkeuringsinstellingen zijn niet gerelateerd aan goedkeuringswerkstromen.</span><span class="sxs-lookup"><span data-stu-id="09b94-119">This approval setup is not related to approval workflows.</span></span> <span data-ttu-id="09b94-120">Zie voor meer informatie [Goedkeuringswerkstromen gebruiken](across-how-use-approval-workflows.md).</span><span class="sxs-lookup"><span data-stu-id="09b94-120">For more information, see [Use Approval Workflows](across-how-use-approval-workflows.md).</span></span>

## <a name="to-set-up-an-ocr-service"></a><span data-ttu-id="09b94-121">Een OCR-service instellen</span><span class="sxs-lookup"><span data-stu-id="09b94-121">To set up an OCR service</span></span>
1. <span data-ttu-id="09b94-122">Klik op het pictogram ![Zoeken naar pagina of rapport](media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Instellingen van OCR-service** in en klik vervolgens op de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="09b94-122">Choose the ![Search for Page or Report](media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **OCR Service Setup**, and then choose the related link.</span></span>
2. <span data-ttu-id="09b94-123">Vul indien nodig de velden in.</span><span class="sxs-lookup"><span data-stu-id="09b94-123">Fill in the fields as necessary.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

## <a name="to-encrypt-your-login-information"></a><span data-ttu-id="09b94-124">Uw aanmeldgegevens versleutelen</span><span class="sxs-lookup"><span data-stu-id="09b94-124">To encrypt your login information</span></span>
<span data-ttu-id="09b94-125">We raden u aan de aanmeldgegevens te beveiligen die u invoert in het venster **Instellingen van OCR-service**.</span><span class="sxs-lookup"><span data-stu-id="09b94-125">It is recommended that you protect the logon information that you enter in the **OCR Service Setup** window.</span></span> <span data-ttu-id="09b94-126">U kunt gegevens op de server versleutelen door nieuwe encryptiesleutels te genereren of bestaande sleutels te importeren die u inschakelt op de serverinstantie die verbinding maakt met de database.</span><span class="sxs-lookup"><span data-stu-id="09b94-126">You can encrypt data on the server by generating new or importing existing encryption keys that you enable on the server instance that connects to the database.</span></span>

1. <span data-ttu-id="09b94-127">Kies in het venster **Instellingen van OCR-service** de actie **Versleutelingsbeheer**.</span><span class="sxs-lookup"><span data-stu-id="09b94-127">In the **OCR Service Setup** window, choose the **Encryption Management** action.</span></span>
2. <span data-ttu-id="09b94-128">Schakel in het venster **Beheer gegevensversleuteling** versleuteling van uw gegevens in.</span><span class="sxs-lookup"><span data-stu-id="09b94-128">In the **Data Encryption Management** window, enable encryption of your data.</span></span>

## <a name="see-also"></a><span data-ttu-id="09b94-129">Zie ook</span><span class="sxs-lookup"><span data-stu-id="09b94-129">See Also</span></span>
[<span data-ttu-id="09b94-130">Inkomende documenten verwerken</span><span class="sxs-lookup"><span data-stu-id="09b94-130">Process Incoming Documents</span></span>](across-process-income-documents.md)  
[<span data-ttu-id="09b94-131">Inkomende documenten</span><span class="sxs-lookup"><span data-stu-id="09b94-131">Incoming Documents</span></span>](across-income-documents.md)  
[<span data-ttu-id="09b94-132">Inkoop</span><span class="sxs-lookup"><span data-stu-id="09b94-132">Purchasing</span></span>](purchasing-manage-purchasing.md)  
<span data-ttu-id="09b94-133">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="09b94-133">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

