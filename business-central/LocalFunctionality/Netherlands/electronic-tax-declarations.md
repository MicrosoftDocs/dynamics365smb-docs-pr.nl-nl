---
title: Elektronische belastingaangiften
description: Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 01/10/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 47d69e7a0ed2541b50a78cead35ace20b1714b16
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="electronic-tax-declarations"></a><span data-ttu-id="11660-103">Elektronische belastingaangiften</span><span class="sxs-lookup"><span data-stu-id="11660-103">Electronic Tax Declarations</span></span>
<span data-ttu-id="11660-104">Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="11660-104">Companies must deliver their VAT and ICP declarations electronically to the tax authorities.</span></span>  

## <a name="prepare-for-electronic-declaration"></a><span data-ttu-id="11660-105">Voorbereiding voor elektronische aangifte</span><span class="sxs-lookup"><span data-stu-id="11660-105">Prepare for Electronic Declaration</span></span>  
 <span data-ttu-id="11660-106">Voordat je elektronische aangiften kan versturen naar de belastingdienst moeten eerst de volgende taken zijn uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="11660-106">Before you can send electronic declarations to the tax authorities you must perform the following tasks:</span></span>  

1.  <span data-ttu-id="11660-107">Gebruikerscertificaten aanvragen bij de certificaatautoriteit (CA) en deze importeren in de toepassing.</span><span class="sxs-lookup"><span data-stu-id="11660-107">Request user certificates from the certification authority (CA) and import them in the application.</span></span> <span data-ttu-id="11660-108">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="11660-108">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  
2.  <span data-ttu-id="11660-109">Aanmelden voor elektronische aangifte bij de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="11660-109">Register at the tax authorities for electronic declaration.</span></span>  
3.  <span data-ttu-id="11660-110">Algemene en persoonlijke gegevens, ontvangen van de belastingdienst, in het venster **Elek. aangifte-instellingen** invoeren.</span><span class="sxs-lookup"><span data-stu-id="11660-110">Enter general data and personal data received from the tax authorities in the **Elec. Tax Declaration Setup** window.</span></span>  

<span data-ttu-id="11660-111">Zie voor meer informatie [Elektronische btw- en ICP-aangiftes](electronic-vat-and-icp-declarations.md).</span><span class="sxs-lookup"><span data-stu-id="11660-111">For more information, see [Electronic VAT and ICP Declarations](electronic-vat-and-icp-declarations.md).</span></span>  

## <a name="create-and-submit-electronic-declarations"></a><span data-ttu-id="11660-112">Elektronische aangiftes maken en verzenden</span><span class="sxs-lookup"><span data-stu-id="11660-112">Create and Submit Electronic Declarations</span></span>  
<span data-ttu-id="11660-113">Als de hierboven vermelde taken zijn afgerond, kan de toepassing btw- en ICP-aangiften maken en verzenden naar de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="11660-113">When the tasks stated above are finished the application can create and submit VAT and ICP declarations to the tax authorities.</span></span>  

<span data-ttu-id="11660-114">De belastingdienst zal voor elke ontvangen aangifte een responsbericht sturen.</span><span class="sxs-lookup"><span data-stu-id="11660-114">For each electronic declaration the tax authorities will send a response message.</span></span> <span data-ttu-id="11660-115">Deze responsberichten worden opgehaald van de server bij de belastingdienst en verwerkt in de applicatie.</span><span class="sxs-lookup"><span data-stu-id="11660-115">These messages must be received from the server of the tax authorities and processed.</span></span>  

## <a name="response-message-from-the-tax-authorities"></a><span data-ttu-id="11660-116">Responsbericht van de belastingdienst</span><span class="sxs-lookup"><span data-stu-id="11660-116">Response Message from the Tax Authorities</span></span>  
<span data-ttu-id="11660-117">De belastingdienst zal een responsbericht sturen om het bedrijf te informeren over de status van de elektronische aangifte(n).</span><span class="sxs-lookup"><span data-stu-id="11660-117">The tax authorities will send a response message to inform the company about the status of their electronic declarations.</span></span> <span data-ttu-id="11660-118">Om te beginnen moet u de responsberichten van de belastingdienst in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] importeren.</span><span class="sxs-lookup"><span data-stu-id="11660-118">The first step is to import the response messages from the tax authorities in [!INCLUDE[d365fin](../../includes/d365fin_md.md)].</span></span> <span data-ttu-id="11660-119">Vervolgens verwerkt u deze responsberichten.</span><span class="sxs-lookup"><span data-stu-id="11660-119">The second step is processing the response messages.</span></span>  

<span data-ttu-id="11660-120">Het responsbericht moeten aan de gerelateerde elektronische aangifte zijn gekoppeld.</span><span class="sxs-lookup"><span data-stu-id="11660-120">The response message must be linked to the related electronic tax declaration.</span></span>

<span data-ttu-id="11660-121">Als de begeleidende elektronische belastingaangifte is gevonden moeten, afhankelijk van de responssoort, verschillende stappen worden uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="11660-121">If the accompanying electronic tax declaration is found then, depending on the type of the response message, different steps must be performed.</span></span>  

## <a name="acknowledgement-response-message"></a><span data-ttu-id="11660-122">Bevestiging van responsbericht</span><span class="sxs-lookup"><span data-stu-id="11660-122">Acknowledgement Response Message</span></span>  
<span data-ttu-id="11660-123">Als er geen fouten zijn gevonden in de elektronische aangifte en de gegevens zijn verwerkt door de belastingdienst, wordt het veld **Status** in de tabel **Elek. aangiftekop** gewijzigd in **Geaccepteerd**.</span><span class="sxs-lookup"><span data-stu-id="11660-123">If no errors were found in the electronic declaration and the data has been processed by the tax authorities, the **Status** field in the **Elec. Tax Declaration Header** table will be changed into **Acknowledgement**.</span></span>  

