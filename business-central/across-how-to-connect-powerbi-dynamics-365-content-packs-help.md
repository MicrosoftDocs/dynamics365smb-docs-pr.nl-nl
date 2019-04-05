---
title: Power BI verbinden met Business Central | Microsoft Docs
description: Inzicht, bedrijfsinformatie en KPI's krijgen uit uw Business Central-gegevens is gemakkelijk met Power BI en de Business Central-inhoudspakketten.
author: SusanneWindfeldPedersen
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: account schedule, analysis, reporting, financial report, business intelligence, KPI
ms.date: 10/01/2018
ms.author: solsen
redirect_url: admin-powerbi
ms.openlocfilehash: 48c57e03f4679ea05792304fe13bdf896be2f1e3
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "794799"
---
# <a name="connecting-power-bi-to-dynamics-365-business-central-content-packs"></a><span data-ttu-id="b4c93-103">Power BI verbinden met Dynamics 365 Business Central-inhoudspakketten</span><span class="sxs-lookup"><span data-stu-id="b4c93-103">Connecting Power BI to Dynamics 365 Business Central Content Packs</span></span>
<span data-ttu-id="b4c93-104">Inzicht krijgen in uw Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-gegevens is gemakkelijk met Power BI en de Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-inhoudspakketten.</span><span class="sxs-lookup"><span data-stu-id="b4c93-104">Getting insights into your Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data is easy with Power BI and the Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] content packs.</span></span> <span data-ttu-id="b4c93-105">Power BI haalt uw gegevens op en maakt vervolgens een kant-en-klaar dashboard en rapporteert op basis van die gegevens.</span><span class="sxs-lookup"><span data-stu-id="b4c93-105">Power BI retrieves your data then builds an out-of-the-box dashboard and reports based on that data.</span></span>

