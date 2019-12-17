---
title: Speciale documentlay-outs toewijzen aan klanten of leveranciers | Microsoft Docs
description: Wanneer aangepaste rapportlay-outs zijn gedefinieerd, kunt u deze selecteren uit klant- en leverancierskaarten om op te geven dat de geselecteerde lay-outs worden gebruikt voor verschillende soorten documenten die u voor de betreffende klant of leverancier maakt.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customized report, document layout, logo, personalize
ms.date: 11/15/2019
ms.author: sgroespe
ms.openlocfilehash: 23c4573c3121a660b8263c3bc9bb2c6ac8b1d331
ms.sourcegitcommit: 893e13fa75b2d04dedd4a29abda216e3e54b24ae
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/15/2019
ms.locfileid: "2809396"
---
# <a name="define-document-layouts-for-customers-and-vendors"></a><span data-ttu-id="2e552-103">Documentlay-outs definiëren voor klanten en leveranciers</span><span class="sxs-lookup"><span data-stu-id="2e552-103">Define Document Layouts for Customers and Vendors</span></span>
<span data-ttu-id="2e552-104">Wanneer aangepaste rapportlay-outs zijn gedefinieerd, kunt u deze selecteren uit klant- en leverancierskaarten om op te geven welke lay-outs worden gebruikt voor verschillende soorten documenten die u voor de betreffende klant of leverancier maakt.</span><span class="sxs-lookup"><span data-stu-id="2e552-104">When custom report layouts are defined, you can select them from customer and vendor cards to specify which layouts will be used for different types of documents that you crate for the customer or vendor in question.</span></span> <span data-ttu-id="2e552-105">De waarde in het veld **Gebruik** definieert voor welk proces de documentlay-out wordt gebruikt, zoals **Aanmaning**, **Verzending** en **Bevestiging**.</span><span class="sxs-lookup"><span data-stu-id="2e552-105">The value in the **Usage** field, defines which process the document layout will be used for, such as **Reminder**, **Shipment**, and **Confirmation**.</span></span>

<span data-ttu-id="2e552-106">Naast het instellen van de lay-outs die voor welk document moeten worden gebruikt, kunt u tijd besparen bij het verzenden van documenten naar verschillende klant- of leverancierscontacten door de e-mailadressen van specifieke contacten in te stellen voor gebruik met specifieke documenten.</span><span class="sxs-lookup"><span data-stu-id="2e552-106">In addition to setting up which layouts to use for what document, you can save time when sending documents to different customer or vendor contacts by setting up specific contacts' email addresses to use with specific documents.</span></span> <span data-ttu-id="2e552-107">Klantafschriften worden bijvoorbeeld verzonden naar accountantcontacten, verkooporders naar de kopers van uw klanten en inkooporders naar verkopers of accountmanagers van leveranciers.</span><span class="sxs-lookup"><span data-stu-id="2e552-107">For example, customer statements will be sent to accountant contacts, sales orders to your customers' purchasers, and purchase orders to vendors' salespeople or account managers.</span></span>

<span data-ttu-id="2e552-108">Wanneer u een documentlay-out definieert voor een klant of leverancier, kunt u ook het e-mailadres opgeven van de contactpersoon die het document moet ontvangen.</span><span class="sxs-lookup"><span data-stu-id="2e552-108">When you define a document layout for a customer or vendor, you can also specify the email address of the contact person that must receive the document.</span></span> <span data-ttu-id="2e552-109">U kunt dit snel doen met de functie **E-mail selecteren vanuit contacten**, die automatisch filtert op contact-e-mailadressen die zijn geregistreerd voor de betreffende klant of leverancier.</span><span class="sxs-lookup"><span data-stu-id="2e552-109">You can quickly do this with the **Select Email from Contacts** function, which automatically filters to contact email addresses registered for the customer or vendor in question.</span></span>

<span data-ttu-id="2e552-110">Voordat u kunt definiëren welke documentlay-out wordt gebruikt voor welke processen en naar welke contactpersoon het document moet worden verzonden, moet u alle beschikbare rapporten (documenten) laden vanaf de pagina **Selecties rapporteren**.</span><span class="sxs-lookup"><span data-stu-id="2e552-110">Before you can define which document layout to use for which processes, and which contact to send the document to, you must load all the available reports (documents) from the **Report Selections** page.</span></span> <span data-ttu-id="2e552-111">U kunt dit snel doen met de functie **Kopiëren uit rapportselectie**.</span><span class="sxs-lookup"><span data-stu-id="2e552-111">You can quickly do this with the **Copy from Report Selection** function.</span></span>

