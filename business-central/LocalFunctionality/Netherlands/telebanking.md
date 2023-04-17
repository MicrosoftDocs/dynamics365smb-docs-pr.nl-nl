---
title: Telebankieren
description: Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 04/01/2021
ms.author: edupont
---
# Telebankieren
Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen. Hieronder vallen ook de export van betalings- en incassogegevens die naar de bank moeten worden doorgestuurd en de import van bankafschriften die door de bank naar u worden verzonden.  

## Transacties  
Over het algemeen worden alle financiële interacties met leveranciers en klanten uitgevoerd door middel van inkoop- of verkoopfacturen en creditnota's. Zodra deze transacties zijn geregistreerd en geboekt, kunnen betalingen of incasso's door uw bedrijf worden uitgevoerd.  

## Voorstellen  
Op basis van leveranciers- en klantenposten kunt u met telebankieren betalings- en incassovoorstellen genereren. Dit kan voor elke bank worden gedaan die voor uw bedrijf is ingesteld. Zowel binnen- als buitenlandse betalingen en incasso's zijn mogelijk.  

U kunt [!INCLUDE[prod_short](../../includes/prod_short.md)] zodanig instellen dat betalingen aan of incasso's van dezelfde bankrekening automatisch worden gecombineerd.  

Als u akkoord gaat met het voorstel, moet het in een betaalrun worden verwerkt.  

> [!NOTE]  
>  Over het algemeen kan voor alle openstaande leveranciers- en klantenposten een voorstel worden gegenereerd als dat aan een aantal criteria voldoet. Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.  

## Betaalruns  
Een betaalrun is eigenlijk precies hetzelfde als een voorstel, het enige verschil is dat gegevens in een betaalrun niet kunnen worden gewijzigd. De betalings- of incassogegevens zijn gereed om naar de bank te worden geëxporteerd en verzonden.  

 Zie voor meer informatie [Betaalrun maken en exporteren](how-to-create-and-export-payment-history.md).  

## Bankafschriften  
 Voor alle financiële interacties die via uw bank plaatsvinden, kan de bank u elektronische bankafschriften toesturen. Deze afschriften kunnen in de Bank-/Giroboeken worden geïmporteerd. Als u wilt kunt u [!INCLUDE[prod_short](../../includes/prod_short.md)] deze afschriften tijdens het importproces automatisch laten reconciliëren en kan worden vastgesteld of een afschrift kan worden vereffend met openstaande posten voor de betreffende leverancier/klant.  

 Zie [Bankafschriften importeren en reconciliëren](how-to-import-and-reconcile-bank-statements.md) voor meer informatie.  
 
 > [!NOTE]  
>  De valuta van de geïmporteerde transacties moet overeenkomen met de valuta die is opgegeven op de bankrekening in [!INCLUDE[prod_short](../../includes/prod_short.md)].  

## Uitwisselingsprotocollen  
 Voor zowel het exporteren als importeren is een aantal protocollen gedefinieerd. [!INCLUDE[prod_short](../../includes/prod_short.md)] ondersteunt de volgende protocollen:  

- BTL91 (export). Dit grensoverschrijdende protocol wordt niet langer geaccepteerd in Nederland vanaf 1 mei 2019. Dit protocol wordt vervangen door het Algemeen betalingsbestand-protocol.
- BBV (exporteren)  
- PAYMUL (exporteren)  
- Algemeen betalingsbestand (export). Kan worden gebruikt voor grensoverschrijdende overdrachten buiten de EU.
- Rabobank mut.asc (importeren)  
- Rabobank vvmut.asc (importeren)  
- Rabobank ASCII (importeren)  
- SEPA CAMT  

## Zie ook  
 [Verkopen factureren](../../sales-how-invoice-sales.md)   
 [Inkopen vastleggen](../../purchasing-how-record-purchases.md)   
 [Voorstellen maken.](how-to-create-proposals.md)   
 [Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]