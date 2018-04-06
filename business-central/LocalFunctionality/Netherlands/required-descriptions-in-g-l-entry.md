---
title: Verplichte beschrijvingen in grootboekpost
description: Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld.
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
ms.openlocfilehash: 8903c2d80fbdfe52a7350e0e81e508a791f3bc51
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="required-descriptions-in-g-l-entry"></a><span data-ttu-id="8138a-103">Verplichte beschrijvingen in grootboekpost</span><span class="sxs-lookup"><span data-stu-id="8138a-103">Required Descriptions in G-L Entry</span></span>
<span data-ttu-id="8138a-104">Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld.</span><span class="sxs-lookup"><span data-stu-id="8138a-104">When entering general journal lines on a form, the system fills in automatically the description field.</span></span> <span data-ttu-id="8138a-105">Deze omschrijving wordt ook opgeslagen in de grootboekpost na het boeken van het dagboek.</span><span class="sxs-lookup"><span data-stu-id="8138a-105">This description will also be stored in the G/L entry after posting the journal.</span></span> <span data-ttu-id="8138a-106">Voor een goede auditprocedure is een meer gedetailleerde omschrijving wenselijk wanneer u een dagboekregel van de soort Grootboekrekening boekt.</span><span class="sxs-lookup"><span data-stu-id="8138a-106">For a good audit trail, a more detailed description is desirable, when you post a journal line of type G/L Account.</span></span>  

<span data-ttu-id="8138a-107">Om een gebruiker te dwingen een meer gedetailleerde omschrijving in te voeren, is het mogelijk te kiezen of het systeem automatisch de omschrijving van de grootboekrekening moet invullen of het veld leeg laten.</span><span class="sxs-lookup"><span data-stu-id="8138a-107">To force the user to enter a more detailed description, it is possible to choose if the system must fill in automatically the description of the G/L account or leave the field blank.</span></span> <span data-ttu-id="8138a-108">Als het veld **Standaardbeschrijv. in dagboek weglaten** in het venster **Grootboekrekening** is aangevinkt, wordt het veld **Omschrijving** voor die grootboekrekening niet ingevuld wanneer dit wordt geselecteerd in een algemene dagboekregel.</span><span class="sxs-lookup"><span data-stu-id="8138a-108">If the **Omit Default Descr. in Jnl. Field** check box in the **G/L Account Card** window is checked, the system will not fill in the **Description** field for that G/L account when selected in a general journal line.</span></span>  

<span data-ttu-id="8138a-109">Wanneer de dagboekregels worden geboekt, wordt door het systeem gecontroleerd of alle velden **Omschrijving** zijn ingevuld.</span><span class="sxs-lookup"><span data-stu-id="8138a-109">When posting the journal lines, the system will check if all the **Description** fields are filled in.</span></span> <span data-ttu-id="8138a-110">Als er een blanco omschrijving is, wordt een foutmelding gegeven.</span><span class="sxs-lookup"><span data-stu-id="8138a-110">If there is a blank description, an error message will appear.</span></span>  

> [!NOTE]  
>  <span data-ttu-id="8138a-111">Het leeg laten van het omschrijvingsveld en controleren of alle omschrijvingsvelden zijn ingevuld vóór het boeken, wordt alleen gedaan in de memoriaalvensters op verscheidene plaatsen in de module en in de vensters van Kas, Bank, Giro.</span><span class="sxs-lookup"><span data-stu-id="8138a-111">Leaving the description field blank and check if all the description fields are filled in before posting, will only be done on the general journal windows in several application areas and on the local Cash Bank Giro windows.</span></span>  

## <a name="see-also"></a><span data-ttu-id="8138a-112">Zie ook</span><span class="sxs-lookup"><span data-stu-id="8138a-112">See Also</span></span>  
 [<span data-ttu-id="8138a-113">Grootboek</span><span class="sxs-lookup"><span data-stu-id="8138a-113">General Ledger</span></span>](general-ledger.md)

