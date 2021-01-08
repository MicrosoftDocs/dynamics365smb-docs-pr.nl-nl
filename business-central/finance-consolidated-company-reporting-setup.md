---
title: Een bedrijfsconsolidatie instellen
description: Lees hoe u kunt configureren hoe gegevens van verschillende bedrijven in Business Central worden gerapporteerd aan een consolidatiebedrijf.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: consolidation, subsidiaries, consolidate
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 7a5ad9eeb2dc42f1cb6fe7640bda721a6f511a75
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927636"
---
# <a name="set-up-company-consolidation"></a><span data-ttu-id="8bf4c-103">Een bedrijfsconsolidatie instellen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-103">Set Up Company Consolidation</span></span>

<span data-ttu-id="8bf4c-104">Voordat u de grootboekposten van twee of meer afzonderlijke bedrijven (dochterondernemingen) in een geconsolideerd bedrijf kunt consolideren, moet u de rekeningschema's en het consolidatiebedrijf voorbereiden.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-104">Before you can consolidate the general ledger entries of two or more separate companies (subsidiaries) into a consolidated company, you must prepare the charts of accounts and the consolidation company.</span></span>  

<span data-ttu-id="8bf4c-105">Afhankelijk van de complexiteit van uw bedrijven kunt u consolidatie op twee manieren instellen:</span><span class="sxs-lookup"><span data-stu-id="8bf4c-105">Depending on the complexity of your businesses, there are two ways to set up consolidation:</span></span>

* <span data-ttu-id="8bf4c-106">Als u geen geavanceerde instellingen nodig hebt, bijvoorbeeld om een bedrijf waarvan u slechts deels de eigenaar bent op te nemen, kunt u de begeleide instelling **Bedrijfsconsolidatie** gebruiken om snel een consolidatie in te stellen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-106">If you do not need advanced settings, such as including a company that you only own part of, you can use the **Company Consolidation** assisted setup guide to quickly set up a consolidation.</span></span> <span data-ttu-id="8bf4c-107">Hierbij wordt u door de basisstappen geleid.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-107">The guide helps you through the basic steps.</span></span>
* <span data-ttu-id="8bf4c-108">Als u meer geavanceerde instellingen nodig hebt, kunt u het geconsolideerde bedrijf en de bedrijfsunits zelf instellen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-108">If you do need more advanced settings, you can set up the consolidated company and business units yourself.</span></span>
  * <span data-ttu-id="8bf4c-109">Specificeer welke grootboekrekeningen van elke bedrijfsunit moeten worden opgenomen in de consolidatie en geef de consolidatievertaalmethode voor elke rekening op.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-109">In each business unit, specify which general ledger accounts are to be included in the consolidation, and specify the consolidation translation method for each account.</span></span>
  * <span data-ttu-id="8bf4c-110">Stel in het consolidatiebedrijf een bedrijfsunitkaart in voor elk bedrijf dat moet worden opgenomen in de consolidatie.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-110">In the consolidation company, set up a business unit card for each company to be included in the consolidation.</span></span> <span data-ttu-id="8bf4c-111">De bedrijfsunitkaart bevat informatie zoals de datums van het boekjaar van de bedrijfsunit en het percentage van elke rekening die moet worden opgenomen in de consolidatie.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-111">The business unit card includes information, such as the dates of the business unit's fiscal year, and the percentage of each account that must be included in the consolidation.</span></span>

## <a name="simple-consolidation-setup"></a><span data-ttu-id="8bf4c-112">Eenvoudige consolidatie instellen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-112">Simple consolidation setup</span></span>

<span data-ttu-id="8bf4c-113">Als de consolidatie ongecompliceerd is, bijvoorbeeld omdat u de enige eigenaar van de te consolideren bedrijfsunits bent, wordt u door de begeleide instellingen **Bedrijfconsolidatie** door de volgende stappen geleid:</span><span class="sxs-lookup"><span data-stu-id="8bf4c-113">If your consolidation is straightforward, for example because you wholly-own the business units to consolidate, the **Company Consolidation** assisted setup guide will help you through the following steps:</span></span>

