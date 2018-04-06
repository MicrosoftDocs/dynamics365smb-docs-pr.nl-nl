---
title: Elektronische btw- en ICP-aangiften
description: Bedrijven moeten periodieke btw- en ICP-aangiften verzenden.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8341d8b1cb72ea9db0e9c3fc9001915a628b0470
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="electronic-vat-and-icp-declarations"></a><span data-ttu-id="f892d-103">Elektronische btw- en ICP-aangiften</span><span class="sxs-lookup"><span data-stu-id="f892d-103">Electronic VAT and ICP Declarations</span></span>
<span data-ttu-id="f892d-104">Bedrijven moeten periodieke btw- en ICP-aangiften verzenden.</span><span class="sxs-lookup"><span data-stu-id="f892d-104">Companies must submit periodic VAT and ICP declarations.</span></span>  

<span data-ttu-id="f892d-105">Btw aangiften moeten op een maandelijkse of driemaandelijkse basis worden verzonden.</span><span class="sxs-lookup"><span data-stu-id="f892d-105">VAT declarations must be submitted on a monthly or quarterly basis.</span></span>  

<span data-ttu-id="f892d-106">Bedrijven die goederen of diensten verkopen aan EU-landen, moeten ICP-aangiften (Intracommunautaire leveringen) op kwartaalbasis verzenden.</span><span class="sxs-lookup"><span data-stu-id="f892d-106">Companies that sell goods or services to European Union (EU) countries must submit Intracommunautaire leveringen (ICP) declarations on a quarterly basis.</span></span> <span data-ttu-id="f892d-107">Inkopen zijn niet opgenomen in deze aangifte.</span><span class="sxs-lookup"><span data-stu-id="f892d-107">Purchases are not included in this declaration.</span></span> <span data-ttu-id="f892d-108">Voor deze intracommunautaire transacties moet echter de handelswaar de grens fysiek overschrijden.</span><span class="sxs-lookup"><span data-stu-id="f892d-108">For these intracommunautaire transactions, it is required that the merchandise have crossed the border physically.</span></span> <span data-ttu-id="f892d-109">Het is niet voldoende dat de locatie van een factuuradres of het kantoor van de leverancier of klant in een ander land of een andere regio in een EU-land ligt.</span><span class="sxs-lookup"><span data-stu-id="f892d-109">It is not enough that the location of an invoice address or the office of the vendor or customer is in another EU country or region.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="f892d-110">Voordat u elektronische aangiften naar de belastingdienst verstuurt, dient uw bedrijf aangemeld te zijn voor elektronische aangifte.</span><span class="sxs-lookup"><span data-stu-id="f892d-110">Before you can send electronic declarations to the tax authorities you must register your company for electronic declaration.</span></span> <span data-ttu-id="f892d-111">De informatie die de belastingdienst nodig heeft is afhankelijk van de ondertekeningsmethode die uw bedrijf zal gebruiken, PIN of PKI.</span><span class="sxs-lookup"><span data-stu-id="f892d-111">The information that the tax authorities need depends on the sign method your company will use, PIN or PKI.</span></span> <span data-ttu-id="f892d-112">Voor beide methoden geldt dat u het formulier "Aanmeldingsformulier voor elektronisch berichtenverkeer met de belastingdienst" naar de belastingdienst moet opsturen.</span><span class="sxs-lookup"><span data-stu-id="f892d-112">For both methods, you have to send the form "Aanmeldingsformulier voor elektronisch berichtenverkeer met de belastingdienst" to the tax authorities.</span></span>  
>   
>  <span data-ttu-id="f892d-113">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f892d-113">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  

## <a name="submitting-electronic-tax-declarations"></a><span data-ttu-id="f892d-114">Elektronische belastingaangiften versturen</span><span class="sxs-lookup"><span data-stu-id="f892d-114">Submitting Electronic Tax Declarations</span></span>  
<span data-ttu-id="f892d-115">U kunt de btw-aangiften en ICP-aangiften als volgt verzenden:</span><span class="sxs-lookup"><span data-stu-id="f892d-115">You can submit the VAT declarations and ICP declarations in the following ways:</span></span>  

