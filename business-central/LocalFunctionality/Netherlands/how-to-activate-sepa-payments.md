---
title: Activeer SEPA-betalingen in de Nederlandse versie
description: 'Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 07/03/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Activeer SEPA-betalingen in de Nederlandse versie

[!INCLUDE [activate-sepa-payments](../includes/BENL/activate-sepa-payments.md)]

## Transactiewijzen activeren voor SEPA  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transactiewijzen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer de transactiewijze die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.  
3. Selecteer in het veld **Exportprotocol** op het sneltabblad **Betalingsvoorstel** van de pagina **Transactiewijzekaart** het SEPA-exportprotocol dat u hebt gemaakt, bijvoorbeeld **SEPA ISO20022**.  
4. Kies de knop **Ok**.  

> [!NOTE]
> Als u  *SEPA DD 008.001.08* en *SEPA CT Pain 001.001.09* wilt gebruiken, moet u nieuwe rapporten instellen *11000015* voor Pain 008.001.08" en *11000014* voor Pain 001.001.09" die kunnen worden geselecteerd in het veld  **Exportprotocol** om bestanden te exporteren in de overeenkomstige formaten.  

## Transactiewijzen voor leveranciersbetalingen voor SEPA verifiëren  

1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Leveranciers** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer de leverancier waarvoor u de transactiewijze wilt verifiëren en kies de actie **Weergave**.  
3. Controleer of de transactiewijze voor de leveranciersbetalingen in het veld **Code transactiewijze** van het sneltabblad **Betalingen** een transactiewijze is die is geactiveerd voor SEPA.  
4. Kies de knop **Ok**.  

## Zie ook  

[Single EURO Payments Area (SEPA)](single-euro-payments-area-sepa-.md)  
[Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling](how-to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
