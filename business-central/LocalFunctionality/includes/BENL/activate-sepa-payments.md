---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 08/26/2020
ms.author: edupont
ms.openlocfilehash: 432d0d4457ecf36427452b699dcf3b9c51d5a006
ms.sourcegitcommit: 3e2eab6920e96596cb4b3c61e590a8c577e8b630
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/27/2020
ms.locfileid: "3731362"
---
<span data-ttu-id="f011b-101">Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen in uw bedrijf.</span><span class="sxs-lookup"><span data-stu-id="f011b-101">To submit vendor payments electronically in Single Euro Payments Area (SEPA) ISO 20022 payment format, you must set up prerequisites for enabling SEPA payments in your company.</span></span>  

<span data-ttu-id="f011b-102">In de volgende procedures wordt beschreven hoe u SEPA-betalingen instelt, inclusief hoe u de instellingen voor specifieke leveranciers wijzigt.</span><span class="sxs-lookup"><span data-stu-id="f011b-102">The following procedures describe how to set up SEPA payments, including how to modify the setup for specific vendors.</span></span>  

## <a name="to-enable-countriesregions-for-sepa"></a><span data-ttu-id="f011b-103">Landen/regio's activeren voor SEPA</span><span class="sxs-lookup"><span data-stu-id="f011b-103">To enable countries/regions for SEPA</span></span>  

1. <span data-ttu-id="f011b-104">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Landen/regio's** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f011b-104">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Countries/Regions**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f011b-105">Kies de actie **Lijst bewerken**.</span><span class="sxs-lookup"><span data-stu-id="f011b-105">Choose the **Edit List** action.</span></span>  
3. <span data-ttu-id="f011b-106">Schakel het selectievakje **SEPA toegestaan** in voor elk land/regio dat u wilt activeren voor SEPA.</span><span class="sxs-lookup"><span data-stu-id="f011b-106">Select the **SEPA Allowed** check box for each country or region that you want to enable for SEPA.</span></span>  
4. <span data-ttu-id="f011b-107">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f011b-107">Choose the **OK** button.</span></span>  

## <a name="to-enable-bank-accounts-for-sepa"></a><span data-ttu-id="f011b-108">Bankrekeningen activeren voor SEPA</span><span class="sxs-lookup"><span data-stu-id="f011b-108">To enable bank accounts for SEPA</span></span>  

1. <span data-ttu-id="f011b-109">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="f011b-109">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Bank Accounts**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f011b-110">Selecteer de bankrekening die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="f011b-110">Select the bank account that you want to enable for SEPA, and then choose the **Edit** action.</span></span>  
3. <span data-ttu-id="f011b-111">Selecteer in het veld **Land-/regiocode** van het sneltabblad **Algemeen** de gewenste code.</span><span class="sxs-lookup"><span data-stu-id="f011b-111">On the **General** FastTab, in the **Country/Region Code** field, select the appropriate code.</span></span>  

    > [!NOTE]  
    > <span data-ttu-id="f011b-112">De opgegeven land-/regiocode moet zijn geactiveerd voor SEPA, zoals is beschreven in de vorige procedure.</span><span class="sxs-lookup"><span data-stu-id="f011b-112">The specified country/region code must be enabled for SEPA as described in the previous procedure.</span></span>  

4. <span data-ttu-id="f011b-113">Geef een waarde op in het veld **Minimumsaldo**.</span><span class="sxs-lookup"><span data-stu-id="f011b-113">Enter a value in the **Min. Balance** field.</span></span>  
5. <span data-ttu-id="f011b-114">Geef in het veld **SWIFT-code** van het sneltabblad **Transfer** een code op.</span><span class="sxs-lookup"><span data-stu-id="f011b-114">On the **Transfer** FastTab, in the **SWIFT Code** field, enter a code.</span></span>  
6. <span data-ttu-id="f011b-115">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f011b-115">Choose the **OK** button.</span></span>  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a><span data-ttu-id="f011b-116">Een SEPA ISO 20022-exportprotocol instellen</span><span class="sxs-lookup"><span data-stu-id="f011b-116">To set up a SEPA ISO 20022 export protocol</span></span>  

1. <span data-ttu-id="f011b-117">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Exportprotocollen** in en kies de gerelateerde koppeling.</span><span class="sxs-lookup"><span data-stu-id="f011b-117">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Export Protocols**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f011b-118">Kies op de pagina **Exportprotocollen** de actie **Nieuw**.</span><span class="sxs-lookup"><span data-stu-id="f011b-118">On the **Export Protocols** page, choose the **New** action.</span></span>  
3. <span data-ttu-id="f011b-119">Vul de velden in.</span><span class="sxs-lookup"><span data-stu-id="f011b-119">Fill in the fields.</span></span> [!INCLUDE [tooltip-inline-tip_md](../../../includes/tooltip-inline-tip_md.md)]
4. <span data-ttu-id="f011b-120">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f011b-120">Choose the **OK** button.</span></span>  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a><span data-ttu-id="f011b-121">Bankrekeningen van leveranciers instellen voor SEPA</span><span class="sxs-lookup"><span data-stu-id="f011b-121">To set up vendor bank accounts for SEPA</span></span>  

1. <span data-ttu-id="f011b-122">Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies de desbetreffende koppeling.</span><span class="sxs-lookup"><span data-stu-id="f011b-122">Choose the ![Lightbulb that opens the Tell Me feature](../../../media/ui-search/search_small.png "Tell me what you want to do") icon, enter **Vendors**, and then choose the related link.</span></span>  
2. <span data-ttu-id="f011b-123">Selecteer de betreffende leverancier en kies vervolgens de actie **Bankrekeningen**.</span><span class="sxs-lookup"><span data-stu-id="f011b-123">Select the relevant vendor, and then choose the **Bank Accounts** action.</span></span>  
3. <span data-ttu-id="f011b-124">Selecteer de bankrekening van de leverancier die u wilt instellen voor SEPA, en kies vervolgens de actie **Bewerken**.</span><span class="sxs-lookup"><span data-stu-id="f011b-124">Select the vendor bank account to set up for SEPA, and then choose the **Edit** action.</span></span>  
4. <span data-ttu-id="f011b-125">Geef in de velden **IBAN** en **SWIFT-code** van het sneltabblad **Transfer** de internationale bankidentificatiecode op van de bank waarbij de leverancier de rekening heeft.</span><span class="sxs-lookup"><span data-stu-id="f011b-125">On the **Transfer** FastTab, in the **IBAN** and **SWIFT Code** fields, enter the international bank identifier code of the bank where the vendor has the account.</span></span>  
5. <span data-ttu-id="f011b-126">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="f011b-126">Choose the **OK** button.</span></span>  
