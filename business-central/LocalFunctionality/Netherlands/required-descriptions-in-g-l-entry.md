---
title: Verplichte beschrijvingen in grootboekpost
description: Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2019
ms.author: sgroespe
ms.openlocfilehash: a0cea30a2b4d295d9ac3180a8da94c14af696040
ms.sourcegitcommit: 60b87e5eb32bb408dd65b9855c29159b1dfbfca8
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/29/2019
ms.locfileid: "1241471"
---
# <a name="required-descriptions-in-g-l-entry"></a><span data-ttu-id="e6e4a-103">Verplichte beschrijvingen in grootboekpost</span><span class="sxs-lookup"><span data-stu-id="e6e4a-103">Required Descriptions in G-L Entry</span></span>
<span data-ttu-id="e6e4a-104">Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-104">When entering general journal lines on a form, the system fills in automatically the description field.</span></span> <span data-ttu-id="e6e4a-105">Deze omschrijving wordt ook opgeslagen in de grootboekpost na het boeken van het dagboek.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-105">This description will also be stored in the G/L entry after posting the journal.</span></span> <span data-ttu-id="e6e4a-106">Voor een goede auditprocedure is een meer gedetailleerde omschrijving wenselijk wanneer u een dagboekregel van de soort Grootboekrekening boekt.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-106">For a good audit trail, a more detailed description is desirable, when you post a journal line of type G/L Account.</span></span>  

<span data-ttu-id="e6e4a-107">Om een gebruiker te dwingen een meer gedetailleerde omschrijving in te voeren, is het mogelijk te kiezen of het systeem automatisch de omschrijving van de grootboekrekening moet invullen of het veld leeg laten.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-107">To force the user to enter a more detailed description, it is possible to choose if the system must fill in automatically the description of the G/L account or leave the field blank.</span></span> <span data-ttu-id="e6e4a-108">Als het veld **Standaardbeschrijv. in dagboek weglaten** op de pagina **Grootboekrekening** is aangevinkt, wordt het veld **Omschrijving** voor die grootboekrekening niet ingevuld wanneer dit wordt geselecteerd in een algemene dagboekregel.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-108">If the **Omit Default Descr. in Jnl. Field** check box on the **G/L Account Card** page is checked, the system will not fill in the **Description** field for that G/L account when selected in a general journal line.</span></span>  

<span data-ttu-id="e6e4a-109">Wanneer de dagboekregels worden geboekt, wordt door het systeem gecontroleerd of alle velden **Omschrijving** zijn ingevuld.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-109">When posting the journal lines, the system will check if all the **Description** fields are filled in.</span></span> <span data-ttu-id="e6e4a-110">Als er een blanco omschrijving is, wordt een foutmelding gegeven.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-110">If there is a blank description, an error message will appear.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="e6e4a-111">Het leeg laten van het omschrijvingsveld en controleren of alle omschrijvingsvelden zijn ingevuld vóór het boeken, wordt alleen gedaan in de memoriaalpagina's op verscheidene plaatsen in de module en op de pagina's van Kas, Bank, Giro.</span><span class="sxs-lookup"><span data-stu-id="e6e4a-111">Leaving the description field blank and check if all the description fields are filled in before posting, will only be done on the general journal pages in several application areas and on the local Cash Bank Giro pages.</span></span>  

## <a name="see-also"></a><span data-ttu-id="e6e4a-112">Zie ook</span><span class="sxs-lookup"><span data-stu-id="e6e4a-112">See Also</span></span>  
 [<span data-ttu-id="e6e4a-113">Grootboek</span><span class="sxs-lookup"><span data-stu-id="e6e4a-113">General Ledger</span></span>](general-ledger.md)
