---
title: Een nieuw bedrijf maken | Microsoft Docs
description: Om RapidStart Services te kunnen gebruiken worden tabellen en pagina's gemaakt, maar ze bevatten geen gegevens.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: sgroespe
ms.openlocfilehash: c7042e783ec004cb2de637e6544c590bc8b9b81c
ms.sourcegitcommit: 88e4b30eaf6fa32af0c1452ce2f85ff1111c75e2
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2020
ms.locfileid: "3187193"
---
# <a name="create-a-new-company"></a><span data-ttu-id="a3fcf-103">Een nieuw bedrijf maken</span><span class="sxs-lookup"><span data-stu-id="a3fcf-103">Create a New Company</span></span>
<span data-ttu-id="a3fcf-104">Als u RapidStart Services voor [!INCLUDE[d365fin](includes/d365fin_md.md)] wilt gebruiken, maakt u eerst een nieuw bedrijf waarvoor u een klantimplementatie wilt uitvoeren.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-104">To use RapidStart Services for [!INCLUDE[d365fin](includes/d365fin_md.md)], you first create a new company for which you want to perform a customer implementation.</span></span> <span data-ttu-id="a3fcf-105">Bij het maken van een nieuw bedrijf worden de standaard [!INCLUDE[d365fin](includes/d365fin_md.md)]-tabellen en pagina's gemaakt, maar deze zijn leeg.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-105">When you create a new company, the standard [!INCLUDE[d365fin](includes/d365fin_md.md)] tables and pages are created, but there is no data in them.</span></span>

<span data-ttu-id="a3fcf-106">Bovendien kunt u specifieke instellingsgegevens op uw bedrijf toepassen nadat u het hebt geïnitialiseerd.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-106">In addition, you can apply specific setup data to your company after you initialize it.</span></span> <span data-ttu-id="a3fcf-107">Deze gegevens worden in een configuratiepakket (een .rapidstart-bestand) verstrekt welke de inhoud in een gecomprimeerde indeling levert.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-107">The information is provided in a configuration package, a .rapidstart file, which delivers content in a compressed format.</span></span>  

<span data-ttu-id="a3fcf-108">Voorbeeldconfiguratiepakketten, inclusief land-/regiospecifieke bestanden, zijn opgenomen bij het demonstratiebedrijf CRONUS.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-108">Example configuration packages, including country/region-specific files, are included with the CRONUS demonstration company.</span></span> <span data-ttu-id="a3fcf-109">Gebruik de volgende procedures om het voorbeeldconfiguratiepakket met een nieuw bedrijf te gebruiken.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-109">Use the following procedures to use the example configuration package with a new company.</span></span>  

## <a name="to-use-the-sample-basicconfig-configuration-package"></a><span data-ttu-id="a3fcf-110">Het voorbeeldconfiguratiepakket BASICCONFIG gebruiken</span><span class="sxs-lookup"><span data-stu-id="a3fcf-110">To use the sample BASICCONFIG configuration package</span></span>  
1. <span data-ttu-id="a3fcf-111">Open het bedrijf CRONUS International Ltd.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-111">Open the CRONUS International Ltd. company.</span></span> <span data-ttu-id="a3fcf-112">Zie voor meer informatie [Basisinstellingen wijzigen](ui-change-basic-settings.md).</span><span class="sxs-lookup"><span data-stu-id="a3fcf-112">For more information, see [Change Basic Settings](ui-change-basic-settings.md).</span></span>
2. <span data-ttu-id="a3fcf-113">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Configuratiepakketten** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-113">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Configuration Packages**, and then choose the related link.</span></span>  
3. <span data-ttu-id="a3fcf-114">Kies het pakket BASICCONFIG in de lijst en kies vervolgens de actie **Pakket exporteren**.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-114">Choose the BASICCONFIG package from the list, and then choose the **Export Package** action.</span></span>  

<span data-ttu-id="a3fcf-115">Gebruik de onderstaande procedure om een nieuw bedrijf aan te maken en gebruik het pakket BASICCONFIG als deel van het proces.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-115">Use the following procedure to create a new company, and use the BASICCONFIG package as part of the process.</span></span>  

## <a name="to-create-a-new-company"></a><span data-ttu-id="a3fcf-116">Een nieuw bedrijf maken</span><span class="sxs-lookup"><span data-stu-id="a3fcf-116">To create a new company</span></span>  
1. <span data-ttu-id="a3fcf-117">Maak een nieuw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-117">Create a new company.</span></span> <span data-ttu-id="a3fcf-118">Zie [Nieuwe bedrijven maken in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md) voor meer informatie.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-118">For more information, see [Creating New Companies in [!INCLUDE[d365fin](includes/d365fin_md.md)]](about-new-company.md).</span></span>
2. <span data-ttu-id="a3fcf-119">Vanuit het rolcentrum RapidStart Services-implementatie kunt u het configuratiepakket nu importeren dat u vanuit het bedrijf CRONUS International Ltd. hebt geëxporteerd.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-119">From the RapidStart Services Implementer Role Center, you can now import the configuration package that you exported from the CRONUS International Ltd. company.</span></span>

