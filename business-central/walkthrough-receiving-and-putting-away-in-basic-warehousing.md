---
title: 'Procedure: ontvangen en opslaan in standaardmagazijnconfiguraties | Microsoft Docs'
description: In Business Central kunnen de inkomende processen voor ontvangst en opslag op vier manieren worden uitgevoerd met verschillende functionaliteiten, afhankelijk van het complexiteitsniveau van het magazijn.
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
ms.sourcegitcommit: 9dbd92409ba02281f008246194f3ce0c53e4e001
ms.openlocfilehash: 2441c41c6bb28691a855ac4b5d50359b95b23f7d
ms.contentlocale: nl-nl
ms.lasthandoff: 09/28/2018

---
# <a name="walkthrough-receiving-and-putting-away-in-basic-warehouse-configurations"></a><span data-ttu-id="a8014-103">Procedure: ontvangen en opslaan in standaardmagazijnconfiguraties</span><span class="sxs-lookup"><span data-stu-id="a8014-103">Walkthrough: Receiving and Putting Away in Basic Warehouse Configurations</span></span>
<span data-ttu-id="a8014-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)] kunnen de inkomende processen voor ontvangst en opslag op vier manieren worden uitgevoerd met verschillende functionaliteiten, afhankelijk van het complexiteitsniveau van het magazijn.</span><span class="sxs-lookup"><span data-stu-id="a8014-104">In [!INCLUDE[d365fin](includes/d365fin_md.md)], the inbound processes for receiving and putting away can be performed in four ways using different functionalities depending on the warehouse complexity level.</span></span>  

|<span data-ttu-id="a8014-105">Methode</span><span class="sxs-lookup"><span data-stu-id="a8014-105">Method</span></span>|<span data-ttu-id="a8014-106">Inkomend proces</span><span class="sxs-lookup"><span data-stu-id="a8014-106">Inbound process</span></span>|<span data-ttu-id="a8014-107">Opslaglocaties</span><span class="sxs-lookup"><span data-stu-id="a8014-107">Bins</span></span>|<span data-ttu-id="a8014-108">Ontvangsten</span><span class="sxs-lookup"><span data-stu-id="a8014-108">Receipts</span></span>|<span data-ttu-id="a8014-109">Magazijnopslag</span><span class="sxs-lookup"><span data-stu-id="a8014-109">Put-aways</span></span>|<span data-ttu-id="a8014-110">Complexiteitsniveau (zie [Ontwerpdetails: Magazijninstelling](design-details-warehouse-setup.md))</span><span class="sxs-lookup"><span data-stu-id="a8014-110">Complexity level (See [Design Details: Warehouse Setup](design-details-warehouse-setup.md))</span></span>|  
|------------|---------------------|----------|--------------|----------------|--------------------------------------------------------------------------------------------------------------------|  
|<span data-ttu-id="a8014-111">A</span><span class="sxs-lookup"><span data-stu-id="a8014-111">A</span></span>|<span data-ttu-id="a8014-112">Ontvangst en opslag van de orderregel boeken</span><span class="sxs-lookup"><span data-stu-id="a8014-112">Post receipt and put-away from the order line</span></span>|<span data-ttu-id="a8014-113">X</span><span class="sxs-lookup"><span data-stu-id="a8014-113">X</span></span>|||<span data-ttu-id="a8014-114">2</span><span class="sxs-lookup"><span data-stu-id="a8014-114">2</span></span>|  
|<span data-ttu-id="a8014-115">B</span><span class="sxs-lookup"><span data-stu-id="a8014-115">B</span></span>|<span data-ttu-id="a8014-116">Ontvangst en opslag van een voorraadopslagdocument boeken</span><span class="sxs-lookup"><span data-stu-id="a8014-116">Post receipt and put-away from an inventory put-away document</span></span>|||<span data-ttu-id="a8014-117">X</span><span class="sxs-lookup"><span data-stu-id="a8014-117">X</span></span>|<span data-ttu-id="a8014-118">3</span><span class="sxs-lookup"><span data-stu-id="a8014-118">3</span></span>|  
|<span data-ttu-id="a8014-119">L</span><span class="sxs-lookup"><span data-stu-id="a8014-119">C</span></span>|<span data-ttu-id="a8014-120">Ontvangst en opslag van een magazijnontvangstdocument boeken</span><span class="sxs-lookup"><span data-stu-id="a8014-120">Post receipt and put-away from a warehouse receipt document</span></span>||<span data-ttu-id="a8014-121">X</span><span class="sxs-lookup"><span data-stu-id="a8014-121">X</span></span>||<span data-ttu-id="a8014-122">5-4-6</span><span class="sxs-lookup"><span data-stu-id="a8014-122">4/5/6</span></span>|  
|<span data-ttu-id="a8014-123">D</span><span class="sxs-lookup"><span data-stu-id="a8014-123">D</span></span>|<span data-ttu-id="a8014-124">Ontvangst van een magazijnontvangstdocument en opslag van een magazijnopslagdocument boeken</span><span class="sxs-lookup"><span data-stu-id="a8014-124">Post receipt from a warehouse receipt document and post put-away from a warehouse put-away document</span></span>||<span data-ttu-id="a8014-125">X</span><span class="sxs-lookup"><span data-stu-id="a8014-125">X</span></span>|<span data-ttu-id="a8014-126">X</span><span class="sxs-lookup"><span data-stu-id="a8014-126">X</span></span>|<span data-ttu-id="a8014-127">5-4-6</span><span class="sxs-lookup"><span data-stu-id="a8014-127">4/5/6</span></span>|  

