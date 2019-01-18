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
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: 28276c3649ef0b9c8cd875a7ad50c1f11271eede
ms.contentlocale: nl-nl
ms.lasthandoff: 11/26/2018

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
2.  Selecteer op de pagina **Importprotocoloverzicht** het vereiste importprotocol en kies vervolgens de knop **OK**.  
3.  Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.  

    > [!NOTE]  
    >  Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT. Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**. Zie voor meer informatie [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md).  

4.  Kies de knop **OK**.  
5.  Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.  

Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek. Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).  

## <a name="see-also"></a>Zie ook  
 [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md)   
 [Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)

