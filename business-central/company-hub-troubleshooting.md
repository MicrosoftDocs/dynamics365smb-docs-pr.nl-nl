---
title: Problemen met uw bedrijfshub oplossen
description: Leer hoe u problemen omzeilt in de bedrijfshub in Dynamics 365 Business Central.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: accountant, accounting, troubleshoot
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 3f348de3e8116efd789f85f1b011ecc7013bf2b1
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3927640"
---
# <a name="troubleshooting-your-company-hub"></a><span data-ttu-id="cc499-103">Problemen met uw bedrijfshub oplossen</span><span class="sxs-lookup"><span data-stu-id="cc499-103">Troubleshooting Your Company Hub</span></span>

<span data-ttu-id="cc499-104">Bedrijven toevoegen aan de bedrijfshub is gemakkelijk, maar in dit artikel komen problemen aan bod die zich onderweg kunnen voordoen.</span><span class="sxs-lookup"><span data-stu-id="cc499-104">Adding companies to the company hub dashboard is easy enough, but this article addresses issues that you may have on the way.</span></span>  

## <a name="check-errors"></a><span data-ttu-id="cc499-105">Controleren op fouten</span><span class="sxs-lookup"><span data-stu-id="cc499-105">Check errors</span></span>

<span data-ttu-id="cc499-106">Gebruik de actie **Fouten controleren** om een lijst met recente fouten te bekijken.</span><span class="sxs-lookup"><span data-stu-id="cc499-106">Use the **Check Errors** action to view a list of recent errors.</span></span> <span data-ttu-id="cc499-107">U kunt voor elke fout aanvullende details zien en u kunt het logboek opschonen door oudere vermeldingen te verwijderen.</span><span class="sxs-lookup"><span data-stu-id="cc499-107">You can see additional details for each error, and you can clean up the log by deleting older entries.</span></span>  

## <a name="connection-failed"></a><span data-ttu-id="cc499-108">Verbinding mislukt</span><span class="sxs-lookup"><span data-stu-id="cc499-108">Connection failed</span></span>

<span data-ttu-id="cc499-109">Er kan een aantal redenen zijn waarom u geen verbinding kunt maken met een bedrijf, waaronder de volgende:</span><span class="sxs-lookup"><span data-stu-id="cc499-109">There can be a couple of reasons why you cannot connect to a company, including the following:</span></span>

- <span data-ttu-id="cc499-110">De URL in het veld **Omgevingskoppeling** is ongeldig</span><span class="sxs-lookup"><span data-stu-id="cc499-110">The URL in the **Environment Link** field is not valid</span></span>  

  <span data-ttu-id="cc499-111">Ga naar de pagina **Omgevingskoppelingen**, open de omgeving waarmee u geen verbinding kunt maken en kies vervolgens de actie **De verbinding testen**.</span><span class="sxs-lookup"><span data-stu-id="cc499-111">Go to the **Environment Links** page, open the environment that you cannot connect to, and then choose the **Test the connection** action.</span></span>  
- <span data-ttu-id="cc499-112">Het bedrijf van de cliënt is momenteel offline, bijvoorbeeld als dit wordt bijgewerkt</span><span class="sxs-lookup"><span data-stu-id="cc499-112">The client's company is currently offline, for example if it being upgraded</span></span>

  <span data-ttu-id="cc499-113">Kies in het dashboard de menuopdracht **Extra** en vervolgens **Fouten controleren**.</span><span class="sxs-lookup"><span data-stu-id="cc499-113">In your dashboard, choose the **Tools** menu item, and then choose **Check Errors**.</span></span> <span data-ttu-id="cc499-114">Vervolgens wordt er een lijst met technische gegevens weergegeven. Als u fouten ziet, kunt u contact opnemen met uw beheerder.</span><span class="sxs-lookup"><span data-stu-id="cc499-114">This opens a list with technical details, so you might want to contact your administrator if you're seeing errors.</span></span> <span data-ttu-id="cc499-115">Het foutbericht "*De server heeft de cliëntreferenties geweigerd*" wijst erop dat u geen toegang hebt.</span><span class="sxs-lookup"><span data-stu-id="cc499-115">For example, the error message "*The server has rejected the client credentials*" suggests that you do not have access.</span></span>  