<span data-ttu-id="2e552-112">Hieronder wordt beschreven hoe u lay-outs van verkoopdocumenten vanaf een klantenkaart kunt definiëren.</span><span class="sxs-lookup"><span data-stu-id="2e552-112">The following describes how to define sales document layouts from a customer card.</span></span> <span data-ttu-id="2e552-113">De stappen zijn hetzelfde voor lay-outs voor inkoopdocumenten van een leverancierskaart.</span><span class="sxs-lookup"><span data-stu-id="2e552-113">The steps are the same for purchase document layouts from a vendor card.</span></span>

## <a name="to-enable-all-available-sales-documents-for-a-customer"></a><span data-ttu-id="2e552-114">Alle beschikbare verkoopdocumenten voor een klant inschakelen</span><span class="sxs-lookup"><span data-stu-id="2e552-114">To enable all available sales documents for a customer</span></span>
1. <span data-ttu-id="2e552-115">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Klanten** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="2e552-115">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Customers**, and then choose the related link.</span></span>
2. <span data-ttu-id="2e552-116">Open de kaart van de klant voor wie u documentlay-outs per bedrijfsproces wilt definiëren.</span><span class="sxs-lookup"><span data-stu-id="2e552-116">Open the card of the customer for whom you want to define document layouts per business process.</span></span>
3. <span data-ttu-id="2e552-117">Kies op de pagina **Klantenkaart** de pagina **Documentlay-outs**.</span><span class="sxs-lookup"><span data-stu-id="2e552-117">On the **Customer Card** page, choose the **Document Layouts** page.</span></span>
4. <span data-ttu-id="2e552-118">Kies op de pagina **Documentlay-outs** de actie **Kopiëren uit rapportselectie**.</span><span class="sxs-lookup"><span data-stu-id="2e552-118">On the **Document Layouts** page, choose the **Copy from Report Selection** action.</span></span>

