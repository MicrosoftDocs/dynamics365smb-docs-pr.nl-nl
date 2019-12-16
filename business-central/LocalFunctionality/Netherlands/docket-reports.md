---
title: Borderelrapporten
description: Met de Nederlandse toepassing voor telebankieren kunt u posten voor dezelfde klant of leverancier die dezelfde transactiewijze hebben tot één betaal- of verzamelopdracht voor de bank combineren.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: f42666fe51014665c46036c414ad7adc6660cf3b
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881363"
---
# <a name="docket-reports"></a><span data-ttu-id="55c98-103">Borderelrapporten</span><span class="sxs-lookup"><span data-stu-id="55c98-103">Docket Reports</span></span>
<span data-ttu-id="55c98-104">Met de Nederlandse toepassing voor telebankieren kunt u posten voor dezelfde klant of leverancier die dezelfde transactiewijze hebben tot één betaal- of verzamelopdracht voor de bank combineren.</span><span class="sxs-lookup"><span data-stu-id="55c98-104">The Dutch telebanking application allows you to combine ledger entries for the same customer or vendor, having the same transaction mode, into one payment or collection order to the bank.</span></span> <span data-ttu-id="55c98-105">Als zodanig wordt één totaalbedrag betaald aan of geïnd van de betreffende leverancier of klant.</span><span class="sxs-lookup"><span data-stu-id="55c98-105">As such one total amount will be paid to or collected from the vendor or customer involved.</span></span> <span data-ttu-id="55c98-106">Mogelijk bevat deze gecombineerde betaling alle detailgegevens over de afzonderlijke betalingen of incasso's.</span><span class="sxs-lookup"><span data-stu-id="55c98-106">Possibly this combined payment could lack all detail information about the individual payments or collections.</span></span> <span data-ttu-id="55c98-107">Telebankieren biedt u de mogelijkheid om uw leverancier of klant gedetailleerd te informeren door een borderelrapport te genereren waarin de afzonderlijke betalingen worden beschreven waaruit het totale betaalde of geïnde bedrag bestaat.</span><span class="sxs-lookup"><span data-stu-id="55c98-107">Telebanking offers you the possibility to inform your vendor or customer in detail by generating a docket report that describes the individual payments that constitute the total amount paid or collected.</span></span>  

<span data-ttu-id="55c98-108">Tijdens het genereren van betalingsvoorstellen met de batchverwerking **Voorstelposten ophalen** wordt het selectievakje **Borderel** van het voorstel automatisch ingeschakeld als:</span><span class="sxs-lookup"><span data-stu-id="55c98-108">When generating payment proposals using the **Get Proposal Entries** batch job the system will select the **Docket** check box on the proposal in case that:</span></span>  

- <span data-ttu-id="55c98-109">De resulterende gecombineerde betaling te veel factuurnummers bevat om deze weer te geven in de vier beschikbare omschrijvingsvelden van de nieuwe voorstelregel: de velden **Omschrijving 1**, **Omschrijving 2**, **Omschrijving 3** en **Omschrijving 4**.</span><span class="sxs-lookup"><span data-stu-id="55c98-109">The resulting combined payment includes too many invoice numbers to list them in the available four description fields of the new proposal line: **Description 1** field, **Description 2** field, **Description 3** field, and **Description 4** field.</span></span>  

- <span data-ttu-id="55c98-110">De betaling niet is gebaseerd op een factuur.</span><span class="sxs-lookup"><span data-stu-id="55c98-110">The payment is not based upon an invoice.</span></span>  

## <a name="see-also"></a><span data-ttu-id="55c98-111">Zie ook</span><span class="sxs-lookup"><span data-stu-id="55c98-111">See Also</span></span>  
 [<span data-ttu-id="55c98-112">Telebankieren</span><span class="sxs-lookup"><span data-stu-id="55c98-112">Telebanking</span></span>](telebanking.md)
