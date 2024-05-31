---
title: Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-indeling (NL)
description: In de Nederlandse versie van Business Central kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a>Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling

In de Nederlandse versie van [!INCLUDE[prod_short](../../includes/prod_short.md)] kunt u elektronische SEPA-leveranciersbetalingen (Single Euro Payments Area) ISO 20022 maken en verzenden.  

Voordat u SEPA-leveranciersbetalingen kunt maken en verzenden, moet u SEPA-betalingen activeren. Zie [SEPA-betalingen activeren](how-to-activate-sepa-payments.md) voor meer informatie.  

## <a name="to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format"></a>Leverancierbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling

1.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Telebank - bankoverzicht** in en kies vervolgens de gerelateerde koppeling.  
2.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
3.  Selecteer de betreffende leveranciersbankrekening en kies vervolgens de actie **Posten ophalen**.  
4.  Vul op het sneltabblad **Opties** van de batchverwerking **Voorstelposten ophalen** de velden in, zoals wordt beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Valutadatum**|Hier geeft u de valutadatum op.|  
    |**Vervaldatum contantkort.**|Hier geeft u de vervaldatum voor de contantkorting op.|  

5.  Selecteer in het sneltabblad **Transactiemodus** de gewenste filters.  
6.  Selecteer in het sneltabblad **Klantenpost** de gewenste filters.  
7.  Selecteer op het sneltabblad **Leverancierspost** het filter **Leveranciersnr.** en selecteer een leveranciersnummer.  

    > [!NOTE]  
    >  Selecteer eventuele overige vereiste filters.  

8.  Kies de knop **OK**.  

De voorstelregels worden opgenomen op de pagina **Telebankierenvoorstel**.  

## <a name="see-also"></a>Zie ook
 [SEPA-betalingen activeren](how-to-activate-sepa-payments.md)   
 [Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md)   


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