<span data-ttu-id="b4c93-106">U moet een geldig account bij Dynamics 365 en Power BI hebben.</span><span class="sxs-lookup"><span data-stu-id="b4c93-106">You must have a valid account with Dynamics 365 and with Power BI.</span></span> <span data-ttu-id="b4c93-107">Ook moet u [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) downloaden als u uw eigen Power BI-rapporten wilt maken.</span><span class="sxs-lookup"><span data-stu-id="b4c93-107">Also, you must download [Power BI Desktop](https://powerbi.microsoft.com/en-us/desktop/) if you wish to create your own Power BI reports.</span></span> <span data-ttu-id="b4c93-108">Voor Power BI-inhoudspakketten zijn machtigingen vereist voor de tabellen waaruit de gegevens worden opgehaald.</span><span class="sxs-lookup"><span data-stu-id="b4c93-108">Power BI content packs require permissions to the tables where data is retrieved from.</span></span> <span data-ttu-id="b4c93-109">Meer details over de vereisten worden verderop beschreven.</span><span class="sxs-lookup"><span data-stu-id="b4c93-109">More details on the requirements are described below.</span></span>  

## <a name="how-to-connect"></a><span data-ttu-id="b4c93-110">Verbinding maken</span><span class="sxs-lookup"><span data-stu-id="b4c93-110">How to Connect</span></span>
1. <span data-ttu-id="b4c93-111">Selecteer **Gegevens ophalen** onder in het linkernavigatiedeelvenster.</span><span class="sxs-lookup"><span data-stu-id="b4c93-111">Select **Get Data** at the bottom of the left navigation pane.</span></span>  
<span data-ttu-id="b4c93-112">![Navigeren om gegevens op te halen](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span><span class="sxs-lookup"><span data-stu-id="b4c93-112">![Navigating to Get Data](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-get-data.png)</span></span>

<span data-ttu-id="b4c93-113">U kunt ook aan de slag gaan vanuit Dynamics 365 Business Edition.</span><span class="sxs-lookup"><span data-stu-id="b4c93-113">You may also get starting from within Dynamics 365 Business Edition.</span></span> <span data-ttu-id="b4c93-114">Navigeer in het rolcentrum naar **Rapportselectie** in het onderdeel Power BI-rolcentrum.</span><span class="sxs-lookup"><span data-stu-id="b4c93-114">From the role center, navigate to **Report Selection** in the Power BI Role Center part.</span></span> <span data-ttu-id="b4c93-115">Selecteer **Service** of **Mijn organisatie** vanuit het lint.</span><span class="sxs-lookup"><span data-stu-id="b4c93-115">Select either **Service** or **My Organization** from the ribbon.</span></span> <span data-ttu-id="b4c93-116">Wanneer een van deze acties wordt geselecteerd, gaat u naar de Organisatiegalerie in Power BI of naar de servicebibliotheek in Power BI, die ook wordt gefilterd op alleen weergave van inhoudspakketten die verband houden met [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b4c93-116">When either of these actions are selected, you will be taken to either the Organization gallery in Power BI or to the services library in Power BI, which will also be filtered to only display content packs related to [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span>

2. <span data-ttu-id="b4c93-117">Selecteer **Ophalen** in het vak **Diensten**.</span><span class="sxs-lookup"><span data-stu-id="b4c93-117">In the **Services** box, select **Get**.</span></span> <span data-ttu-id="b4c93-118">Hierdoor wordt een pagina geopend met de **AppSource** en **Apps voor Power BI-apps**.</span><span class="sxs-lookup"><span data-stu-id="b4c93-118">This will open a page with the **AppSource** and **Apps for Power BI apps**.</span></span>  
<span data-ttu-id="b4c93-119">![Inhoudspakketten kiezen uit online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span><span class="sxs-lookup"><span data-stu-id="b4c93-119">![Choose content packs from online services](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-online-services-get.png)</span></span>
3. <span data-ttu-id="b4c93-120">Selecteer **Apps** op het tabblad **Apps voor Power BI-apps** en kies het **Microsoft Dynamics 365 Business Central**-inhoudspakket dat u wilt gebruiken. Selecteer vervolgens **Nu ophalen**.</span><span class="sxs-lookup"><span data-stu-id="b4c93-120">Select **Apps** from the **Apps for Power BI apps** tab, choose the **Microsoft Dynamics 365 Business Central** content pack that you want to use, and then select **Get it now**.</span></span>  
<span data-ttu-id="b4c93-121">![Selecteer Dynamics 365 Business Central en selecteer Nu ophalen](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span><span class="sxs-lookup"><span data-stu-id="b4c93-121">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-dynamics365-for-financials-get-it-now.png)</span></span>
4. <span data-ttu-id="b4c93-122">Voer wanneer daarom wordt gevraagd de naam van *uw bedrijf* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b4c93-122">When prompted, enter the name of *your company* in [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="b4c93-123">Dit is niet de weergavenaam.</span><span class="sxs-lookup"><span data-stu-id="b4c93-123">This is not the display name.</span></span> <span data-ttu-id="b4c93-124">De bedrijfsnaam kan op de pagina Bedrijven worden gevonden binnen uw [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)]-exemplaar.</span><span class="sxs-lookup"><span data-stu-id="b4c93-124">The company name can be found on the 'Companies' page within your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] instance.</span></span> 
<span data-ttu-id="b4c93-125">![Selecteer Dynamics 365 Business Central en selecteer Nu ophalen](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span><span class="sxs-lookup"><span data-stu-id="b4c93-125">![Select Dynamics 365 Business Central and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-connect-to-d365-finance-and-operations-crm.png)</span></span>
5. <span data-ttu-id="b4c93-126">Nadat verbinding is gemaakt, worden automatisch een dashboard, rapport en gegevensset geladen in uw Power BI-werkruimte.</span><span class="sxs-lookup"><span data-stu-id="b4c93-126">Once connected, a dashboard, report and dataset will automatically be loaded into your Power BI workspace.</span></span> <span data-ttu-id="b4c93-127">Wanneer dit is voltooid, worden de tegels bijgewerkt met gegevens uit uw [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)]-bedrijf.</span><span class="sxs-lookup"><span data-stu-id="b4c93-127">When completed, the tiles will update with data from your [!INCLUDE[d365fin_md](includes/d365fin_long_md.md)] company.</span></span>
<span data-ttu-id="b4c93-128">![Selecteer Dynamics 365 Business Central en selecteer Nu ophalen](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span><span class="sxs-lookup"><span data-stu-id="b4c93-128">![Select Dynamics 365 Business Central  and select Get it now](./media/across-how-to-connect-powerbi-d365-content-packs/powerbi-workspace-dashboard-report-dataset.png)</span></span>

## <a name="what-now"></a><span data-ttu-id="b4c93-129">Wat nu?</span><span class="sxs-lookup"><span data-stu-id="b4c93-129">What Now?</span></span>

- <span data-ttu-id="b4c93-130">Probeer [een vraag te stellen in het vraag- en antwoordvak](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) boven aan het dashboard.</span><span class="sxs-lookup"><span data-stu-id="b4c93-130">Try [asking a question in the Q&A box](https://docs.microsoft.com/en-us/power-bi/service-q-and-a) at the top of the dashboard.</span></span>
- <span data-ttu-id="b4c93-131">[Wijzig de tegels](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in het dashboard.</span><span class="sxs-lookup"><span data-stu-id="b4c93-131">[Change the tiles](https://docs.microsoft.com/en-us/power-bi/service-dashboard-edit-tile) in the dashboard.</span></span>  
- <span data-ttu-id="b4c93-132">[Selecteer een tegel](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) om het onderliggende rapport te openen.</span><span class="sxs-lookup"><span data-stu-id="b4c93-132">[Select a tile](https://docs.microsoft.com/en-us/power-bi/service-dashboard-tiles) to open the underlying report.</span></span>  
- <span data-ttu-id="b4c93-133">Terwijl uw gegevensset wordt gepland om dagelijks te worden vernieuwd, kunt u het vernieuwingsschema wijzigen of op verzoek proberen te vernieuwen met **Nu vernieuwen**.</span><span class="sxs-lookup"><span data-stu-id="b4c93-133">While your dataset will be scheduled to refreshed daily, you can change the refresh schedule or try refreshing it on demand using **Refresh Now**.</span></span>

## <a name="system-requirements"></a><span data-ttu-id="b4c93-134">Systeemvereisten</span><span class="sxs-lookup"><span data-stu-id="b4c93-134">System Requirements</span></span>
<span data-ttu-id="b4c93-135">Als u uw [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-gegevens in Power BI wilt importeren, moet u machtigingen hebben voor de webservices die worden gebruikt om gegevens op te halen.</span><span class="sxs-lookup"><span data-stu-id="b4c93-135">To import your [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] data into Power BI, you need to have permissions to the web services used to retrieve data.</span></span> <span data-ttu-id="b4c93-136">De webservices die voor elk inhoudspakket vereist zijn omvatten:</span><span class="sxs-lookup"><span data-stu-id="b4c93-136">The web services required for each content pack include:</span></span>

## <a name="role-center-reports"></a><span data-ttu-id="b4c93-137">Rolcentrumrapporten</span><span class="sxs-lookup"><span data-stu-id="b4c93-137">Role Center Reports</span></span>

<span data-ttu-id="b4c93-138">**Microsoft Dynamics 365 Business Central – CRM**</span><span class="sxs-lookup"><span data-stu-id="b4c93-138">**Microsoft Dynamics 365 Business Central – CRM**</span></span>
- <span data-ttu-id="b4c93-139">Verkoopopportunities</span><span class="sxs-lookup"><span data-stu-id="b4c93-139">Sales Opportunities</span></span>
- <span data-ttu-id="b4c93-140">Excel-sjabloonweergave Bedrijf</span><span class="sxs-lookup"><span data-stu-id="b4c93-140">Excel Template View Company</span></span>
- <span data-ttu-id="b4c93-141">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-141">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-142">**Microsoft Dynamics 365 Business Central – Financiën**</span><span class="sxs-lookup"><span data-stu-id="b4c93-142">**Microsoft Dynamics 365 Business Central – Finance**</span></span>
- <span data-ttu-id="b4c93-143">PowerBIFinance</span><span class="sxs-lookup"><span data-stu-id="b4c93-143">PowerBIFinance</span></span>
- <span data-ttu-id="b4c93-144">Excel-sjabloonweergave Bedrijf</span><span class="sxs-lookup"><span data-stu-id="b4c93-144">Excel Template View Company</span></span>
- <span data-ttu-id="b4c93-145">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-145">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-146">**Microsoft Dynamics 365 Business Central – Taken**</span><span class="sxs-lookup"><span data-stu-id="b4c93-146">**Microsoft Dynamics 365 Business Central – Jobs**</span></span>
- <span data-ttu-id="b4c93-147">Projectoverzicht</span><span class="sxs-lookup"><span data-stu-id="b4c93-147">Job List</span></span>
- <span data-ttu-id="b4c93-148">Projectplanningsregels</span><span class="sxs-lookup"><span data-stu-id="b4c93-148">Job Planning Lines</span></span>
- <span data-ttu-id="b4c93-149">Projecttaakregels</span><span class="sxs-lookup"><span data-stu-id="b4c93-149">Job Task Lines</span></span>
- <span data-ttu-id="b4c93-150">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-150">Power BI Report Labels</span></span>
- <span data-ttu-id="b4c93-151">Excel-sjabloonweergave Bedrijf</span><span class="sxs-lookup"><span data-stu-id="b4c93-151">Excel Template View Company</span></span>

<span data-ttu-id="b4c93-152">**Microsoft Dynamics 365 Business Central - Verkoop**</span><span class="sxs-lookup"><span data-stu-id="b4c93-152">**Microsoft Dynamics 365 Business Central - Sales**</span></span>
- <span data-ttu-id="b4c93-153">Verkoopdashboard</span><span class="sxs-lookup"><span data-stu-id="b4c93-153">Sales Dashboard</span></span>
- <span data-ttu-id="b4c93-154">Excel-sjabloonweergave Bedrijf</span><span class="sxs-lookup"><span data-stu-id="b4c93-154">Excel Template View Company</span></span>
- <span data-ttu-id="b4c93-155">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-155">Power BI Report Labels</span></span>

## <a name="list-page-reports"></a><span data-ttu-id="b4c93-156">Lijstpaginarapporten</span><span class="sxs-lookup"><span data-stu-id="b4c93-156">List Page Reports</span></span> 

<span data-ttu-id="b4c93-157">**Microsoft Dynamics 365 Business Central – Klantenlijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-157">**Microsoft Dynamics 365 Business Central – Customers List**</span></span>
- <span data-ttu-id="b4c93-158">Artikelverkopen per klant</span><span class="sxs-lookup"><span data-stu-id="b4c93-158">Item Sales by Customer</span></span>
- <span data-ttu-id="b4c93-159">Power BI-artikelinkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-159">Power BI Item Purchase List</span></span>
- <span data-ttu-id="b4c93-160">Power BI-artikelverkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-160">Power BI Item Sales List</span></span>
- <span data-ttu-id="b4c93-161">Verkoopdashboard</span><span class="sxs-lookup"><span data-stu-id="b4c93-161">Sales Dashboard</span></span>
- <span data-ttu-id="b4c93-162">Power BI-klantenlijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-162">Power BI Customer List</span></span>
- <span data-ttu-id="b4c93-163">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-163">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-164">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-164">Power BI Report Labels</span></span> 

<span data-ttu-id="b4c93-165">**Microsoft Dynamics 365 Business Central - Lijst met algemene posten**</span><span class="sxs-lookup"><span data-stu-id="b4c93-165">**Microsoft Dynamics 365 Business Central - General Ledger Entries List**</span></span>
- <span data-ttu-id="b4c93-166">Power BI-lijst met grootboekbedragen</span><span class="sxs-lookup"><span data-stu-id="b4c93-166">Power BI GL Amount List</span></span>
- <span data-ttu-id="b4c93-167">Power BI gebudgetteerd grootboekbedrag</span><span class="sxs-lookup"><span data-stu-id="b4c93-167">Power BI GL Budgeted Amount</span></span>
- <span data-ttu-id="b4c93-168">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-168">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-169">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-169">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-170">**Microsoft Dynamics 365 Business Central – artikellijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-170">**Microsoft Dynamics 365 Business Central – Items List**</span></span>
- <span data-ttu-id="b4c93-171">Artikelverkopen per klant</span><span class="sxs-lookup"><span data-stu-id="b4c93-171">Item Sales by Customer</span></span>
- <span data-ttu-id="b4c93-172">Power BI-artikelinkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-172">Power BI Item Purchase List</span></span>
- <span data-ttu-id="b4c93-173">Power BI-artikelverkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-173">Power BI Item Sales List</span></span>
- <span data-ttu-id="b4c93-174">Verkoopdashboard</span><span class="sxs-lookup"><span data-stu-id="b4c93-174">Sales Dashboard</span></span>
- <span data-ttu-id="b4c93-175">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-175">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-176">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-176">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-177">**Microsoft Dynamics 365 Business Central – Takenlijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-177">**Microsoft Dynamics 365 Business Central – Jobs List**</span></span>
- <span data-ttu-id="b4c93-178">Power BI-takenlijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-178">Power BI Jobs List</span></span>
- <span data-ttu-id="b4c93-179">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-179">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-180">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-180">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-181">**Microsoft Dynamics 365 Business Central – Inkoopfacturenlijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-181">**Microsoft Dynamics 365 Business Central – Purchase Invoices List**</span></span>
- <span data-ttu-id="b4c93-182">Power BI-inkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-182">Power BI Purchase List</span></span>
- <span data-ttu-id="b4c93-183">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-183">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-184">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-184">Power BI Report Labels</span></span>

<span data-ttu-id="b4c93-185">**Microsoft Dynamics 365 Business Central – Verkooporderlijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-185">**Microsoft Dynamics 365 Business Central – Sales Orders List**</span></span>
- <span data-ttu-id="b4c93-186">Power BI-verkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-186">Power BI Sales List</span></span>
- <span data-ttu-id="b4c93-187">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-187">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-188">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-188">Power BI Report Labels</span></span>


<span data-ttu-id="b4c93-189">**Microsoft Dynamics 365 Business Central – Leverancierslijst**</span><span class="sxs-lookup"><span data-stu-id="b4c93-189">**Microsoft Dynamics 365 Business Central – Vendors List**</span></span>
- <span data-ttu-id="b4c93-190">Power BI-artikelinkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-190">Power BI Item Purchase List</span></span>
- <span data-ttu-id="b4c93-191">Power BI-artikelverkooplijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-191">Power BI Item Sales List</span></span>
- <span data-ttu-id="b4c93-192">Power BI-leverancierslijst</span><span class="sxs-lookup"><span data-stu-id="b4c93-192">Power BI Vendor List</span></span>
- <span data-ttu-id="b4c93-193">ExcelTemplateViewCompany</span><span class="sxs-lookup"><span data-stu-id="b4c93-193">ExcelTemplateViewCompany</span></span>
- <span data-ttu-id="b4c93-194">Labels van Power BI-rapport</span><span class="sxs-lookup"><span data-stu-id="b4c93-194">Power BI Report Labels</span></span>

## <a name="web-services"></a><span data-ttu-id="b4c93-195">Webservices</span><span class="sxs-lookup"><span data-stu-id="b4c93-195">Web Services</span></span>
<span data-ttu-id="b4c93-196">Een eenvoudige manier om de webservices te vinden is te zoeken naar webservices in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span><span class="sxs-lookup"><span data-stu-id="b4c93-196">An easy way to find the web services is to search for web services in [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)].</span></span> <span data-ttu-id="b4c93-197">In de lijst moet u ervoor zorgen het vakje Publiceren is gemarkeerd voor de hierboven genoemde webservices.</span><span class="sxs-lookup"><span data-stu-id="b4c93-197">In the list make sure the Publish box is marked for the web services listed above.</span></span>

## <a name="troubleshooting"></a><span data-ttu-id="b4c93-198">Problemen oplossen</span><span class="sxs-lookup"><span data-stu-id="b4c93-198">Troubleshooting</span></span>
<span data-ttu-id="b4c93-199">Het dashboard van Power BI gebruikt de gepubliceerde webservices die hierboven worden genoemd en bevat gegevens van het demobedrijf of uw eigen bedrijf als u gegevens importeert uit uw huidige financiële oplossing.</span><span class="sxs-lookup"><span data-stu-id="b4c93-199">The Power BI dashboard relies on the published web services that are listed above, and it will show data from the demonstration company or your own company if you import data from your current finance solution.</span></span> <span data-ttu-id="b4c93-200">Als er echter iets verkeerd gaat, biedt deze sectie een oplossing voor de meest voorkomende problemen.</span><span class="sxs-lookup"><span data-stu-id="b4c93-200">However, if something goes wrong, this section provides a workaround for the most typical issues.</span></span>

### <a name="incorrect-company-name"></a><span data-ttu-id="b4c93-201">Onjuiste bedrijfsnaam</span><span class="sxs-lookup"><span data-stu-id="b4c93-201">Incorrect Company Name</span></span>  
<span data-ttu-id="b4c93-202">Een veel voorkomende fout is de weergavenaam van het bedrijf in te voeren in plaats van de bedrijfsnaam.</span><span class="sxs-lookup"><span data-stu-id="b4c93-202">A common mistake is to enter the company display name instead of the company name.</span></span> <span data-ttu-id="b4c93-203">Als u de bedrijfsnaam wilt vinden, zoekt u naar **Bedrijven**.</span><span class="sxs-lookup"><span data-stu-id="b4c93-203">To find the company name search for **Companies**.</span></span> <span data-ttu-id="b4c93-204">Gebruik vervolgens het veld **Naam** wanneer u uw bedrijfsnaam invoert.</span><span class="sxs-lookup"><span data-stu-id="b4c93-204">Then use the **Name** field when entering your company name.</span></span>

### <a name="incorrect-user-name-and-password"></a><span data-ttu-id="b4c93-205">Onjuiste gebruikersnaam en wachtwoord</span><span class="sxs-lookup"><span data-stu-id="b4c93-205">Incorrect User Name and Password</span></span>  
<span data-ttu-id="b4c93-206">De gebruikersnaam en het wachtwoord die worden gebruikt om verbinding te maken, zijn hetzelfde als wat wordt gebruikt om verbinding te maken met uw Microsoft Office 365-account.</span><span class="sxs-lookup"><span data-stu-id="b4c93-206">The user name and password used to connect will be the same as what is used to connect to your Microsoft Office 365 account.</span></span>  

<span data-ttu-id="b4c93-207">De inhoudspakketten vereisen ook dat u een Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-account hebt.</span><span class="sxs-lookup"><span data-stu-id="b4c93-207">The content packs also require that you have a Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account.</span></span> <span data-ttu-id="b4c93-208">Zodra u uw aanmeldingsgegevens invoert, worden eventuele Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-tenants waartoe u toegang hebt, automatisch gevonden.</span><span class="sxs-lookup"><span data-stu-id="b4c93-208">Once you enter your credentials, we will auto discover any Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] tenants you have access to.</span></span> <span data-ttu-id="b4c93-209">Als u geen gelicentieerd of proef Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)]-account hebt, wordt een foutbericht weergegeven.</span><span class="sxs-lookup"><span data-stu-id="b4c93-209">If you do not have a licensed or trial Microsoft [!INCLUDE[d365fin_long_md](includes/d365fin_long_md.md)] account, you will receive an error message.</span></span>

### <a name="the-key-didnt-match-any-rows-in-the-table"></a><span data-ttu-id="b4c93-210">De sleutel kwam met geen rijen uit de tabel overeen</span><span class="sxs-lookup"><span data-stu-id="b4c93-210">The Key Didn't Match Any Rows in the Table</span></span>
<span data-ttu-id="b4c93-211">Als u een ongeldige bedrijfsnaam invoert tijdens het verbindingsproces, kunt u de foutmelding "De sleutel kwam met geen rijen uit de tabel overeen" krijgen.</span><span class="sxs-lookup"><span data-stu-id="b4c93-211">If you enter a non-valid company name during the connection process, you may get the error message "The key didn't match any rows in the table".</span></span> <span data-ttu-id="b4c93-212">Geef de juiste bedrijfsnaam op en probeer opnieuw verbinding te maken.</span><span class="sxs-lookup"><span data-stu-id="b4c93-212">Provide the correct company name and try connecting again.</span></span>

## <a name="see-also"></a><span data-ttu-id="b4c93-213">Zie ook</span><span class="sxs-lookup"><span data-stu-id="b4c93-213">See Also</span></span>
[<span data-ttu-id="b4c93-214">Aan de slag met Power BI</span><span class="sxs-lookup"><span data-stu-id="b4c93-214">Get started with Power BI</span></span>](https://docs.microsoft.com/en-us/power-bi/service-get-started)  
[<span data-ttu-id="b4c93-215">Power BI - Basisconcepten</span><span class="sxs-lookup"><span data-stu-id="b4c93-215">Power BI - Basic Concepts</span></span>](https://docs.microsoft.com/en-us/power-bi/service-basic-concepts)  
[<span data-ttu-id="b4c93-216">Bedrijfsinformatie</span><span class="sxs-lookup"><span data-stu-id="b4c93-216">Business Intelligence</span></span>](bi.md)  
[<span data-ttu-id="b4c93-217">Aan de slag</span><span class="sxs-lookup"><span data-stu-id="b4c93-217">Getting Started</span></span>](product-get-started.md)  
[<span data-ttu-id="b4c93-218">Bedrijfsgegevens importeren uit andere financiële systemen</span><span class="sxs-lookup"><span data-stu-id="b4c93-218">Importing Business Data from Other Finance Systems</span></span>](across-import-data-configuration-packages.md)  
<span data-ttu-id="b4c93-219">[Instellen van [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span><span class="sxs-lookup"><span data-stu-id="b4c93-219">[Setting Up [!INCLUDE[d365fin](includes/d365fin_md.md)]](setup.md)</span></span>  
[<span data-ttu-id="b4c93-220">Financiën</span><span class="sxs-lookup"><span data-stu-id="b4c93-220">Finance</span></span>](finance.md)  
<span data-ttu-id="b4c93-221">[Rapportage voor [!INCLUDE[d365fin](includes/d365fin_md.md)] instellen in Power BI](across-how-use-financials-data-source-powerbi.md)</span><span class="sxs-lookup"><span data-stu-id="b4c93-221">[Setup Reporting for [!INCLUDE[d365fin](includes/d365fin_md.md)] in Power BI](across-how-use-financials-data-source-powerbi.md)</span></span>  