- <span data-ttu-id="f892d-116">Meld u aan op de website van het Nederlandse belastingkantoor en voer de informatie handmatig in.</span><span class="sxs-lookup"><span data-stu-id="f892d-116">Log on to the website of the Dutch tax office and enter the information manually.</span></span> <span data-ttu-id="f892d-117">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f892d-117">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  

    <span data-ttu-id="f892d-118">Voor ICP-aangiften kunt u maximaal 99 regels invoeren.</span><span class="sxs-lookup"><span data-stu-id="f892d-118">For ICP declarations, you can enter a maximum of 99 lines.</span></span>  

- <span data-ttu-id="f892d-119">Een elektronische aangifte maken en het versleutelde bestand via SMTP (Simple Mail Transfer Protocol) naar het Nederlandse belastingkantoor versturen.</span><span class="sxs-lookup"><span data-stu-id="f892d-119">Create an electronic declaration and submit the encrypted file through Simple Mail Transfer Protocol (SMTP) server to the Dutch tax office.</span></span>  

<span data-ttu-id="f892d-120">De elektronische btw-aangifte bevat de geboekte btw en de berekende belasting over een opgegeven periode die aan de douane moet worden betaald.</span><span class="sxs-lookup"><span data-stu-id="f892d-120">The electronic VAT declaration contains the posted VAT and the calculated duty liable to the customs authorities for a specified period.</span></span> <span data-ttu-id="f892d-121">De gegevens van de btw-aangifte zijn gebaseerd op de definitie van de btw-aangifte in de tabel **Btw-aangifteregel**.</span><span class="sxs-lookup"><span data-stu-id="f892d-121">The data of the VAT declaration is based on the definition of the VAT statement in the **VAT Statement Line** table.</span></span> <span data-ttu-id="f892d-122">Zie Btw-aangifteregel voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="f892d-122">For more information, see VAT Statement Line.</span></span>  

<span data-ttu-id="f892d-123">De gegevens van de ICP-aangifte zijn gebaseerd op de tabel **Btw-post**.</span><span class="sxs-lookup"><span data-stu-id="f892d-123">The data of the ICP declaration is based on the **VAT Entry** table.</span></span> <span data-ttu-id="f892d-124">Zie voor meer informatie Btw-post.</span><span class="sxs-lookup"><span data-stu-id="f892d-124">For more information, see VAT Entry.</span></span>  

## <a name="electronic-tax-declaration-methods"></a><span data-ttu-id="f892d-125">Methoden voor elektronische aangiften</span><span class="sxs-lookup"><span data-stu-id="f892d-125">Electronic Tax Declaration Methods</span></span>  
<span data-ttu-id="f892d-126">U kunt de btw- en ICP-aangifte op elektronische wijze verzenden naar de belastingdienst met de volgende methoden:</span><span class="sxs-lookup"><span data-stu-id="f892d-126">You can submit the VAT and ICP declarations electronically to the tax authorities using the following methods:</span></span>  

<span data-ttu-id="f892d-127">**PIN-methode (Personal Identification Number)**</span><span class="sxs-lookup"><span data-stu-id="f892d-127">**Personal identification number (PIN) method**</span></span>  
 <span data-ttu-id="f892d-128">Gebruikt een PIN-code om de aangifte te ondertekenen.</span><span class="sxs-lookup"><span data-stu-id="f892d-128">Uses a PIN code to sign the declaration.</span></span> <span data-ttu-id="f892d-129">Als u uw aangiften met de PIN-methode verzendt, moet u de PIN-code voor uw bedrijf maken en leveren aan de belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f892d-129">If you submit your declarations using the PIN method, you must create a PIN code for your company and deliver it to the tax authorities.</span></span> <span data-ttu-id="f892d-130">Deze code helpt de belastingdienst het bedrijf te identificeren dat de elektronische aangifte heeft verstuurd.</span><span class="sxs-lookup"><span data-stu-id="f892d-130">This code helps the tax authorities to identify the company that has submitted the electronic declaration.</span></span> <span data-ttu-id="f892d-131">Deze PIN-code wordt niet opgeslagen in de database.</span><span class="sxs-lookup"><span data-stu-id="f892d-131">This PIN code is not stored in the database.</span></span> <span data-ttu-id="f892d-132">Daarom moet u de PIN-code op een veilige plaats bewaren.</span><span class="sxs-lookup"><span data-stu-id="f892d-132">Therefore, you must save the PIN code in a secure location.</span></span>  