<span data-ttu-id="a8014-128">Zie voor meer informatie [Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md).</span><span class="sxs-lookup"><span data-stu-id="a8014-128">For more information, see [Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md).</span></span>  

<span data-ttu-id="a8014-129">De volgende procedure geeft methode B in de vorige tabel weer.</span><span class="sxs-lookup"><span data-stu-id="a8014-129">The following walkthrough demonstrates method B in the previous table.</span></span>  

## <a name="about-this-walkthrough"></a><span data-ttu-id="a8014-130">Informatie over deze procedure</span><span class="sxs-lookup"><span data-stu-id="a8014-130">About This Walkthrough</span></span>  
<span data-ttu-id="a8014-131">In standaardmagazijnconfiguraties waarbij voor uw vestiging de verwerking van opslag, maar niet van ontvangst vereist is, gebruikt u het venster **Voorraadopslag** om opslag- en ontvangstinformatie voor de inkomende brondocumenten te verzamelen en boeken.</span><span class="sxs-lookup"><span data-stu-id="a8014-131">In basic warehouse configurations where your location is set up to require put-away processing but not receive processing, you use the **Inventory Put-away** window to record and post put-away and receipt information for your inbound source documents.</span></span> <span data-ttu-id="a8014-132">Het inkomende brondocument kan een inkooporder zijn, maar ook een verkoopretourorder, een inkomende transferorder of een productieorder met output die kan worden opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="a8014-132">The inbound source document can be a purchase order, sales return order, inbound transfer order, or production order with output that is ready to be put away.</span></span>

> [!NOTE]
> <span data-ttu-id="a8014-133">Hoewel de instellingen **Pick vereist** en **Opslag vereist** worden genoemd, kunt u nog wel ontvangsten en verzendingen rechtstreeks vanuit de bronbedrijfsdocumenten boeken voor vestigingen waarvoor u deze selectievakjes inschakelt.</span><span class="sxs-lookup"><span data-stu-id="a8014-133">Even though the settings are called **Require Pick** and **Require Put-away**, you can still post receipts and shipments directly from the source business documents at locations where you select these check boxes.</span></span>  

<span data-ttu-id="a8014-134">In deze procedure worden de volgende taken gedemonstreerd.</span><span class="sxs-lookup"><span data-stu-id="a8014-134">This walkthrough demonstrates the following tasks.</span></span>  

