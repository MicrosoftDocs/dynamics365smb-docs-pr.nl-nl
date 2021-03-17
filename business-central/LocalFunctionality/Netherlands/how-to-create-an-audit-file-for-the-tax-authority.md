---
title: Een auditfile voor de belastingdienst maken
description: Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen. Basistransacties worden gewoonlijk via dagboekposten verwerkt.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 881f8f796ac6a27d5deb75a9d267a84f7b21a105
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382835"
---
# <a name="create-an-audit-file-for-the-tax-authority"></a><span data-ttu-id="56de3-104">Een auditfile voor de belastingdienst maken</span><span class="sxs-lookup"><span data-stu-id="56de3-104">Create an Audit File for the Tax Authority</span></span>
<span data-ttu-id="56de3-105">Tijdens een controle van de boeken voor een boekjaar kan een belastinginspecteur om gegevens over de basistransacties vanuit het grootboek voor dat boekjaar vragen.</span><span class="sxs-lookup"><span data-stu-id="56de3-105">During an examination of the books for a fiscal year, a tax inspector can ask for data about the basis transactions from the general ledger for that fiscal year.</span></span> <span data-ttu-id="56de3-106">Basistransacties worden gewoonlijk via dagboekposten verwerkt.</span><span class="sxs-lookup"><span data-stu-id="56de3-106">Basis transactions usually are processed via journal entries.</span></span> <span data-ttu-id="56de3-107">Daarom vormen de dagboekposten de basis voor het auditbestand.</span><span class="sxs-lookup"><span data-stu-id="56de3-107">That is the reason why the journal entries are the basis for the audit file.</span></span>  

 <span data-ttu-id="56de3-108">De belastingdienst stimuleert bedrijven om het auditfile te gebruiken, maar dat is niet verplicht.</span><span class="sxs-lookup"><span data-stu-id="56de3-108">The tax authority stimulates companies to use the audit file but it is not prescribed.</span></span>  

 <span data-ttu-id="56de3-109">De auditfile kan tevens worden gebruikt om gegevens uit te wisselen tussen bedrijven.</span><span class="sxs-lookup"><span data-stu-id="56de3-109">The audit file can also be used to exchange data between companies.</span></span> <span data-ttu-id="56de3-110">U kunt elke gewenste periode selecteren, maar de begindatum en einddatum van de opgegeven periode moeten in hetzelfde boekjaar liggen.</span><span class="sxs-lookup"><span data-stu-id="56de3-110">You can select every period you want, but the start and end date of the entered period must be in the same fiscal year.</span></span>  

## <a name="to-make-an-audit-file"></a><span data-ttu-id="56de3-111">Een auditfile maken</span><span class="sxs-lookup"><span data-stu-id="56de3-111">To make an Audit file</span></span>  

1.  <span data-ttu-id="56de3-112">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Belastingdienst - Auditfile** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="56de3-112">Choose the ![Lightbulb that opens the Tell Me feature](../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Tax Authority - Audit File**, and then choose the related link.</span></span>  
2.  <span data-ttu-id="56de3-113">Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.</span><span class="sxs-lookup"><span data-stu-id="56de3-113">On the **Options** FastTab, fill in the fields as described in the following table.</span></span>  

    |<span data-ttu-id="56de3-114">Veld</span><span class="sxs-lookup"><span data-stu-id="56de3-114">Field</span></span>|<span data-ttu-id="56de3-115">Description</span><span class="sxs-lookup"><span data-stu-id="56de3-115">Description</span></span>|  
    |---------------------------------|---------------------------------------|  
    |<span data-ttu-id="56de3-116">**Begindatum**</span><span class="sxs-lookup"><span data-stu-id="56de3-116">**Start Date**</span></span>|<span data-ttu-id="56de3-117">Geef de begindatum of de periode op waarop de gegevens moeten worden gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="56de3-117">Specify the start date of the period on which the data must be based.</span></span>|  
    |<span data-ttu-id="56de3-118">**Einddatum**</span><span class="sxs-lookup"><span data-stu-id="56de3-118">**End Date**</span></span>|<span data-ttu-id="56de3-119">Geef de einddatum of de periode op waarop de gegevens moeten worden gebaseerd.</span><span class="sxs-lookup"><span data-stu-id="56de3-119">Specify the end date of the period on which the data must be based.</span></span>|  
    |<span data-ttu-id="56de3-120">**Beginsaldo uitsluiten**</span><span class="sxs-lookup"><span data-stu-id="56de3-120">**Exclude Begin Balance**</span></span>|<span data-ttu-id="56de3-121">Geeft op of het auditbestand het beginsaldo moet bevatten van grootboekrekeningen.</span><span class="sxs-lookup"><span data-stu-id="56de3-121">Specifies if the audit file must contain the begin balance of general ledger accounts.</span></span><br /><br /> <span data-ttu-id="56de3-122">Het veld kan worden bewerkt als de begindatum van de periode gelijk is aan de begindatum van een boekjaar.</span><span class="sxs-lookup"><span data-stu-id="56de3-122">The field is editable if the start date of the period is equal to the start date of a fiscal year.</span></span>|  

3.  <span data-ttu-id="56de3-123">Kies de knop **OK** om het auditbestand te maken.</span><span class="sxs-lookup"><span data-stu-id="56de3-123">Choose the **OK** button to create the audit file.</span></span> <span data-ttu-id="56de3-124">Als u het auditbestand niet wilt maken, kiest u de knop **Annuleren** om de pagina te sluiten.</span><span class="sxs-lookup"><span data-stu-id="56de3-124">If you do not want to create the audit file, choose the **Cancel** button to close the page.</span></span>  

<span data-ttu-id="56de3-125">Wanneer u het rapport uitvoert, moet u de naam en locatie van het geëxporteerde bestand opgeven.</span><span class="sxs-lookup"><span data-stu-id="56de3-125">When you run the report, you must specify the name and location of the exported file.</span></span> <span data-ttu-id="56de3-126">De standaardbestandsnaam is **audit.xaf**, maar u kunt dat wijzigen.</span><span class="sxs-lookup"><span data-stu-id="56de3-126">The default file name is **audit.xaf**, but you can change that.</span></span> <span data-ttu-id="56de3-127">De bestandsextensie moet .xaf zijn.</span><span class="sxs-lookup"><span data-stu-id="56de3-127">The file extension must be .xaf.</span></span>  

## <a name="see-also"></a><span data-ttu-id="56de3-128">Zie ook</span><span class="sxs-lookup"><span data-stu-id="56de3-128">See Also</span></span>  
 [<span data-ttu-id="56de3-129">Elektronische btw- en ICP-aangiften verzenden</span><span class="sxs-lookup"><span data-stu-id="56de3-129">Submitting Electronic VAT and ICP Declarations</span></span>](electronic-vat-and-icp-declarations.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]