## <a name="declaration-for-a-fiscal-entity"></a><span data-ttu-id="11660-124">Aangifte voor een fiscale eenheid</span><span class="sxs-lookup"><span data-stu-id="11660-124">Declaration for a Fiscal Entity</span></span>  
<span data-ttu-id="11660-125">Als een bedrijf verscheidene bedrijven heeft geregistreerd als dochterondernemingen van een moedermaatschappij, hebben deze de mogelijkheid om de btw-aangifte afzonderlijk te doen of gecombineerd voor één fiscale eenheid.</span><span class="sxs-lookup"><span data-stu-id="11660-125">If a company has several companies registered as subsidiaries of a holding company, they have the option to submit the VAT declaration individually or combined for one fiscal entity.</span></span> <span data-ttu-id="11660-126">Ongeacht de keuze, moeten ICP-aangiften altijd afzonderlijk worden ingediend.</span><span class="sxs-lookup"><span data-stu-id="11660-126">Regardless of the choice, the ICP declarations must always be submitted individually.</span></span>  

<span data-ttu-id="11660-127">In het programma kunnen geen belastinggegevens van verschillende bedrijven worden gecombineerd tot één btw-aangifte.</span><span class="sxs-lookup"><span data-stu-id="11660-127">The application cannot combine tax information for several companies into one electronic VAT declaration.</span></span> <span data-ttu-id="11660-128">Als het bedrijf de belastinggegevens wil combineren, moet er een btw-aangifte op papier worden opgesteld voor elke dochteronderneming en moet het totale bedrag voor de moedermaatschappij worden berekend.</span><span class="sxs-lookup"><span data-stu-id="11660-128">If the company wants to combine the tax information, they have to create a VAT statement on paper for each subsidiary company and calculate the total amount for the holding company.</span></span> <span data-ttu-id="11660-129">Daarna moeten deze bedragen handmatig worden ingevoerd op de website van de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="11660-129">After that these amounts can be manually entered on the website of the tax authorities.</span></span>  

<span data-ttu-id="11660-130">Voor elke dochteronderneming kan een elektronische ICP-aangifte worden opgesteld en aan de belastingdienst worden gezonden.</span><span class="sxs-lookup"><span data-stu-id="11660-130">For each subsidiary company an electronic ICP declaration can be created and submitted to the tax authorities.</span></span> <span data-ttu-id="11660-131">Deze elektronische ICP-aangiften moeten het btw-nummer van de dochteronderneming en het veld **Nr. fiscale eenheid**</span><span class="sxs-lookup"><span data-stu-id="11660-131">These electronic ICP declarations must contain the VAT registration number of the subsidiary company and the **Fiscal Entity No.**</span></span> <span data-ttu-id="11660-132">van de moedermaatschappij uit de tabel **Bedrijfsgegevens** bevatten.</span><span class="sxs-lookup"><span data-stu-id="11660-132">field of the holding company, in the **Company Information** window.</span></span>  

<span data-ttu-id="11660-133">Als u elektronische aangiften voor dochterondernemingen van een moedermaatschappij wilt instellen, moet u een vinkje plaatsen in het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen**.</span><span class="sxs-lookup"><span data-stu-id="11660-133">To setup electronic declarations for subsidiaries of a holding company, you must select the **Part of Fiscal Entity** field in the **Elec. Tax Declaration Setup** window.</span></span>  

## <a name="digipoort"></a><span data-ttu-id="11660-134">Digipoort</span><span class="sxs-lookup"><span data-stu-id="11660-134">Digipoort</span></span>
<span data-ttu-id="11660-135">In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen.</span><span class="sxs-lookup"><span data-stu-id="11660-135">In the Netherlands, you use Digipoort to make periodic electronic filings for VAT declarations and ICP reports in EU sales list submissions.</span></span> <span data-ttu-id="11660-136">Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden.</span><span class="sxs-lookup"><span data-stu-id="11660-136">Digipoort is the electronic post office provided by the Dutch government for companies.</span></span> <span data-ttu-id="11660-137">Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes.</span><span class="sxs-lookup"><span data-stu-id="11660-137">It provides the common infrastructure for the communication of information between companies and the government, including VAT declarations.</span></span> <span data-ttu-id="11660-138">De rapporten hebben de XBRL-indeling.</span><span class="sxs-lookup"><span data-stu-id="11660-138">The reports are in XBRL format.</span></span> <span data-ttu-id="11660-139">Zie voor meer informatie [Overzicht van Digipoort](digipoort-overview.md).</span><span class="sxs-lookup"><span data-stu-id="11660-139">For more information, see [Digipoort Overview](digipoort-overview.md).</span></span>

## <a name="see-also"></a><span data-ttu-id="11660-140">Zie ook</span><span class="sxs-lookup"><span data-stu-id="11660-140">See Also</span></span>  
 [<span data-ttu-id="11660-141">Elektronische btw- en ICP-aangiften</span><span class="sxs-lookup"><span data-stu-id="11660-141">Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md)  
 [<span data-ttu-id="11660-142">Overzicht van Digipoort</span><span class="sxs-lookup"><span data-stu-id="11660-142">Digipoort Overview</span></span>](digipoort-overview.md)

