---
title: Bankafschriften importeren en reconciliëren
description: Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 12/13/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Bankafschriften importeren en reconciliëren
Banken bieden elektronische bankafschriften voor al uw financiële interacties. U kunt deze afschriften in het bank- of giroboek importeren.  

Het importbankafschrift wordt ondersteund door de volgende protocollen:  

- Rabobank mut.asc  
- Rabobank vvmut.ac  
- Rabobank ASCII  
- SEPA CAMT  

## Bankafschriften importeren en reconciliëren  

1.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bank-/giroboek** in en kies vervolgens de gerelateerde koppeling.  
2.  Kies de actie **Bankafschrift importeren**, selecteer het vereiste importprotocol en kies vervolgens de knop **OK**.  
3.  Als u bankafschriften automatisch wilt laten reconciliëren tijdens het importeren, schakelt u op het sneltabblad **Opties** het selectievakje **Automatisch reconciliëren** in.  

    > [!NOTE]  
    >  Deze functie werkt niet voor bankafschriftbestanden van de soort SEPA CAMT. Gebruik in plaats daarvan de actie **Automatisch afstemmen** op de pagina **Bankreconciliatie**. Zie [Bankrekeningen reconciliëren](../../bank-how-reconcile-bank-accounts-separately.md) voor meer informatie.  

4.  Kies de knop **Ok**.  
5.  Als u het bestand wilt importeren dat het elektronische bankafschrift bevat, geeft u de bestandsnaam en het pad op en kiest u de knop **Openen**.  

Het elektronische bankafschrift wordt geïmporteerd in het bank- of giroboek. Zie voor meer informatie [Elektronisch bankieren voor Nederland](dutch-electronic-banking.md).  

## Zie ook  
[Elektronisch bankieren voor Nederland](dutch-electronic-banking.md)   
[Betalingen automatisch vereffenen en bankrekeningen reconciliëren](../../receivables-apply-payments-auto-reconcile-bank-accounts.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]