* <span data-ttu-id="8bf4c-114">Geef op of er een nieuw geconsolideerd bedrijf moet worden gemaakt of dat de gegevens moeten worden geconsolideerd in een bedrijf dat u al voor de consolidatie hebt gemaakt.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-114">Choose whether to create a new consolidated company, or whether to consolidate the data in a company that you have already created for the consolidation.</span></span> <span data-ttu-id="8bf4c-115">Het bedrijf moet geen transacties bevatten.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-115">The company should not contain transactions.</span></span>
* <span data-ttu-id="8bf4c-116">Bekijk de resultaten.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-116">Preview the results.</span></span> [!INCLUDE[d365fin](includes/d365fin_md.md)] <span data-ttu-id="8bf4c-117">verifieert of de hoofdgegevens en transacties naar het geconsolideerde bedrijf kunnen worden overgebracht.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-117">verifies that the master data and transactions can be successfully transferred to the consolidated company.</span></span>

<span data-ttu-id="8bf4c-118">Ga als volgt te werk om de begeleide instelling te gebruiken:</span><span class="sxs-lookup"><span data-stu-id="8bf4c-118">To use the assisted setup guide, follow these steps:</span></span>

1. <span data-ttu-id="8bf4c-119">Kies in het rolcentrum **Accountant** de actie **Begeleide instelling**.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-119">On the **Accountant** Role Center, choose the **Assisted Setup** action.</span></span>
2. <span data-ttu-id="8bf4c-120">Kies **Consolidatierapportage instellen** en voltooi elke stap in de begeleide instelling.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-120">Choose **Set up consolidation reporting**, and then complete each step in the assisted setup guide.</span></span>

## <a name="advanced-consolidation-setup"></a><span data-ttu-id="8bf4c-121">Geavanceerde consolidatie instellen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-121">Advanced consolidation setup</span></span>

<span data-ttu-id="8bf4c-122">Als u meer geavanceerde instellingen voor de consolidatie nodig hebt, kunt u de consolidatie handmatig instellen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-122">If you need more advanced settings for your consolidation, you can set up consolidation manually.</span></span> <span data-ttu-id="8bf4c-123">U kunt dit bijvoorbeeld doen als u bedrijven hebt die slechts deels uw eigendom zijn of die u niet in de consolidatie wilt opnemen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-123">For example, if you have companies that you own only partially, or you have companies that you do not want to include in the consolidation.</span></span>  

### <a name="set-up-the-consolidated-company"></a><span data-ttu-id="8bf4c-124">Het geconsolideerde bedrijf instellen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-124">Set up the consolidated company</span></span>

<span data-ttu-id="8bf4c-125">U moet eerst het geconsolideerde bedrijf instellen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-125">First, you must set up the consolidated company.</span></span> <span data-ttu-id="8bf4c-126">U stelt het geconsolideerde bedrijf in op dezelfde manier als waarop u andere bedrijven instelt.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-126">You set up the consolidated company in the same way that you set up other companies.</span></span> <span data-ttu-id="8bf4c-127">Zie voor meer informatie [Voorbereid zijn om zaken te doen](ui-get-ready-business.md).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-127">For more information, see [Getting Ready for Doing Business](ui-get-ready-business.md).</span></span>  

<span data-ttu-id="8bf4c-128">De volgende lijst illustreert de belangrijkste aspecten van het geconsolideerde bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-128">The following list illustrates key aspects of the consolidated company.</span></span>