-   <span data-ttu-id="a8014-135">Locatie ZILVER instellen voor voorraadopslag.</span><span class="sxs-lookup"><span data-stu-id="a8014-135">Setting up SILVER location for inventory put aways.</span></span>  
-   <span data-ttu-id="a8014-136">Locatie ZILVER instellen voor opslaglocatieverwerking.</span><span class="sxs-lookup"><span data-stu-id="a8014-136">Setting up SILVER location for bin handling.</span></span>  
-   <span data-ttu-id="a8014-137">Een standaardopslaglocatie voor artikel LS-81 definiëren.</span><span class="sxs-lookup"><span data-stu-id="a8014-137">Defining a default bin for item LS-81.</span></span> <span data-ttu-id="a8014-138">(LS-75 is al ingesteld in CRONUS.)</span><span class="sxs-lookup"><span data-stu-id="a8014-138">(LS-75 is already set up in CRONUS.)</span></span>  
-   <span data-ttu-id="a8014-139">Maak een inkooporder voor leverancier 10000 voor 40 luidsprekers.</span><span class="sxs-lookup"><span data-stu-id="a8014-139">Creating a purchase order for vendor 10000 for 40 loudspeakers.</span></span>  
-   <span data-ttu-id="a8014-140">Controleren of de opslaglocaties vooringesteld zijn.</span><span class="sxs-lookup"><span data-stu-id="a8014-140">Verifying that the put-away bins are preset by setup.</span></span>  
-   <span data-ttu-id="a8014-141">De inkooporder vrijgeven voor magazijnverwerking.</span><span class="sxs-lookup"><span data-stu-id="a8014-141">Releasing the purchase order for warehouse handling.</span></span>  
-   <span data-ttu-id="a8014-142">Een voorraadopslag maken op basis van een vrijgegeven brondocument.</span><span class="sxs-lookup"><span data-stu-id="a8014-142">Creating an inventory put-away based on a released source document.</span></span>  
-   <span data-ttu-id="a8014-143">Verifiëren dat de opslaglocaties worden overgenomen van de inkooporder.</span><span class="sxs-lookup"><span data-stu-id="a8014-143">Verifying that the put-away bins are inherited from the purchase order.</span></span>  
-   <span data-ttu-id="a8014-144">De magazijnverplaatsing in het magazijn vastleggen en tegelijkertijd de inkoopontvangst voor de broninkooporder boeken.</span><span class="sxs-lookup"><span data-stu-id="a8014-144">Registering the warehouse movement into the warehouse and at the same time posting the purchase receipt for the source purchase order.</span></span>  

## <a name="roles"></a><span data-ttu-id="a8014-145">Rollen</span><span class="sxs-lookup"><span data-stu-id="a8014-145">Roles</span></span>  
<span data-ttu-id="a8014-146">In dit overzicht worden taken gedemonstreerd voor de volgende gebruikersrollen:</span><span class="sxs-lookup"><span data-stu-id="a8014-146">This walkthrough demonstrates tasks that are performed by the following user roles:</span></span>  

-   <span data-ttu-id="a8014-147">Magazijnbeheerder</span><span class="sxs-lookup"><span data-stu-id="a8014-147">Warehouse Manager</span></span>  
-   <span data-ttu-id="a8014-148">Inkoper</span><span class="sxs-lookup"><span data-stu-id="a8014-148">Purchasing Agent</span></span>  
-   <span data-ttu-id="a8014-149">Magazijnmedewerker</span><span class="sxs-lookup"><span data-stu-id="a8014-149">Warehouse Worker</span></span>  

## <a name="prerequisites"></a><span data-ttu-id="a8014-150">Vereisten</span><span class="sxs-lookup"><span data-stu-id="a8014-150">Prerequisites</span></span>  
<span data-ttu-id="a8014-151">U moet het volgende doen om deze procedure uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="a8014-151">To complete this walkthrough, you will need:</span></span>  

