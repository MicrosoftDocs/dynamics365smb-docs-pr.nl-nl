---
title: Postcode-updates importeren
description: "Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken."
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
ms.openlocfilehash: 15a74f1b7e47fccd35ff8f9c4b096a747a951661
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="import-post-code-updates"></a><span data-ttu-id="8fe3c-104">Updates van postcodes importeren</span><span class="sxs-lookup"><span data-stu-id="8fe3c-104">Import Post Code Updates</span></span>
<span data-ttu-id="8fe3c-105">Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-105">Every month a post code file will be delivered with all post code mutations in a month.</span></span> <span data-ttu-id="8fe3c-106">Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-106">This post code file can be imported and update the relevant data of the **Post Code Range** table.</span></span>  

## <a name="to-import-the-update-file"></a><span data-ttu-id="8fe3c-107">Het updatebestand importeren</span><span class="sxs-lookup"><span data-stu-id="8fe3c-107">To import the update file</span></span>  

1.  <span data-ttu-id="8fe3c-108">Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Postcode-updates** in en kies vervolgens de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-108">Choose the ![Search for Page or Report](../../media/ui-search/search_small.png "Search for Page or Report icon") icon, enter **Post Codes Updates**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="8fe3c-109">Kies in het venster **Postcode-updates** de actie **Postcodes-update importeren**.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-109">In the **Post Codes Updates** window, choose the **Import Post Codes Update** action.</span></span>  
3.  <span data-ttu-id="8fe3c-110">Geef het pad en de naam op van het postcode-updatebestand en kies vervolgens de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-110">Specify the path and name of the post code update file, and then choose the **OK** button.</span></span> <span data-ttu-id="8fe3c-111">Als u het bestand niet wilt importeren, kiest u de knop **Annuleren** om het venster te sluiten.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-111">If you do not want to import the file, choose the **Cancel** button to close the window.</span></span>  

<span data-ttu-id="8fe3c-112">Als geen bestand met een volledige set postcodegegevens is geïmporteerd, verschijnt er een bericht.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-112">If there is no file imported with a full set of post code data, then a message appears.</span></span>  

<span data-ttu-id="8fe3c-113">Voordat de postcodes worden bijgewerkt, worden de volgende controles uitgevoerd:</span><span class="sxs-lookup"><span data-stu-id="8fe3c-113">Before updating the post codes the following checks will be performed:</span></span>  

- <span data-ttu-id="8fe3c-114">Is er al een updatebestand geïmporteerd met een recenter datumveld dan de datum van dit nieuwe updatebestand?</span><span class="sxs-lookup"><span data-stu-id="8fe3c-114">Is there already an update file imported with a Date Field later then the date of this new update file?</span></span> <span data-ttu-id="8fe3c-115">Als dat het geval is, wordt het proces gestopt.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-115">If so then the process will stop.</span></span>  

- <span data-ttu-id="8fe3c-116">Is er een lange periode tussen de datum van dit bestand en de waarde in het datumveld van het laatst geïmporteerde bestand?</span><span class="sxs-lookup"><span data-stu-id="8fe3c-116">Is there a gap between the date of this file and the value in the Date Field field for the last imported file?</span></span> <span data-ttu-id="8fe3c-117">Als dat het geval is, verschijnt er een bericht.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-117">If there is a gap then a message appears.</span></span> <span data-ttu-id="8fe3c-118">U kunt kiezen of u het updatebestand nog steeds wilt importeren.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-118">You can choose if you still want to import the update file.</span></span>  

<span data-ttu-id="8fe3c-119">Gegevens over de geïmporteerde postcode worden opgeslagen in de tabel Postcode-update logpost.</span><span class="sxs-lookup"><span data-stu-id="8fe3c-119">Information about the imported post code will be saved in the Post Code Update Log Entry Table table.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8fe3c-120">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8fe3c-120">See Also</span></span>  
[<span data-ttu-id="8fe3c-121">Nederlandse postcodes</span><span class="sxs-lookup"><span data-stu-id="8fe3c-121">Dutch Post Codes</span></span>](dutch-post-codes.md)

