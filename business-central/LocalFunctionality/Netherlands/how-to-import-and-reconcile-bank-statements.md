---
title: "Bankafschriften importeren en reconciliëren"
description: "Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren."
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 12/06/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 8a73de1aa2f4a0f633c401ea341bb7bde6579723
ms.openlocfilehash: 04235583bc44f780b1f36f9641fc5c0e91c77d30
ms.contentlocale: nl-nl
ms.lasthandoff: 12/11/2018

---
# <a name="import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren
Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.  

Het importbankafschrift wordt ondersteund door de volgende protocollen:  

- Rabobank mut.asc  
- Rabobank vvmut.ac  
- Rabobank ASCII  
- SEPA CAMT  

## <a name="to-import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bank-/giroboek** in en klik vervolgens op de gerelateerde koppeling.  
2.  Kies de actie **Bankafschrift importeren**, selecteer het vereiste importprotocol en kies vervolgens de knop **OK**.  
3.  Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.  

    > [!NOTE]  
    >  Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT. Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**. Zie [Bankrekeningen apart reconciliëren](../../bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.  

4.  Kies de knop **OK**.  
5.  Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.  

Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek. Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).  

## <a name="see-also"></a>Zie ook  
[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md)   
[Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)