-   <span data-ttu-id="a8014-152">CRONUS International Ltd. installeren.</span><span class="sxs-lookup"><span data-stu-id="a8014-152">CRONUS International Ltd. installed.</span></span>  
-   <span data-ttu-id="a8014-153">Maak van uzelf een magazijnwerknemer bij vestiging ZILVER door de volgende stappen uit te voeren:</span><span class="sxs-lookup"><span data-stu-id="a8014-153">To make yourself a warehouse employee at SILVER location by following these steps:</span></span>  

    1.  <span data-ttu-id="a8014-154">Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Magazijnwerknemers** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="a8014-154">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Warehouse Employees**, and then choose the related link.</span></span>  
    2.  <span data-ttu-id="a8014-155">Kies het veld **Gebruikers-ID** en selecteer uw eigen gebruikersaccount in het venster **Gebruikers**.</span><span class="sxs-lookup"><span data-stu-id="a8014-155">Choose the **User ID** field, and select your own user account in the **Users** window.</span></span>  
    3.  <span data-ttu-id="a8014-156">Voer ZILVER in het veld **Vestiging** in.</span><span class="sxs-lookup"><span data-stu-id="a8014-156">In the **Location Code** field, enter SILVER.</span></span>  
    4.  <span data-ttu-id="a8014-157">Selecteer het veld **Standaard**.</span><span class="sxs-lookup"><span data-stu-id="a8014-157">Select the **Default** field.</span></span>  

## <a name="story"></a><span data-ttu-id="a8014-158">Scenario</span><span class="sxs-lookup"><span data-stu-id="a8014-158">Story</span></span>  
<span data-ttu-id="a8014-159">Ellen, de magazijnmanager bij CRONUS International Ltd., maakt een inkooporder voor 10 eenheden van artikel LS-75 en 30 eenheden van artikel LS-81 van leverancier 10000 om te worden afgeleverd bij magazijn ZILVER.</span><span class="sxs-lookup"><span data-stu-id="a8014-159">Ellen, the warehouse manager at CRONUS International Ltd., creates a purchase order for 10 units of item LS-75 and 30 units of item LS-81 from vendor 10000 to be delivered to SILVER Warehouse.</span></span> <span data-ttu-id="a8014-160">Wanneer de bezorging in het magazijn aankomt, zet de magazijnmedewerker Johanna de artikelen in de standaardopslaglocaties die voor de artikelen zijn gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="a8014-160">When the delivery arrives at the warehouse, John, the warehouse worker, puts the items away in default bins defined for the items.</span></span> <span data-ttu-id="a8014-161">Wanneer Johanna de voorraadopslag boekt, worden de artikelen als ontvangen en beschikbaar voor verkoop of andere oproepen in de voorraad.</span><span class="sxs-lookup"><span data-stu-id="a8014-161">When John posts the put-away, the items are posted as received into inventory and available for sale or other demand.</span></span>  

## <a name="setting-up-the-location"></a><span data-ttu-id="a8014-162">De locatie instellen</span><span class="sxs-lookup"><span data-stu-id="a8014-162">Setting up the Location</span></span>  
 <span data-ttu-id="a8014-163">De instellingen van het venster **Vestiging** definiëren de magazijnstromen van het bedrijf.</span><span class="sxs-lookup"><span data-stu-id="a8014-163">The setup of the **Location Card** window defines the company’s warehouse flows.</span></span>  

### <a name="to-set-up-the-location"></a><span data-ttu-id="a8014-164">De vestiging instellen</span><span class="sxs-lookup"><span data-stu-id="a8014-164">To set up the location</span></span>  