- <span data-ttu-id="cc499-116">U hebt geen toegang tot alle bedrijven in de omgeving waarmee u verbinding probeert te maken</span><span class="sxs-lookup"><span data-stu-id="cc499-116">You do not have access to all companies in the environment that you are trying to connect to</span></span>

  <span data-ttu-id="cc499-117">In [!INCLUDE [prodshort](includes/prodshort.md)] kan een organisatie meerdere bedrijfsunits hebben, bedrijven genaamd, en hebt u mogelijk geen toegang tot alle bedrijven.</span><span class="sxs-lookup"><span data-stu-id="cc499-117">In [!INCLUDE [prodshort](includes/prodshort.md)], an organization can have multiple business units called companies, and you might not have access to all companies.</span></span> <span data-ttu-id="cc499-118">Werk samen met uw beheerder of cliënt om ervoor te zorgen dat u toegang hebt tot de bedrijven waarin u moet werken.</span><span class="sxs-lookup"><span data-stu-id="cc499-118">Work with your administrator or client to make sure that you have access to the companies that you have to work in.</span></span>  

## <a name="data-does-not-refresh"></a><span data-ttu-id="cc499-119">Gegevens worden niet vernieuwd</span><span class="sxs-lookup"><span data-stu-id="cc499-119">Data does not refresh</span></span>

<span data-ttu-id="cc499-120">Wanneer u een bedrijf toevoegt of om vernieuwen van de gegevens verzoekt, worden de gegevens opgehaald door [!INCLUDE [prodshort](includes/prodshort.md)].</span><span class="sxs-lookup"><span data-stu-id="cc499-120">When you add a company or request a refresh of the data, [!INCLUDE [prodshort](includes/prodshort.md)] fetches the data.</span></span> <span data-ttu-id="cc499-121">U moet de pagina echter zelf vernieuwen, bijvoorbeeld door de actie **Alle bedrijven opnieuw laden** te kiezen, de browserpagina te vernieuwen of uit en vervolgens weer naar het dashboard te navigeren.</span><span class="sxs-lookup"><span data-stu-id="cc499-121">But you must refresh the page yourself, such as choosing the **Reload all companies** action, refresh the browser page, navigate away from the dashboard and then back again, or similar.</span></span>  

<span data-ttu-id="cc499-122">Als u een bedrijf hebt toegevoegd, maar het wordt niet weergegeven in de lijst, kunt u ook de actie **Alle bedrijven opnieuw laden** gebruiken om de lijst bij te werken.</span><span class="sxs-lookup"><span data-stu-id="cc499-122">If you've added a company but it is not displaying in the list, you can also use the **Reload all companies** action to update the list.</span></span>

## <a name="see-also"></a><span data-ttu-id="cc499-123">Zie ook</span><span class="sxs-lookup"><span data-stu-id="cc499-123">See also</span></span>

[<span data-ttu-id="cc499-124">Werk beheren tussen meerdere bedrijven in de bedrijfshub</span><span class="sxs-lookup"><span data-stu-id="cc499-124">Manage Work across Multiple Companies in the Company Hub</span></span>](company-hub.md)  
[<span data-ttu-id="cc499-125">Bedrijven toevoegen aan uw bedrijfshub</span><span class="sxs-lookup"><span data-stu-id="cc499-125">Add companies to your company hub</span></span>](company-hub-add-company.md)  
[<span data-ttu-id="cc499-126">Accountantervaringen in Business Central</span><span class="sxs-lookup"><span data-stu-id="cc499-126">Accountant Experiences in Business Central</span></span>](finance-accounting.md)  