1. <span data-ttu-id="8bf4c-129">Het rekeningschema instellen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-129">Set up the chart of accounts</span></span>

    <span data-ttu-id="8bf4c-130">Voor meer informatie raadpleegt u [Het rekeningschema instellen of wijzigen](finance-setup-chart-accounts.md).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-130">For more information, see [Setting Up or Changing the Chart of Accounts](finance-setup-chart-accounts.md).</span></span>  

    <span data-ttu-id="8bf4c-131">De rekeningschema's kunnen identiek zijn voor een bedrijfsunit en het geconsolideerde bedrijf, of het geconsolideerde bedrijf kan een ander rekeningschema hebben.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-131">The charts of accounts can be identical across a business unit and the consolidated company, or the consolidated company can have a different chart of account.</span></span> <span data-ttu-id="8bf4c-132">Als het rekeningschema van een bedrijfsunit verschilt van dat van het geconsolideerde bedrijf, moet u de toewijzing tussen rekeningen op de rekeningen in de bedrijfsunit opgeven.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-132">If a business unit's chart of accounts is different from that of the consolidated company, you must specify the mapping between accounts on the accounts in the business unit.</span></span> <span data-ttu-id="8bf4c-133">Zie voor meer informatie de sectie [Grootboekrekeningen voorbereiden voor consolidatie](#glacc).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-133">For more information, see the [Prepare general ledger accounts for consolidation](#glacc) section.</span></span>

2. <span data-ttu-id="8bf4c-134">Bedrijfsunits toevoegen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-134">Add business units</span></span>

    <span data-ttu-id="8bf4c-135">Voor het consolideren van de financiële gegevens van meerdere bedrijven in een geconsolideerd bedrijf moet u gegevens opgeven over zowel het dochterbedrijf als de bedrijfsunits die worden opgenomen en over de mate waarin de cijfers ervan worden opgenomen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-135">To consolidate several companies' financial data in a consolidated company, you must enter information about the subsidiary as business units to be included and about how much their figures will be included.</span></span>

    <span data-ttu-id="8bf4c-136">Zie voor meer informatie de sectie [Bedrijfsunits toevoegen](#busunit).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-136">For more information, see the [Add business units](#busunit) section.</span></span>
3. <span data-ttu-id="8bf4c-137">U kunt wisselkoersen opgeven wanneer u de financiële overzichten van bedrijfsunits consolideert als de financiële overzichten in een vreemde valuta zijn.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-137">You can specify exchange rates when consolidating the financial statements of business units if the financial statements are in a foreign currency.</span></span>

    <span data-ttu-id="8bf4c-138">De drie wisselkoersen die worden gebruikt, zijn **Gemiddelde koers (handmatig)**, **Wisselkoers** en **Laatste wisselkoers**.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-138">The three exchange rates that are used are **Average Rate (Manual)**, **Closing Rate**, and **Last Closing Rate**.</span></span> <span data-ttu-id="8bf4c-139">Zie voor meer informatie de sectie [Wisselkoersen opgeven voor consolidaties](#exchrates).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-139">For more information, see the [Specify exchange rates for consolidations](#exchrates) section.</span></span>
4. <span data-ttu-id="8bf4c-140">U kunt dimensiegegevens en grootboekrekeningen consolideren.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-140">You can consolidate dimension information and general ledger accounts.</span></span>

    <span data-ttu-id="8bf4c-141">Zie voor meer informatie de sectie [Dimensies opnemen of uitsluiten](#dim).</span><span class="sxs-lookup"><span data-stu-id="8bf4c-141">For more information, see the [Include or exclude dimensions](#dim) section.</span></span>

### <a name="add-business-units"></a><a name="busunit"></a><span data-ttu-id="8bf4c-142">Bedrijfsunits toevoegen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-142">Add business units</span></span>

<span data-ttu-id="8bf4c-143">Met [!INCLUDE[d365fin](includes/d365fin_md.md)] kunt u een lijst met te consolideren bedrijfsunits instellen, de boekhoudgegevens vóór de consolidatie controleren, bestanden importeren en consolidatierapporten genereren.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-143">[!INCLUDE[d365fin](includes/d365fin_md.md)] lets you set up a list of business units to consolidate, verify the accounting data before you consolidate it, import files, and generate consolidation reports.</span></span>  

1. <span data-ttu-id="8bf4c-144">Meld u aan bij het geconsolideerde bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-144">Sign in to the consolidated company.</span></span>
2. <span data-ttu-id="8bf4c-145">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bedrijfsunits** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-145">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Business Units**, and then choose the related link.</span></span>  
3. <span data-ttu-id="8bf4c-146">Kies **Nieuw** en vul vervolgens de vereiste velden in.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-146">Choose **New**, and then fill in the required fields.</span></span> [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!IMPORTANT]
    > <span data-ttu-id="8bf4c-147">Wanneer u de velden **Begindatum** en **Einddatum** invult, moet u ervoor zorgen dat u GAAP-regels betreffende de boekhoudperioden van de bedrijfsunit versus het hoofdbedrijf naleeft.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-147">When you fill in the **Starting Date** and **Ending Date** fields, make sure you comply with GAAP rules concerning the fiscal periods of the business unit versus the parent company.</span></span>
4. <span data-ttu-id="8bf4c-148">Herhaal stap 3 voor elke extra bedrijfsunit</span><span class="sxs-lookup"><span data-stu-id="8bf4c-148">Repeat step 3 for each additional business unit</span></span>

<span data-ttu-id="8bf4c-149">Als de bedrijfsunit een vreemde valuta gebruikt, moet u de wisselkoers opgeven die in de consolidatie moet worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-149">If your business unit uses a foreign currency, you must specify the exchange rate to use in the consolidation.</span></span> <span data-ttu-id="8bf4c-150">U moet ook consolidatiegegevens invoeren over de grootboekrekeningen van de bedrijfsunit.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-150">You must also enter consolidation information about the business unit's general ledger accounts.</span></span> <span data-ttu-id="8bf4c-151">Deze processen worden beschreven in de volgende secties.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-151">These processes are described in the following sections.</span></span>

### <a name="prepare-general-ledger-accounts-for-consolidation"></a><a name="glacc"></a><span data-ttu-id="8bf4c-152">Grootboekrekeningen voor consolidatie voorbereiden</span><span class="sxs-lookup"><span data-stu-id="8bf4c-152">Prepare general ledger accounts for consolidation</span></span>

<span data-ttu-id="8bf4c-153">Het rekeningschema van een bedrijf dat wordt geconsolideerd, moet rekeningen voor de consolidatie specificeren.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-153">The chart of accounts for a company that will be consolidated must specify accounts for consolidation.</span></span> <span data-ttu-id="8bf4c-154">Voor elke boekingsgrootboekrekening in elk bedrijf moet u de grootboekrekening in het geconsolideerde bedrijf opgeven waarnaar de balans wordt overgebracht bij consolidatie.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-154">For each posting general ledger account in each company, you must specify the general ledger account in the consolidated company to which the balance will be transferred on consolidation.</span></span> <span data-ttu-id="8bf4c-155">Dit is een toewijzing waarmee bedrijven met een ander rekeningschema samen worden geconsolideerd.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-155">This is a mapping that will allow companies with different chart of accounts to be consolidated together.</span></span>

<span data-ttu-id="8bf4c-156">Als het rekeningschema van de bedrijfsunit afwijkt van dat van het geconsolideerde bedrijf, moet u grootboekrekeningen voorbereiden voor consolidatie.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-156">If the chart of accounts in the business unit differs from the consolidated company, you must prepare general ledger accounts for consolidation.</span></span> <span data-ttu-id="8bf4c-157">U kunt de rekeningen voor het boeken van debet- en creditbedragen opgeven en instellen welke methode moet worden gebruikt voor de vertaling van valuta in het geconsolideerde bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-157">You can specify the accounts to post debits and credits to, and the method to use to translate currencies in the consolidated company.</span></span> <span data-ttu-id="8bf4c-158">Dit is bijvoorbeeld nuttig als u het rapport vaak uitvoert.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-158">For example, this is useful if you frequently run the report.</span></span>

1. <span data-ttu-id="8bf4c-159">Kies in de [!INCLUDE [prodshort](includes/prodshort.md)] van elke bedrijfsunit het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Rekeningschema** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-159">In each business unit's [!INCLUDE [prodshort](includes/prodshort.md)], choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Chart of Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8bf4c-160">Open de kaart voor de rekening en vul de velden op het sneltabblad **Consolidatie** in.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-160">Open the card for the account, and then fill in the fields on the **Consolidation** FastTab.</span></span> [!INCLUDE [tooltip-inline-tip_md](includes/tooltip-inline-tip_md.md)]

### <a name="specify-exchange-rates-for-consolidations"></a><a name="exchrates"></a><span data-ttu-id="8bf4c-161">Wisselkoersen opgeven voor consolidaties</span><span class="sxs-lookup"><span data-stu-id="8bf4c-161">Specify exchange rates for consolidations</span></span>

<span data-ttu-id="8bf4c-162">Als een bedrijfsunit een andere valuta dan het geconsolideerde bedrijf gebruikt, moet u wisselkoersmethoden voor elke rekening opgeven voordat u de consolidatie uitvoert.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-162">If a business unit uses a different currency than the consolidated company, you must specify exchange rate methods for each account before you consolidate.</span></span> <span data-ttu-id="8bf4c-163">Voor elke rekening bepaalt de inhoud van het veld **Consol.-vertaalmethode** de wisselkoers.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-163">For each account, the content of the **Consol. Translation Method** field determines the exchange rate.</span></span> <span data-ttu-id="8bf4c-164">Op elke bedrijfsunitkaart specificeert u in het veld **Wisselkoerstabel** of de consolidatie de wisselkoersen van de bedrijfsunit of van het geconsolideerde bedrijf moet gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-164">In the consolidated company, on each business unit card, in the **Currency Exchange Rate Table** field, you specify whether consolidation will use exchange rates from the business unit or the consolidated company.</span></span> <span data-ttu-id="8bf4c-165">Als u de wisselkoersen van het geconsolideerde bedrijf gebruikt, kunt u de wisselkoersen wijzigen voor een bedrijfseenheid.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-165">If you use exchange rates from the consolidated company, you can change the exchange rates for a business unit.</span></span> <span data-ttu-id="8bf4c-166">Als het veld **Wisselkoerstabel** op de bedrijfsunitkaart de waarde **Lokaal** bevat, kunt u de wisselkoers van de bedrijfsunitkaart wijzigen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-166">For business units, if the **Currency Exchange Rate Table** field on the business unit card contains **Local**, you can change the exchange rate from the business unit card.</span></span> <span data-ttu-id="8bf4c-167">De wisselkoersen worden overgenomen uit de tabel **Valutawisselkoers**, maar u kunt ze vóór de consolidatie wijzigen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-167">The exchange rates are copied from the **Currency Exchange Rate** table, but you can change them before consolidating.</span></span>

<span data-ttu-id="8bf4c-168">In de volgende tabel worden de wisselkoersmethoden beschreven die u voor rekeningen kunt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-168">The following table describes the exchange rate methods you can use for accounts.</span></span>

|<span data-ttu-id="8bf4c-169">Wisselkoers</span><span class="sxs-lookup"><span data-stu-id="8bf4c-169">Exchange rate</span></span> | <span data-ttu-id="8bf4c-170">Normaal gebruik</span><span class="sxs-lookup"><span data-stu-id="8bf4c-170">Typical use</span></span> |
|---|---|
|<span data-ttu-id="8bf4c-171">Gemiddelde koers (Handmatig)</span><span class="sxs-lookup"><span data-stu-id="8bf4c-171">Average Rate (Manual)</span></span> | <span data-ttu-id="8bf4c-172">U berekent de gemiddelde koers voor de te consolideren periode.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-172">You manually calculate the average rate for the period to consolidate.</span></span> <span data-ttu-id="8bf4c-173">Bereken het gemiddelde als rekenkundig gemiddelde of als schatting en geef het resultaat op voor elke bedrijfsunit.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-173">Calculate the average either as an arithmetic average or as a best estimate, and specify the result for each business unit.</span></span> <span data-ttu-id="8bf4c-174">Wordt gebruikt voor resultatenrekening.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-174">Used for income statement accounts.</span></span>|
|<span data-ttu-id="8bf4c-175">Wisselkoers (Balans)</span><span class="sxs-lookup"><span data-stu-id="8bf4c-175">Closing Rate</span></span> | <span data-ttu-id="8bf4c-176">Wordt gebruikt voor balansrekeningen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-176">Used for balance sheet accounts.</span></span>|
|<span data-ttu-id="8bf4c-177">Laatste wisselkoers (Balans)</span><span class="sxs-lookup"><span data-stu-id="8bf4c-177">Last Closing Rate</span></span> | <span data-ttu-id="8bf4c-178">De koers die gold op de vreemde-valutamarkt op de datum waarvoor de balans- of resultatenrekening wordt voorbereid.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-178">The rate that was valid in the foreign exchange market on the date for which the balance sheet or income statement is being prepared.</span></span> <span data-ttu-id="8bf4c-179">U geeft deze koers op voor elke bedrijfsunit.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-179">You enter this rate for each business unit.</span></span> <span data-ttu-id="8bf4c-180">Wordt gebruikt voor balansrekeningen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-180">Used for balance sheet accounts.</span></span>|
|<span data-ttu-id="8bf4c-181">Historische wisselkoers</span><span class="sxs-lookup"><span data-stu-id="8bf4c-181">Historical Rate</span></span> | <span data-ttu-id="8bf4c-182">De wisselkoers die gold toen de transactie plaatsvond.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-182">The exchange rate that was valid when the transaction occurred.</span></span>|
|<span data-ttu-id="8bf4c-183">Samengestelde koers</span><span class="sxs-lookup"><span data-stu-id="8bf4c-183">Composite Rate</span></span> | <span data-ttu-id="8bf4c-184">De bedragen van de huidige periode worden vertaald tegen de gemiddelde koers en worden toegevoegd aan de eerder geregistreerde balans in het geconsolideerde bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-184">The current period amounts are translated at the average rate and added to the previously recorded balance in the consolidated company.</span></span> <span data-ttu-id="8bf4c-185">Deze methode wordt vooral gebruikt voor het resultaat van het lopende boekjaar, omdat hiertoe bedragen uit verschillende perioden behoren en dit dus een samenstelling van bedragen is die zijn vertaald met verschillende wisselkoersen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-185">This method is typically used for retained earnings accounts because they include amounts from different periods and are therefore a composite of amounts translated with different exchange rates.</span></span>|
|<span data-ttu-id="8bf4c-186">Aandelenkoers</span><span class="sxs-lookup"><span data-stu-id="8bf4c-186">Equity Rate</span></span> | <span data-ttu-id="8bf4c-187">Dit lijkt op **Samengestelde koers**.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-187">This is similar to **Composite**.</span></span> <span data-ttu-id="8bf4c-188">Verschillen worden geboekt naar verschillende grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-188">Differences are posted to separate general ledger accounts.</span></span>|

<span data-ttu-id="8bf4c-189">Ga als volgt te werk om wisselkoersen voor bedrijfsunits op te geven:</span><span class="sxs-lookup"><span data-stu-id="8bf4c-189">To specify exchange rates for business units, follow these steps:</span></span>

1. <span data-ttu-id="8bf4c-190">Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bedrijfsunits** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-190">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Business Units**, and then choose the related link.</span></span>  
2. <span data-ttu-id="8bf4c-191">Kies op de pagina **Overzicht bedrijfsunits** de bedrijfsunit en kies vervolgens de actie **Gemiddelde koers (Handmatig)**.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-191">On the **Business Unit List** page, choose the business unit, and then choose the **Average Rate (Manual)** action.</span></span>  
3. <span data-ttu-id="8bf4c-192">Op de pagina **Wisselkoers wijzigen** is de inhoud van het veld **Gerel. wisselkoers** gekopieerd uit de tabel **Valutawisselkoers**, maar u kunt deze wijzigen.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-192">On the **Change Exchange Rate** page, the contents of the **Relational Exch. Rate** field have been copied from the **Currency Exchange Rate** table, but you can modify them.</span></span> <span data-ttu-id="8bf4c-193">Sluit de pagina.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-193">Close the page.</span></span>  
4. <span data-ttu-id="8bf4c-194">Kies de actie **Wisselkoers (Balans)**.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-194">Choose the **Closing Rate** action.</span></span>  
5. <span data-ttu-id="8bf4c-195">Voer in het veld **Gerel. wisselkoersbedrag** de wisselkoers in.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-195">In the **Relational Exch. Rate Amount** field, enter the exchange rate.</span></span>

### <a name="include-or-exclude-dimensions"></a><a name="dim"></a><span data-ttu-id="8bf4c-196">Dimensies opnemen of uitsluiten</span><span class="sxs-lookup"><span data-stu-id="8bf4c-196">Include or exclude dimensions</span></span>

<span data-ttu-id="8bf4c-197">U kunt dimensiegegevens en grootboekrekeningen consolideren.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-197">You can consolidate dimension information and general ledger accounts.</span></span>

* <span data-ttu-id="8bf4c-198">Geef in de relevante dimensies het veld **Consolidatiecode** op of laat het leeg</span><span class="sxs-lookup"><span data-stu-id="8bf4c-198">On the relevant dimensions, specify the **Consolidation Code** field, or leave it blank</span></span>
  * <span data-ttu-id="8bf4c-199">Als u een dimensie in de consolidatie wilt uitsluiten, laat u het veld **Consolidatiecode** leeg voor de dimensie en kiest u geen dimensies in de **Dimensies kopiëren**-velden in consolidatiefuncties of rapporten.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-199">To exclude a dimension in the consolidation, leave the **Consolidation Code** field blank on the dimension, and do not choose dimensions in the **Copy Dimensions** fields in any consolidation functions or reports.</span></span>
  * <span data-ttu-id="8bf4c-200">Als u dimensie-informatie in de consolidatie wilt opnemen, laat u het veld **Consolidatiecode** leeg.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-200">To include dimension information in the consolidation, leave the **Consolidation Code** field blank.</span></span> <span data-ttu-id="8bf4c-201">De consolidatie werkt echter alleen als de dimensiewaarden in de bedrijfsunit hetzelfde zijn als die van het geconsolideerde bedrijf.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-201">However, the consolidation will only work if the dimension values in the business unit are the same as the consolidated company.</span></span>
  * <span data-ttu-id="8bf4c-202">Als u de dimensiewaardecode in de bedrijfsunit wilt consolideren met een andere dimensiewaardecode in het geconsolideerde bedrijf, vult u het veld **Consolidatiecode** voor de relevante dimensies in.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-202">To consolidate the dimension value code in the business unit with a different dimension value code in the consolidated company, fill in the **Consolidation Code** field on the relevant dimensions.</span></span>  
* <span data-ttu-id="8bf4c-203">Voeg de relevante dimensies toe aan de relevante grootboekrekeningen</span><span class="sxs-lookup"><span data-stu-id="8bf4c-203">Add the relevant dimensions to the relevant general ledger accounts</span></span>

### <a name="exclude-a-company-from-consolidation"></a><a name="exclude"></a><span data-ttu-id="8bf4c-204">Een bedrijf uitsluiten van consolidatie</span><span class="sxs-lookup"><span data-stu-id="8bf4c-204">Exclude a company from consolidation</span></span>

<span data-ttu-id="8bf4c-205">Als u een bedrijfsunit niet wilt opnemen in de consolidatie, kunt u deze uitsluiten.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-205">If you do not want to include a business unit in the consolidation, you can exclude it.</span></span> <span data-ttu-id="8bf4c-206">Hiervoor gaat u naar de bedrijfsunitkaart en schakelt u het selectievakje **Consolideren** uit.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-206">To do that, go to the business unit card, and clear the **Consolidate** check box.</span></span>

### <a name="include-a-partially-owned-company-in-consolidation"></a><a name="include"></a><span data-ttu-id="8bf4c-207">Een bedrijf dat deels eigendom is, opnemen in een consolidatie</span><span class="sxs-lookup"><span data-stu-id="8bf4c-207">Include a partially-owned company in consolidation</span></span>

<span data-ttu-id="8bf4c-208">Als u slechts een deel van een bedrijf bezit, kunt u een percentage van elke transactie opnemen dat overeenkomt met het percentage van het bedrijf dat in uw bezit is.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-208">If you own only part of a company, you can include a percentage of each transaction that corresponds to the percentage of the company you own.</span></span> <span data-ttu-id="8bf4c-209">Als u voor 70% eigenaar van het bedrijf bent, bevat de consolidatie bijvoorbeeld € 70 van een factuur voor € 100.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-209">For example, if you own 70% of the company, consolidation will include $70 of an invoice for $100.</span></span> <span data-ttu-id="8bf4c-210">Als u het percentage wilt opgeven dat het bedrijf van u is, gaat u naar de bedrijfsunitkaart en voert u het percentage in het veld **Consolidatie %** in.</span><span class="sxs-lookup"><span data-stu-id="8bf4c-210">To specify the percentage of the company you own, go to the business unit card, and enter the percentage in the **Consolidation %** field.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8bf4c-211">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8bf4c-211">See Also</span></span>

[<span data-ttu-id="8bf4c-212">Financiële gegevens uit meerdere bedrijven consolideren</span><span class="sxs-lookup"><span data-stu-id="8bf4c-212">Consolidating Financial Data from Multiple Companies</span></span>](finance-consolidated-company-reporting.md)  
[<span data-ttu-id="8bf4c-213">Intercompany-transacties beheren</span><span class="sxs-lookup"><span data-stu-id="8bf4c-213">Managing Intercompany Transactions</span></span>](intercompany-manage.md)  
<span data-ttu-id="8bf4c-214">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="8bf4c-214">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>  
[<span data-ttu-id="8bf4c-215">Uw bedrijfsgegevens naar Excel exporteren</span><span class="sxs-lookup"><span data-stu-id="8bf4c-215">Exporting Your Business Data to Excel</span></span>](about-export-data.md)