<span data-ttu-id="a3fcf-120">Nadat u een nieuw bedrijf maakt, worden sommige tabellen automatisch ingevuld, zelfs als er geen bedrijfssjabloon is toegepast.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-120">After you create a new company, some tables are automatically filled in, even if no company template is applied.</span></span> <span data-ttu-id="a3fcf-121">U kunt bijvoorbeeld de standaardcodes bekijken voor het boeken en voor batchtransacties op de pagina **Broncode**.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-121">For example, you can review the standard codes for posting and batch transactions on the **Source Code** page.</span></span> <span data-ttu-id="a3fcf-122">Als u een lokale versie van [!INCLUDE[d365fin](includes/d365fin_md.md)] hebt, moet u deze tabel bekijken en rekening houden met de lokale taal.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-122">If you provide a local version of [!INCLUDE[d365fin](includes/d365fin_md.md)], you should review this table and consider any local language issues.</span></span>

## <a name="about-data-tables"></a><span data-ttu-id="a3fcf-123">Gegevenstabellen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-123">About Data Tables</span></span>
[!INCLUDE[d365fin](includes/d365fin_md.md)]<span data-ttu-id="a3fcf-124">-gegevenstabellen worden geleverd in twee basistypen: Hoofd en Instellingen.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-124">, data tables come in two basic types: Master and Setup.</span></span> <span data-ttu-id="a3fcf-125">Wanneer u een bedrijfsconfiguratie opzet, kunt u deze typen gebruiken om een gerichte configuratiestrategie te hanteren.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-125">When you are setting up a company configuration, you can use these types to focus your configuration strategy.</span></span>  

### <a name="master-data-tables"></a><span data-ttu-id="a3fcf-126">Hoofdgegevenstabellen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-126">Master Data Tables</span></span>  
<span data-ttu-id="a3fcf-127">In de volgende tabel worden enkele voorbeelden van de hoofdgegevenstabellen weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-127">The following table lists some of the master data tables.</span></span> <span data-ttu-id="a3fcf-128">Wanneer u een nieuw bedrijf initialiseert, zijn deze tabellen leeg.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-128">When you initialize a new company, these tables are empty.</span></span>  

|<span data-ttu-id="a3fcf-129">Tabelnr.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-129">Table No.</span></span>|<span data-ttu-id="a3fcf-130">Tabelnaam</span><span class="sxs-lookup"><span data-stu-id="a3fcf-130">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="a3fcf-131">15</span><span class="sxs-lookup"><span data-stu-id="a3fcf-131">15</span></span>|<span data-ttu-id="a3fcf-132">Grootboekrekening</span><span class="sxs-lookup"><span data-stu-id="a3fcf-132">G/L Account</span></span>|  
|<span data-ttu-id="a3fcf-133">18</span><span class="sxs-lookup"><span data-stu-id="a3fcf-133">18</span></span>|<span data-ttu-id="a3fcf-134">Klant</span><span class="sxs-lookup"><span data-stu-id="a3fcf-134">Customer</span></span>|  
|<span data-ttu-id="a3fcf-135">23</span><span class="sxs-lookup"><span data-stu-id="a3fcf-135">23</span></span>|<span data-ttu-id="a3fcf-136">Leverancier</span><span class="sxs-lookup"><span data-stu-id="a3fcf-136">Vendor</span></span>|  
|<span data-ttu-id="a3fcf-137">27</span><span class="sxs-lookup"><span data-stu-id="a3fcf-137">27</span></span>|<span data-ttu-id="a3fcf-138">Artikel</span><span class="sxs-lookup"><span data-stu-id="a3fcf-138">Item</span></span>|  
|<span data-ttu-id="a3fcf-139">5050</span><span class="sxs-lookup"><span data-stu-id="a3fcf-139">5050</span></span>|<span data-ttu-id="a3fcf-140">Contactpersoon</span><span class="sxs-lookup"><span data-stu-id="a3fcf-140">Contact</span></span>|  

### <a name="setup-data-tables"></a><span data-ttu-id="a3fcf-141">Instellingsgegevenstabellen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-141">Setup Data Tables</span></span>  
<span data-ttu-id="a3fcf-142">De volgende tabel bevat enkele van de instellingsgegevenstabellen, waarin u instelinformatie vastlegt in de configuratievragenlijst.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-142">The following table lists some of the setup data tables, in which you capture setup information in the configuration questionnaire.</span></span> <span data-ttu-id="a3fcf-143">Deze tabellen bevatten basislijngegevens wanneer het bedrijf wordt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-143">These tables contain baseline information when the company is created.</span></span>  