1.  <span data-ttu-id="a8014-165">Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Locaties** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="a8014-165">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Locations**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a8014-166">Open de vestigingskaart ZILVER.</span><span class="sxs-lookup"><span data-stu-id="a8014-166">Open the SILVER location card.</span></span>  
3.  <span data-ttu-id="a8014-167">Selecteer het selectievakje **Opslag vereist**.</span><span class="sxs-lookup"><span data-stu-id="a8014-167">Select the **Require Put-away** check box.</span></span>  

    <span data-ttu-id="a8014-168">Ga door met het instellen van een standaardopslaglocatie voor de twee artikelnummers om te bepalen waar deze worden opgeslagen.</span><span class="sxs-lookup"><span data-stu-id="a8014-168">Proceed to set up a default bin for the two item numbers to control where they are put away.</span></span>  

4.  <span data-ttu-id="a8014-169">Kies de actie **Opslaglocaties**.</span><span class="sxs-lookup"><span data-stu-id="a8014-169">Choose the **Bins** action.</span></span>  
5.  <span data-ttu-id="a8014-170">Selecteer de eerste rij voor opslaglocatie S-01-0001 en kies vervolgens de actie **Inhoud**.</span><span class="sxs-lookup"><span data-stu-id="a8014-170">Select the first row, for bin S-01-0001, and then choose the **Contents** action.</span></span>  

    <span data-ttu-id="a8014-171">U ziet in het venster **Opslaglocatie-inhoud** dat artikel LS-75 al is ingesteld als inhoud in opslaglocatie S-01-0001.</span><span class="sxs-lookup"><span data-stu-id="a8014-171">Notice in the **Bin Content** window that item LS-75 is already set up as content in bin S-01-0001.</span></span>  

6.  <span data-ttu-id="a8014-172">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="a8014-172">Choose the **New** action.</span></span>  
7.  <span data-ttu-id="a8014-173">Selecteer de velden **Vast** en **Standaard**.</span><span class="sxs-lookup"><span data-stu-id="a8014-173">Select the **Fixed** and the **Default** fields.</span></span>  
8.  <span data-ttu-id="a8014-174">Voer in het veld **Artikelnr.** de waarde LS-81 in.</span><span class="sxs-lookup"><span data-stu-id="a8014-174">In the **Item No.** field, enter LS-81.</span></span>  

## <a name="creating-the-purchase-order"></a><span data-ttu-id="a8014-175">De inkooporder maken</span><span class="sxs-lookup"><span data-stu-id="a8014-175">Creating the Purchase Order</span></span>  
<span data-ttu-id="a8014-176">Inkooporders zijn de meest gebruikte soort inkomend brondocument.</span><span class="sxs-lookup"><span data-stu-id="a8014-176">Purchase orders are the most common type of inbound source document.</span></span>  

### <a name="to-create-the-purchase-order"></a><span data-ttu-id="a8014-177">De inkooporder maken</span><span class="sxs-lookup"><span data-stu-id="a8014-177">To create the purchase order</span></span>  