> [!WARNING]  
>  <span data-ttu-id="f892d-133">De belastingdienst overweegt aangiften te accepteren die met behulp van een PIN-code zijn ondertekend.</span><span class="sxs-lookup"><span data-stu-id="f892d-133">The tax authorities are reconsidering whether to accept declarations that are signed using a PIN code.</span></span> <span data-ttu-id="f892d-134">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f892d-134">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  

<span data-ttu-id="f892d-135">**PKI-methode (Public Key Infrastructure)**</span><span class="sxs-lookup"><span data-stu-id="f892d-135">**Public Key Infrastructure (PKI) method**</span></span>  
 <span data-ttu-id="f892d-136">Gebruikt digitale certificaten om berichten te versleutelen en digitale handtekening te verifiëren.</span><span class="sxs-lookup"><span data-stu-id="f892d-136">Uses digital certificates to encrypt messages and verify digital signature.</span></span> <span data-ttu-id="f892d-137">Als u uw aangiften met de PKI-methode verzendt, moet u ook aanvullende certificaten, algemene parameters en andere parameters hebben wanneer u de PKI-methode gebruikt.</span><span class="sxs-lookup"><span data-stu-id="f892d-137">If you submit your declarations using the PKI method, you must also have additional certificates, generic parameters, and other parameters when you use the PKI method.</span></span> <span data-ttu-id="f892d-138">Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="f892d-138">For more information, see the [website](http://go.microsoft.com/fwlink/?LinkID=223151) of the Dutch tax office.</span></span>  

## <a name="contact-information"></a><span data-ttu-id="f892d-139">Contactgegevens</span><span class="sxs-lookup"><span data-stu-id="f892d-139">Contact Information</span></span>  
<span data-ttu-id="f892d-140">De elektronische btw- en ICP-aangifte bevat contactgegevens over de belastingplichtige of intermediair.</span><span class="sxs-lookup"><span data-stu-id="f892d-140">The electronic VAT and ICP declarations contain contact information about the taxpayer or the agent.</span></span> <span data-ttu-id="f892d-141">Zie voor meer informatie Btw-nummer.</span><span class="sxs-lookup"><span data-stu-id="f892d-141">For more information, see VAT Registration No..</span></span>  

## <a name="see-also"></a><span data-ttu-id="f892d-142">Zie ook</span><span class="sxs-lookup"><span data-stu-id="f892d-142">See Also</span></span>  
 <span data-ttu-id="f892d-143">[Elektronische belastingaangiften](electronic-tax-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="f892d-143">[Electronic Tax Declarations](electronic-tax-declarations.md) </span></span>  
 <span data-ttu-id="f892d-144">[Btw-categorieën instellen](how-to-set-up-vat-categories.md) </span><span class="sxs-lookup"><span data-stu-id="f892d-144">[Set Up VAT Categories](how-to-set-up-vat-categories.md) </span></span>  
 <span data-ttu-id="f892d-145">[Elektronische btw- en ICP-aangiften maken](how-to-create-electronic-vat-and-icp-declarations.md) </span><span class="sxs-lookup"><span data-stu-id="f892d-145">[Create Electronic VAT and ICP Declarations](how-to-create-electronic-vat-and-icp-declarations.md) </span></span>  
 [<span data-ttu-id="f892d-146">Responsberichten van de belastingdienst verwerken</span><span class="sxs-lookup"><span data-stu-id="f892d-146">Process Response Messages from Tax Authorities</span></span>](how-to-process-response-messages-from-tax-authorities.md)