|<span data-ttu-id="a3fcf-144">Tabelnr.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-144">Table No.</span></span>|<span data-ttu-id="a3fcf-145">Tabelnaam</span><span class="sxs-lookup"><span data-stu-id="a3fcf-145">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="a3fcf-146">98</span><span class="sxs-lookup"><span data-stu-id="a3fcf-146">98</span></span>|<span data-ttu-id="a3fcf-147">Grootboekinstellingen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-147">General Ledger Setup</span></span>|  
|<span data-ttu-id="a3fcf-148">311</span><span class="sxs-lookup"><span data-stu-id="a3fcf-148">311</span></span>|<span data-ttu-id="a3fcf-149">Verkoopinstellingen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-149">Sales & Receivables Setup</span></span>|  
|<span data-ttu-id="a3fcf-150">312</span><span class="sxs-lookup"><span data-stu-id="a3fcf-150">312</span></span>|<span data-ttu-id="a3fcf-151">Inkoopinstellingen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-151">Purchases & Payables Setup</span></span>|  
|<span data-ttu-id="a3fcf-152">313</span><span class="sxs-lookup"><span data-stu-id="a3fcf-152">313</span></span>|<span data-ttu-id="a3fcf-153">Voorraadinstelling</span><span class="sxs-lookup"><span data-stu-id="a3fcf-153">Inventory Setup</span></span>|  

<span data-ttu-id="a3fcf-154">Behalve instellingsgegevenstabellen bevat [!INCLUDE[d365fin](includes/d365fin_md.md)] ook instellingstabellen waarin kerngegevens over het bedrijf en de bedrijfsprocessen worden opgegeven.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-154">In addition to setup data tables, [!INCLUDE[d365fin](includes/d365fin_md.md)] also has setup-type data tables that specify core information about the company and its business processes.</span></span> <span data-ttu-id="a3fcf-155">In de volgende tabel wordt een aantal ervan weergegeven.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-155">The following table lists some of them.</span></span>  

|<span data-ttu-id="a3fcf-156">Tabelnr.</span><span class="sxs-lookup"><span data-stu-id="a3fcf-156">Table No.</span></span>|<span data-ttu-id="a3fcf-157">Tabelnaam</span><span class="sxs-lookup"><span data-stu-id="a3fcf-157">Table Name</span></span>|  
|-------------------|--------------------|  
|<span data-ttu-id="a3fcf-158">3</span><span class="sxs-lookup"><span data-stu-id="a3fcf-158">3</span></span>|<span data-ttu-id="a3fcf-159">Betalingsvoorwaarden</span><span class="sxs-lookup"><span data-stu-id="a3fcf-159">Payment Terms</span></span>|  
|<span data-ttu-id="a3fcf-160">4</span><span class="sxs-lookup"><span data-stu-id="a3fcf-160">4</span></span>|<span data-ttu-id="a3fcf-161">Valuta</span><span class="sxs-lookup"><span data-stu-id="a3fcf-161">Currency</span></span>|  
|<span data-ttu-id="a3fcf-162">6</span><span class="sxs-lookup"><span data-stu-id="a3fcf-162">6</span></span>|<span data-ttu-id="a3fcf-163">Klantenprijsgroepen</span><span class="sxs-lookup"><span data-stu-id="a3fcf-163">Customer Price Groups</span></span>|  
|<span data-ttu-id="a3fcf-164">5700</span><span class="sxs-lookup"><span data-stu-id="a3fcf-164">5700</span></span>|<span data-ttu-id="a3fcf-165">SKU</span><span class="sxs-lookup"><span data-stu-id="a3fcf-165">Stockkeeping Unit</span></span>|

  

## <a name="see-also"></a><span data-ttu-id="a3fcf-166">Zie ook</span><span class="sxs-lookup"><span data-stu-id="a3fcf-166">See Also</span></span>  
[<span data-ttu-id="a3fcf-167">Configuraties toepassen op nieuwe bedrijven</span><span class="sxs-lookup"><span data-stu-id="a3fcf-167">Apply Configurations to New Companies</span></span>](admin-apply-configuration-to-new-companies.md)  
[<span data-ttu-id="a3fcf-168">Een bedrijf instellen met RapidStart Services</span><span class="sxs-lookup"><span data-stu-id="a3fcf-168">Setting Up a Company With RapidStart Services</span></span>](admin-set-up-a-company-with-rapidstart.md)  
[<span data-ttu-id="a3fcf-169">Beheer</span><span class="sxs-lookup"><span data-stu-id="a3fcf-169">Administration</span></span>](admin-setup-and-administration.md)
