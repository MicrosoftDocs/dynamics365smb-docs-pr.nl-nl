---
title: Kasboeken, bankboeken of giroboeken invoeren en boeken
description: In Business Central kunt u het kas- en het bankboek gebruiken om de transacties in te voeren die van invloed zijn op de kas- en bankrekening door Kasboek en Bankboek te gebruiken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 0bfa417e2d0d0250346a1942c2a6584a40c2638a
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382121"
---
# <a name="enter-and-post-cash-and-bankgiro-journals"></a>Kasboeken, bankboeken of giroboeken invoeren en boeken
Het kasboek en het bank/giro-boek helpen u transacties in het systeem te boeken op een gemakkelijkere en directere manier dan met het diversendagboek.  

Daarnaast kunt u in combinatie met telebankieren elektronische bankafschriften op de pagina **Bank-/Giroboek** importeren. Desgewenst kunnen deze afschriften tijdens het importproces automatisch worden gereconcilieerd en kan worden vastgesteld of een afschrift kan worden vereffend met openstaande posten voor de betreffende leverancier/klant.

In [!INCLUDE[prod_short](../../includes/prod_short.md)] kunt u het kas- en het bankboek gebruiken om de transacties in te voeren die van invloed zijn op de kas- en bankrekening door de typen **Kasboek** en **Bankboek** te gebruiken.  

U kunt een toenames of afnames op de kasrekening invoeren op de pagina **Kasboeken**. U kunt dit dagboek bijvoorbeeld gebruiken voor het betalen van kleine kas of het ontvangen van transfers van een andere bankrekening.  

De pagina **Bank-/giroboek** registreert de instroom of uitstroom van de contanten naar een bepaalde rekening. Dit dagboek vormt de basis voor bankreconciliatie. De indeling van dit dagboek lijkt op het papieren bankafschrift, dus u kunt u de vereiste velden van het papieren afschrift overnemen in het dagboek of u kunt een elektronisch bankafschriftbestand importeren. De transacties kunnen klantbetalingen of leveranciersbetalingen zijn.  

U kunt de betalingen van klanten vereffenen met de openstaande facturen van Vorderingen. U kunt ook grootboektransacties invoeren om overige bedragen vast te leggen, zoals bankkosten of rente-inkomsten. Btw codes kunnen ook op deze transactieregels worden toegepast. U kunt een dagboek per bankrekening opgeven.  

## <a name="to-post-cash-journals"></a>Kasjournalen boeken  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Kasboek** in en kies de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Vul op de pagina **Kasboek** op het sneltabblad **Regel** de vereiste velden in zoals beschreven in de volgende tabel.  

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

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bank-/Giroboek** in en kies de gerelateerde koppeling.  
2.  Kies de actie **Nieuw**.  
3.  Selecteer de relevante dagboeksjabloon en kies vervolgens de knop **OK**.  
4.  Vul op de pagina **Bank-/girodagboek** de velden in, zoals is beschreven in de volgende tabel.  

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
 [Telebankieren](telebanking.md)   
 [Kasboeken, bankboeken of giroboeken invoeren en boeken](how-to-enter-and-post-cash-and-bank-or-giro-journals.md)  
 [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]