1.  <span data-ttu-id="a8014-178">Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Inkooporders** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="a8014-178">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Purchase Orders**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a8014-179">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="a8014-179">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="a8014-180">Maak een inkooporder voor leverancier 10000 op 23 januari (werkdatum) met de volgende inkooporderregels.</span><span class="sxs-lookup"><span data-stu-id="a8014-180">Create a purchase order for vendor 10000 on the work date (January 23) with the following purchase order lines.</span></span>  

    |<span data-ttu-id="a8014-181">Artikel</span><span class="sxs-lookup"><span data-stu-id="a8014-181">Item</span></span>|<span data-ttu-id="a8014-182">Vestiging</span><span class="sxs-lookup"><span data-stu-id="a8014-182">Location code</span></span>|<span data-ttu-id="a8014-183">Opslaglocatie</span><span class="sxs-lookup"><span data-stu-id="a8014-183">Bin code</span></span>|<span data-ttu-id="a8014-184">Aantal</span><span class="sxs-lookup"><span data-stu-id="a8014-184">Quantity</span></span>|  
    |----------|-------------------|--------------|--------------|  
    |<span data-ttu-id="a8014-185">LS_75</span><span class="sxs-lookup"><span data-stu-id="a8014-185">LS_75</span></span>|<span data-ttu-id="a8014-186">ZILVER</span><span class="sxs-lookup"><span data-stu-id="a8014-186">SILVER</span></span>|<span data-ttu-id="a8014-187">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="a8014-187">S-01-0001</span></span>|<span data-ttu-id="a8014-188">10</span><span class="sxs-lookup"><span data-stu-id="a8014-188">10</span></span>|  
    |<span data-ttu-id="a8014-189">LS-81</span><span class="sxs-lookup"><span data-stu-id="a8014-189">LS-81</span></span>|<span data-ttu-id="a8014-190">ZILVER</span><span class="sxs-lookup"><span data-stu-id="a8014-190">SILVER</span></span>|<span data-ttu-id="a8014-191">S-01-0001</span><span class="sxs-lookup"><span data-stu-id="a8014-191">S-01-0001</span></span>|<span data-ttu-id="a8014-192">30</span><span class="sxs-lookup"><span data-stu-id="a8014-192">30</span></span>|  

    > [!NOTE]  
    >  <span data-ttu-id="a8014-193">De opslaglocatiecode wordt automatisch ingevoerd op basis van de instellingen die u in de sectie 'De locatie instellen' heeft uitgevoerd.</span><span class="sxs-lookup"><span data-stu-id="a8014-193">The bin code is entered automatically according to the setup that you performed in the “Setting up the Location” section.</span></span>  

    <span data-ttu-id="a8014-194">Ga door om het magazijn te informeren dat de inkooporder klaar is voor de magazijnverwerking wanneer de bezorging aankomt.</span><span class="sxs-lookup"><span data-stu-id="a8014-194">Proceed to notify the warehouse that the purchase order is ready for warehouse handling when the delivery arrives.</span></span>  

4.  <span data-ttu-id="a8014-195">Kies de actie **Vrijgeven**.</span><span class="sxs-lookup"><span data-stu-id="a8014-195">Choose the **Release** action.</span></span>  

    <span data-ttu-id="a8014-196">Het leveren van luidsprekers van leverancier 10000 is aangekomen op magazijn SILVER en Jan bergt ze op.</span><span class="sxs-lookup"><span data-stu-id="a8014-196">The delivery of loudspeakers from vendor 10000 has arrived at SILVER warehouse, and John proceeds to put them away.</span></span>  

## <a name="receiving-and-putting-the-items-away"></a><span data-ttu-id="a8014-197">De artikelen ontvangen en opslaan</span><span class="sxs-lookup"><span data-stu-id="a8014-197">Receiving and Putting the Items Away</span></span>  
<span data-ttu-id="a8014-198">In het venster **Voorraadopslag** kunt u alle inkomende magazijnactiviteiten voor een bepaald brondocument beheren, zoals een inkooporder.</span><span class="sxs-lookup"><span data-stu-id="a8014-198">In the **Inventory Put-away** window, you can manage all inbound warehouse activities for a specific source document, such as a purchase order.</span></span>  

### <a name="to-receive-and-put-the-items-away"></a><span data-ttu-id="a8014-199">De artikelen ontvangen en opslaan</span><span class="sxs-lookup"><span data-stu-id="a8014-199">To receive and put the items away</span></span>  

