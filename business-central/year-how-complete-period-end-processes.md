---
title: Optionele activiteiten voor sluitingsperiodes
description: In dit artikel worden de optionele processen en activiteiten voor het afsluiten van boekhoudperioden in Business Central beschreven.
author: jswymer
ms.topic: overview
ms.devlang: al
ms.search.keywords: 'year closing, close accounting period, close fiscal year, aging, creditor payments, vendor payments'
ms.date: 08/02/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="overview-of-tasks-to-close-accounting-periods"></a>Overzicht van taken voor Sluiten boekhoudperioden

[!INCLUDE[prod_short](includes/prod_short.md)] dwingt u niet tot Sluiten-periodes, maar er zijn veel activiteiten aan het einde van de periode (maandeinde) die u kunt doen. Dit artikel biedt een overzicht van optionele processen en activiteiten voor afsluitingsperioden.  

## <a name="general-ledger"></a>Grootboek

* Geef de boekingsperioden voor het gehele systeem of een specifieke gebruiker op.  

    Hiermee worden de datums opgegeven waartussen u boekingen wilt toestaan. Afhankelijk van uw bedrijf wilt u mogelijk toestaan dat er aan het begin of tegen het einde van de periode wordt gepost. Meer informatie op [Boekingsperioden opgeven](finance-how-specify-posting-periods.md).  
* Breng alle benodigde wijzigingen in het grootboek aan.  
* Wijzig en boek periodieke dagboeken.  
  <!--* Process Consolidations-->
* Voer financiële rapporten als volgt uit:  
  * Open de pagina **Financiële rapporten** en kies de actie **Afdrukken**.  

## <a name="sales-and-receivables"></a>Verkopen en tegoeden

* Boek alle verkooporders, facturen, creditnota's en retourorders.  
* Boek alle ontvangstendagboeken.  
* Wijzig en boek periodieke dagboeken die met verkoop en tegoeden te maken hebben.  
* Reconcilieer klanten met het grootboek.  
* Voer de batchverwerking **Gefactureerde verkooporders verwijderen** uit.  

## <a name="purchases-and-payables"></a>Inkopen en schulden

* Boek alle inkooporders, facturen, creditnota's en retourorders.  
* Boek alle betalingsdagboeken.  
* Wijzig en boek periodieke dagboeken die bij met inkopen en leveranciers te maken hebben.  
* Voer het rapport **Vervallen betalingen** uit en reconcilieer leveranciers met het grootboek.  
* Voer de batchverwerking **Gefactureerde inkooporders verwijderen** uit.  

## <a name="fixed-assets"></a>Vaste activa

* Boek alle onderhoudskosten die zijn geboekt via de VA-dagboeken of -facturen.
* Boek herwaarderingen.
* Boek waardevermeerdering.
* Boek afschrijving.
* Wijzig en boek het periodiek VA-dagboek.

## <a name="intercompany"></a>Intercomp

* IC-transacties verwerken.

## <a name="calculate-and-process-sales-tax"></a>Btw berekenen en verwerken

* Belastingaangiften invullen.  

## <a name="see-also"></a>Zie ook

[Jaren en perioden afsluiten](year-close-years-periods.md)  
[Boeken afsluiten](year-close-books.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
