---
title: Bankafschriften importeren en reconciliëren
description: Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 41406e5dd5dca16ba43fcb01af649d3bb1746290
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5771388"
---
# <a name="import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren
Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.  

Het importbankafschrift wordt ondersteund door de volgende protocollen:  

- Rabobank mut.asc  
- Rabobank vvmut.ac  
- Rabobank ASCII  
- SEPA CAMT  

## <a name="to-import-and-reconcile-bank-statements"></a>Bankafschriften importeren en reconciliëren  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bank-/Giroboek** in en kies de gerelateerde koppeling.  
2.  Kies de actie **Bankafschrift importeren**, selecteer het vereiste importprotocol en kies vervolgens de knop **OK**.  
3.  Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.  

    > [!NOTE]  
    >  Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT. Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**. Zie [Bankrekeningen reconciliëren](../../bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.  

4.  Kies de knop **Ok**.  
5.  Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.  

Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek. Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).  

## <a name="see-also"></a>Zie ook  
[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md)   
[Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]