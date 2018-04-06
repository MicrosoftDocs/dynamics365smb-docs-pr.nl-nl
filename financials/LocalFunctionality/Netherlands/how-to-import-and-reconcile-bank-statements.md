---
title: "Bankafschriften importeren en reconciliëren"
description: "Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren."
services: project-madeira
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
ms.openlocfilehash: d5e785cb349d1eb73eeecabf961c94a5e2b0f9c8
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren
Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.  

Het importbankafschrift wordt ondersteund door de volgende protocollen:  

- Rabobank mut.asc  
- Rabobank vvmut.ac  
- Rabobank ASCII  
- SEPA CAMT  

## <a name="to-import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Bankafschrift importeren** in en klik vervolgens op de gerelateerde koppeling.  
2.  Selecteer in het venster **Importprotocoloverzicht** het vereiste importprotocol en kies vervolgens de knop **OK**.  
3.  Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.  

    > [!NOTE]  
    >  Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT. Gebruik in plaats daarvan de actie **Automatisch afstemmen** in het venster **Bankreconciliatie**. Zie voor meer informatie [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md).  

4.  Kies de knop **OK**.  
5.  Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.  

Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek. Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).  

## <a name="see-also"></a>Zie ook  
 [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md)   
 [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)

