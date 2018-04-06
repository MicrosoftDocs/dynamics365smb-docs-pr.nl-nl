---
title: SEPA-betalingen activeren
description: Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen.
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: cceecd5c485208205b5886c48ff6df3a531f0e3b
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="activate-sepa-payments"></a>SEPA-betalingen activeren
Als u leveranciersbetalingen elektronisch wilt verzenden in de betalingsindeling SEPA (Single Euro Payments Area) ISO 20022, moet u eerst de vereiste instellingen aanbrengen voor het activeren van SEPA-betalingen.  

In de volgende procedures beschrijven de eerste vier hoe u SEPA-betalingen activeert. De twee overige procedures hebben betrekking op de afzonderlijke leveranciers.  

## <a name="to-enable-countriesregions-for-sepa"></a>Landen/regio's activeren voor SEPA  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Landen/regio's** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Lijst bewerken**.  
3.  Schakel het selectievakje **SEPA toegestaan** in voor elk land of elke regio dat/die u wilt activeren voor SEPA.  
4.  Kies de knop **OK**.  

## <a name="to-enable-bank-accounts-for-sepa"></a>Bankrekeningen activeren voor SEPA  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bankrekeningen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de bankrekening die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.  
3.  Selecteer in het veld **Land-/regiocode** van het sneltabblad **Algemeen** de gewenste code.  

    > [!NOTE]  
    >  De opgegeven land-/regiocode moet zijn geactiveerd voor SEPA, zoals is beschreven in de vorige procedure.  

4.  Geef een waarde op in het veld **Minimumsaldo**.  
5.  Geef in het veld **SWIFT-code** van het sneltabblad **Transfer** een code op.  
6.  Kies de knop **OK**.  

## <a name="to-set-up-a-sepa-iso-20022-export-protocol"></a>Een SEPA ISO 20022-exportprotocol instellen  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Exportprotocollen** in en kies vervolgens de gerelateerde koppeling.  
2.  Kies in het venster **Exportprotocollen** de actie **Nieuw**.  
3.  Vul de velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Code**|Hier stelt u de exportprotocolcode in, zoals **SEPA ISO20022**.|  
    |**Beschrijving**|Hier wordt een omschrijving weergegeven voor het exportprotocol.|  
    |**Controle-id**|Hier wordt de id ingesteld voor de code-unit om de betaling te controleren, bijvoorbeeld **11000010**.|  
    |**Controlenaam**|Hier wordt de naam van de code-unit ingesteld.|  
    |**Soort exportprotocol**|Hiermee wordt het soort exportprotocol opgegeven:<br /><br /> -   **Rapport**<br />-   **XMLPort**|  
    |**Export-id**|Hier wordt de id ingesteld voor de batchverwerking om betalingen te exporteren, bijvoorbeeld **11000011**.<br /><br /> Als u XMLPort als uw exportprotocolsoort selecteert, kiest u een id zoals **1000**|  
    |**Exportnaam**|De naam van de batchverwerking.|  
    |**Borderel-id**|Hier wordt de id ingesteld voor de batchverwerking om de contactpersoon op de hoogte te brengen van gecombineerde betalingen, zoals **11000004**.<br /><br /> Dit is niet van toepassing op XMLPort-protocolsoorten.|  
    |**Borderelnaam**|De naam van het borderelrapport.|  
    |**Standaardbestandsnamen**|Hier wordt de locatie ingesteld voor het exporteren van betalings- en inningsgegevens.|  

4.  Kies de knop **OK**.  

## <a name="to-enable-transaction-modes-for-sepa"></a>Transactiewijzen activeren voor SEPA  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Transactiewijzen** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de transactiewijze die u wilt activeren voor SEPA en kies vervolgens de actie **Bewerken**.  
3.  Selecteer in het venster **Transactiewijzekaart** op het sneltabblad **Betalingsvoorstel** in het veld **Exportprotocol** het SEPA-exportprotocol dat u hebt gemaakt, bijvoorbeeld **SEPA ISO20022**.  
4.  Kies de knop **OK**.  

## <a name="to-verify-vendor-payment-transaction-modes-for-sepa"></a>Transactiewijzen voor leveranciersbetalingen voor SEPA verifiëren  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de leverancier waarvoor u de transactiewijze wilt verifiëren en kies de actie **Weergave**.  
3.  Controleer of de transactiewijze voor de leveranciersbetalingen in het veld **Code transactiewijze** van het sneltabblad **Betalingen** een transactiewijze is die is geactiveerd voor SEPA.  
4.  Kies de knop **OK**.  

## <a name="to-set-up-vendor-bank-accounts-for-sepa"></a>Bankrekeningen van leveranciers instellen voor SEPA  

1.  Klik op het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Leveranciers** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer de betreffende leverancier en kies vervolgens de actie **Bankrekeningen**.  
3.  Selecteer de bankrekening van de leverancier die u wilt instellen voor SEPA, en kies vervolgens de actie **Bewerken**.  
4.  Geef in de velden **IBAN** en **SWIFT-code** van het sneltabblad **Transfer** de internationale bankidentificatiecode op van de bank waarbij de leverancier de rekening heeft.  
5.  Kies de knop **OK**.  

## <a name="see-also"></a>Zie ook  
 [Gemeenschappelijke betalingsruimte voor de euro (SEPA)](single-euro-payments-area-sepa-.md)   
 [Leveranciersbetalingen elektronisch versturen in SEPA ISO 20022-betalingsindeling](how-to-submit-vendor-payments-electronically-in-sepa-iso-20022-payment-format.md) 

