---
title: Kasboeken, bankboeken of giroboeken invoeren en boeken
description: In Business Central kunt u het kas- en het bankboek gebruiken om de transacties in te voeren die van invloed zijn op de kas- en bankrekening door **Kasboek** en **Bankboek** te gebruiken.
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
ms.openlocfilehash: 47411ec745ee3c0dae6614bda529e8081c4df002
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="enter-and-post-cash-and-bank-or-giro-journals"></a>Kasboeken, bankboeken of giroboeken invoeren en boeken
In [!INCLUDE[d365fin](../../includes/d365fin_md.md)] kunt u het kas- en het bankboek gebruiken om de transacties in te voeren die van invloed zijn op de kas- en bankrekening door **Kasboek** en **Bankboek** te gebruiken.  

U kunt een toenames of afnames op de kasrekening invoeren in de **Kasboeken**. U kunt dit dagboek bijvoorbeeld gebruiken voor het betalen van kleine kas of het ontvangen van transfers van een andere bankrekening.  

Het **Bank-/giroboek** registreert de instroom of uitstroom van de contanten naar een bepaalde rekening. Dit dagboek vormt de basis voor bankreconciliatie. De indeling van dit dagboek lijkt op het papieren bankafschrift, dus u kunt u de vereiste velden van het papieren afschrift overnemen in het dagboek of u kunt een elektronisch bankafschriftbestand importeren. De transacties kunnen klantbetalingen of leveranciersbetalingen zijn.  

U kunt de betalingen van klanten vereffenen met de openstaande facturen van Vorderingen. U kunt ook grootboektransacties invoeren om overige bedragen vast te leggen, zoals bankkosten of rente-inkomsten. Btw codes kunnen ook op deze transactieregels worden toegepast. U kunt een dagboek per bankrekening opgeven.  

## <a name="to-post-cash-journals"></a>Kasjournalen boeken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Kasboek** in en klik op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Vul in het venster **Kasboek** op het sneltabblad **Regel** de vereiste velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Datum**|De dagboekboekingsdatum.|  
    |**Documentnr.**|Het documentnummer waarvoor de dagboekpost wordt gemaakt.|  
    |**Rekeningsoort**|Het rekeningtype waarnaar de post moet worden geboekt.|  
    |**Rekeningnr.**|Het rekeningnummer waarnaar de post moet worden geboekt.|  
    |**Beschrijving**|De omschrijving van de post. Dit veld vult automatisch de omschrijving van het geselecteerde rekeningnummer in het veld **Rekeningnr.** in.|  
    |**Btw-productboekingsgroep**|De btw-productboekingsgroepscode die wordt gebruikt om de post te boeken. U kunt in dit veld alleen een code selecteren als het **Rekeningsoort** **Grootboekrek.** is. Zie Btw-productboekingsgroepen voor meer informatie.|  
    |**Bedrag**|Het totale bedrag waaruit de afschriftregel bestaat. U moet het debetbedrag zonder plus- of minteken invoeren en het creditbedrag met een minteken invoeren.<br /><br /> Als dit bedrag het btw-bedrag omvat, selecteert u het selectievakje **Bedrag incl. btw**.|  

4.  Kies de actie **Boeken**.  

    > [!NOTE]  
    >  Als er een verschil is tussen het beginsaldo en het eindsaldo, moet u het eindsaldo vóór het boeken van de post wijzigen.  

     De posten worden naar het grootboek geboekt. Zie Gootboekposten voor meer informatie.  

## <a name="to-post-bank-or-giro-journals"></a>Bank- of giroboeken boeken  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bank-/giroboek** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Selecteer de relevante dagboeksjabloon en kies vervolgens de knop **OK**.  
4.  Vul in het venster **Bank-/girodagboek** de velden in, zoals is beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Beginsaldo**|Het huidige saldo van de bankrekening of girorekening. Dit is gelijk aan het eindsaldo van de eerder geboekte posten voor het dagboek.|  
    |**Eindsaldo**|Het nieuwe eindsaldo van het dagboek.|  

5.  Vul op het sneltabblad **Regels** de vereiste velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Datum**|De dagboekboekingsdatum.|  
    |**Rekeningsoort**|Het rekeningtype waarnaar de dagboekpost moet worden geboekt.|  
    |**Rekeningnr.**|Het rekeningnummer waarnaar de dagboekpost moet worden geboekt.|  
    |**Kenmerk**|Het identificatienummer dat de afschriftregel aan een betaalrunregel koppelt.|  
    |**Beschrijving**|De omschrijving van de post.|  
    |**Btw-productboekingsgroep**|De btw-productboekingsgroep die wordt gebruikt wanneer u de post op de afschriftregel boekt.|  
    |**Bedrag**|Het totale bedrag waaruit de afschriftregel bestaat. U moet het debetbedrag zonder plus- of minteken invoeren en het creditbedrag met een minteken invoeren.<br /><br /> Als dit bedrag het btw-bedrag omvat, selecteert u het selectievakje **Bedrag incl. btw**.|  

6.  Kies de actie **Boeken**.  

> [!NOTE]  
>  Als er een verschil is tussen het beginsaldo en het eindsaldo, moet u het eindsaldo vóór het boeken van de post wijzigen.  

De posten worden naar het grootboek geboekt. Zie Gootboekposten voor meer informatie.  

## <a name="see-also"></a>Zie ook  
 [De testrapporten afdrukken voor kasboeken, bankboeken of giroboeken](how-to-print-the-test-reports-for-cash-and-bank-or-giro-journals.md)