1.  <span data-ttu-id="a8014-200">Kies het pictogram ![lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Voorraadopslag** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="a8014-200">Choose the ![Lightbulb that opens the Tell Me feature](media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Inventory Put-aways**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="a8014-201">Kies de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="a8014-201">Choose the **New** action.</span></span>  
3.  <span data-ttu-id="a8014-202">Selecteer het veld **Brondocument** en selecteer vervolgens **Inkooporder**.</span><span class="sxs-lookup"><span data-stu-id="a8014-202">Select the **Source Document** field, and then select **Purchase Order**.</span></span>  
4.  <span data-ttu-id="a8014-203">Selecteer het veld **Bronnr.**, selecteer de regel voor de inkoop van leverancier 10000, en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8014-203">Select the **Source No.** field, select the line for the purchase from vendor 10000, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="a8014-204">Of kies op het tabblad **Acties** in de groep **Functies** de optie **Brondocument ophalen** en selecteer de inkooporder.</span><span class="sxs-lookup"><span data-stu-id="a8014-204">Alternatively, on the **Actions** tab, in the **Functions** group, choose **Get Source Document**, and then select the purchase order.</span></span>  

5.  <span data-ttu-id="a8014-205">Kies de actie **Te verwerken aantal autom. invullen**.</span><span class="sxs-lookup"><span data-stu-id="a8014-205">Choose the **Autofill Qty. to Handle** action.</span></span>  

    <span data-ttu-id="a8014-206">Of voer in het veld **Te verwerken aantal** respectievelijk 10 en 30 in op de twee voorraadopslagregels.</span><span class="sxs-lookup"><span data-stu-id="a8014-206">Alternatively, in the **Qty. to Handle** field, enter 10 and 30 respectively on the two inventory put-away lines.</span></span>  

6.  <span data-ttu-id="a8014-207">Kies de actie **Boeken**, selecteer de actie **Ontvangen** en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="a8014-207">Choose the **Post** action, select the **Receive** action, and then choose the **OK** button.</span></span>  

    <span data-ttu-id="a8014-208">Nu zijn de 40 luidsprekers geregistreerd als opgeslagen in opslaglocatie S-01-0001 en een positieve artikelpost is gemaakt om de geboekte inkoopontvangst te weerspiegelen.</span><span class="sxs-lookup"><span data-stu-id="a8014-208">The 40 loudspeakers are now registered as put away in bin S-01-0001, and a positive item ledger entry is created reflecting the posted purchase receipt.</span></span>  

## <a name="see-also"></a><span data-ttu-id="a8014-209">Zie ook</span><span class="sxs-lookup"><span data-stu-id="a8014-209">See Also</span></span>  
 <span data-ttu-id="a8014-210">[Artikelen opslaan met voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-210">[Put Items Away with Inventory Put-aways](warehouse-how-to-put-items-away-with-inventory-put-aways.md) </span></span>  
 <span data-ttu-id="a8014-211">[Standaardmagazijnen met bewerkingsgebieden instellen](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-211">[Set Up Basic Warehouses with Operations Areas](warehouse-how-to-set-up-basic-warehouses-with-operations-areas.md) </span></span>  
 <span data-ttu-id="a8014-212">[Onderdelen verplaatsen naar een bewerkingsgebied in standaardmagazijnconfiguraties](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-212">[Move Components to an Operation Area in Basic Warehouse Configurations](warehouse-how-to-move-components-to-an-operation-area-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="a8014-213">[Picken voor productie of assemblage](warehouse-how-to-pick-for-production.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-213">[Pick for Production or Assembly](warehouse-how-to-pick-for-production.md) </span></span>  
 <span data-ttu-id="a8014-214">[Artikelen ad hoc verplaatsen in standaardmagazijnconfiguraties](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-214">[Move Items Ad Hoc in Basic Warehouse Configurations](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md) </span></span>  
 <span data-ttu-id="a8014-215">[Ontwerpdetails: Inkomende magazijnstroom](design-details-inbound-warehouse-flow.md) </span><span class="sxs-lookup"><span data-stu-id="a8014-215">[Design Details: Inbound Warehouse Flow](design-details-inbound-warehouse-flow.md) </span></span>  
 [<span data-ttu-id="a8014-216">Procedures voor bedrijfsprocessen</span><span class="sxs-lookup"><span data-stu-id="a8014-216">Business Process Walkthroughs</span></span>](walkthrough-business-process-walkthroughs.md)  
 <span data-ttu-id="a8014-217">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="a8014-217">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

