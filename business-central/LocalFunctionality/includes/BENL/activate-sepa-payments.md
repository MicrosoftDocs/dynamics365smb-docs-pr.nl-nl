---
author: edupont04
ms.service: dynamics365-business-central
ms.topic: include
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 4830a9d3a70bc83c5f69e1746fd934803112e0ea
ms.sourcegitcommit: ddbb5cede750df1baba4b3eab8fbed6744b5b9d6
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/01/2020
ms.locfileid: "3916515"
---
Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen in uw bedrijf.  

In de volgende procedures wordt beschreven hoe u SEPA-betalingen instelt, inclusief hoe u de instellingen voor specifieke leveranciers wijzigt.  

## <a name="to-enable-countriesregions-for-sepa"></a>Landen/regio's activeren voor SEPA  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Landen/regio's** in en kies de gerelateerde koppeling.  
2. Kies de actie **Lijst bewerken**.  
3. Schakel het selectievakje **SEPA toegestaan** in voor elk land/regio dat u wilt activeren voor SEPA.  
4. Kies de knop **OK**.  

## <a name="to-enable-bank-accounts-for-sepa"></a>Bankrekeningen activeren voor SEPA  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.  
2. Selecteer de bankrekening die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.  
3. Selecteer in het veld **Land-/regiocode** van het sneltabblad **Algemeen** de gewenste code.  

    > [!NOTE]  
    > De opgegeven land-/regiocode moet zijn geactiveerd voor SEPA, zoals is beschreven in de vorige procedure.  

4. Geef een waarde op in het veld **Minimumsaldo**.  
5. Geef in het veld **SWIFT-code** van het sneltabblad **Transfer** een code op.  
6. Kies de knop **OK**.  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a>Een SEPA ISO 20022-exportprotocol instellen  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Exportprotocollen** in en kies de gerelateerde koppeling.  
2. Kies op de pagina **Exportprotocollen** de actie **Nieuw**.  
3. Vul de velden in. [!INCLUDE [tooltip-inline-tip_md](../../../includes/tooltip-inline-tip_md.md)]
4. Kies de knop **OK**.  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a>Bankrekeningen van leveranciers instellen voor SEPA  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies de desbetreffende koppeling.  
2. Selecteer de betreffende leverancier en kies vervolgens de actie **Bankrekeningen**.  
3. Selecteer de bankrekening van de leverancier die u wilt instellen voor SEPA, en kies vervolgens de actie **Bewerken**.  
4. Geef in de velden **IBAN** en **SWIFT-code** van het sneltabblad **Transfer** de internationale bankidentificatiecode op van de bank waarbij de leverancier de rekening heeft.  
5. Kies de knop **OK**.  