<span data-ttu-id="2e552-119">De pagina **Documentlay-outs** voor de klant in kwestie is gevuld met alle rapportlay-outs voor verkoop die in het systeem bestaan.</span><span class="sxs-lookup"><span data-stu-id="2e552-119">The **Document Layouts** page for the customer in question is filled with all the report layouts for sales that exist in the system.</span></span> <span data-ttu-id="2e552-120">Zie voor meer informatie over hoe ze zijn gemaakt [Aangepaste rapportlay-outs maken en wijzigen](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="2e552-120">For more information about they were created, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

<span data-ttu-id="2e552-121">U kunt nu doorgaan met het aanpassen van de lijst met aangepaste rapportlay-outs of e-mailadressen voor de contactpersonen waarnaar de documenten moeten worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="2e552-121">You can now proceed to adjust the list with any custom report layouts or email addresses for the contacts that the documents must be sent to.</span></span>

## <a name="to-select-a-custom-report-layout-to-use-for-the-sales-document-layout"></a><span data-ttu-id="2e552-122">Een aangepaste rapportlay-out selecteren om te gebruiken voor de lay-out van het verkoopdocument</span><span class="sxs-lookup"><span data-stu-id="2e552-122">To select a custom report layout to use for the sales document layout</span></span>
<span data-ttu-id="2e552-123">Als voor een of meer van de rapportlay-outs die zijn gedefinieerd op de pagina **Documentlay-outs** voor de klant, geen aangepaste rapportlay-out is gedefinieerd, kunt u dat snel doen.</span><span class="sxs-lookup"><span data-stu-id="2e552-123">If one or more of the report layouts that are defined in the **Document Layouts** page for the customer do not have a custom report layout defined, then you can quickly do that.</span></span>

1. <span data-ttu-id="2e552-124">Kies op de pagina **Documentlay-outs** op de regel voor een rapportlay-out waarvoor u een aangepaste lay-out wilt gebruiken, het veld **Aangepaste lay-outbeschrijving**.</span><span class="sxs-lookup"><span data-stu-id="2e552-124">On the **Document Layouts** page, on the line for a report layout that you want to use a custom layout for, choose the **Custom Layout Description** field.</span></span> <span data-ttu-id="2e552-125">Het veld wordt ingevuld als de klantlay-out al is geselecteerd of leeg is.</span><span class="sxs-lookup"><span data-stu-id="2e552-125">The field is either filled if customer layout is already selected or blank.</span></span>
2. <span data-ttu-id="2e552-126">Selecteer op de pagina **Aangepaste rapportlay-outs** de speciale documentlay-out die u wilt gebruiken voor het betreffende verkoopdocumenttype.</span><span class="sxs-lookup"><span data-stu-id="2e552-126">On the **Custom Report Layouts** page, select the special document layout that you want to use for the sales document type in question.</span></span> <span data-ttu-id="2e552-127">Zie voor meer informatie [Aangepaste rapportlay-outs maken en wijzigen](ui-how-create-custom-report-layout.md).</span><span class="sxs-lookup"><span data-stu-id="2e552-127">For more information, see [Create and Modify Custom Report Layouts](ui-how-create-custom-report-layout.md).</span></span>

## <a name="to-set-up-which-contact-receives-which-document-layout-for-a-customer"></a><span data-ttu-id="2e552-128">Instellen welk contact welke documentlay-out voor een klant ontvangt</span><span class="sxs-lookup"><span data-stu-id="2e552-128">To set up which contact receives which document layout for a customer</span></span>
<span data-ttu-id="2e552-129">U kunt tijd besparen bij het verzenden van documenten naar verschillende klanten of contactpersonen van leveranciers door contact-e-mailadressen op te geven op de verschillende regels op de pagina **Documentlay-outs**.</span><span class="sxs-lookup"><span data-stu-id="2e552-129">You can save time when sending documents to different customers or vendor contacts by specifying contact email addresses on the different lines on the **Document Layouts** page.</span></span> <span data-ttu-id="2e552-130">Klantafschriften kunnen bijvoorbeeld worden verzonden naar accountantcontacten, verkooporders naar de kopers van uw klanten en inkooporders naar verkopers of accountmanagers van leveranciers.</span><span class="sxs-lookup"><span data-stu-id="2e552-130">For example, customer statements can be sent to accountant contacts, sales orders to your customers' purchasers, and purchase orders to vendors' salespeople or account managers.</span></span>

1. <span data-ttu-id="2e552-131">Kies op de pagina **Documentlay-outs** op de regel voor een rapportlay-out die u naar een specifiek contact voor de klant wilt verzenden, de actie **E-mail selecteren vanuit contacten**.</span><span class="sxs-lookup"><span data-stu-id="2e552-131">On the **Document Layouts** page, on the line for a report layout that you want to send to a specific contact for the customer, choose the **Select Email from Contacts** action.</span></span>
2. <span data-ttu-id="2e552-132">Selecteer op de pagina **Contacten** de regel voor het relevante contact en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="2e552-132">On the **Contacts** page, select the line for the relevant contact, and then choose the **OK** button.</span></span>

<span data-ttu-id="2e552-133">Het e-mailadres van de contactpersoon wordt nu ingevoegd op de documentlay-outregel, zodat het verkoopdocument in kwestie, bijvoorbeeld aanmaningen, altijd naar die contactpersoon in het bedrijf van de klant wordt verzonden.</span><span class="sxs-lookup"><span data-stu-id="2e552-133">The email address of the contact is now inserted on the document layout line so that the sales document in question, for example, reminders, is always sent to that contact at the customer's company.</span></span>

## <a name="see-also"></a><span data-ttu-id="2e552-134">Zie ook</span><span class="sxs-lookup"><span data-stu-id="2e552-134">See Also</span></span>  
[<span data-ttu-id="2e552-135">Aangepaste rapportlay-outs bijwerken</span><span class="sxs-lookup"><span data-stu-id="2e552-135">Update Custom Report Layouts</span></span>](ui-update-report-layouts.md)  
[<span data-ttu-id="2e552-136">Aangepaste rapportlay-outs maken en wijzigen</span><span class="sxs-lookup"><span data-stu-id="2e552-136">Create and Modify Custom Report Layouts</span></span>](ui-how-create-custom-report-layout.md)  
[<span data-ttu-id="2e552-137">Een aangepaste indeling voor een rapport of document importeren of exporteren</span><span class="sxs-lookup"><span data-stu-id="2e552-137">Import and Export a Custom Report or Document Layout</span></span>](ui-how-import-and-export-report-layout.md)  
[<span data-ttu-id="2e552-138">Documenten per e-mail verzenden</span><span class="sxs-lookup"><span data-stu-id="2e552-138">Send Documents by Email</span></span>](ui-how-send-documents-email.md)  
[<span data-ttu-id="2e552-139">Rapportlay-outs beheren</span><span class="sxs-lookup"><span data-stu-id="2e552-139">Managing Report Layouts</span></span>](ui-manage-report-layouts.md)  
[<span data-ttu-id="2e552-140">Werken met rapporten, batchverwerkingen en XMLports</span><span class="sxs-lookup"><span data-stu-id="2e552-140">Working with Reports, Batch Jobs, and XMLports</span></span>](ui-work-report.md)  
[<span data-ttu-id="2e552-141">Werken met rapporten, batchverwerkingen en XMLports</span><span class="sxs-lookup"><span data-stu-id="2e552-141">Working with Reports, Batch Jobs, and XMLports</span></span>](ui-work-report.md)  