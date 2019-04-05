---
title: Telebankieren
description: Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
ms.openlocfilehash: 71529c52588fb6e6bcf0a3be80381c5c293c3f41
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "826883"
---
# <a name="telebanking"></a>Telebankieren
Op basis van zowel verkoop- als inkooptransacties kunt u met telebankieren betalingen en incasso's genereren die u elektronisch met uw bank kunt uitwisselen. Hieronder vallen ook de export van betalings- en incassogegevens die naar de bank moeten worden doorgestuurd en de import van bankafschriften die door de bank naar u worden verzonden.  

## <a name="transactions"></a>Transacties  
Over het algemeen worden alle financiële interacties met leveranciers en klanten uitgevoerd door middel van inkoop- of verkoopfacturen en creditnota's. Zodra deze transacties zijn geregistreerd en geboekt, kunnen betalingen of incasso's door uw bedrijf worden uitgevoerd.  

## <a name="proposals"></a>Voorstellen  
Op basis van leveranciers- en klantenposten kunt u met telebankieren betalings- en incassovoorstellen genereren. Dit kan voor elke bank worden gedaan die voor uw bedrijf is ingesteld. Zowel binnen- als buitenlandse betalingen en incasso's zijn mogelijk.  

U kunt [!INCLUDE[d365fin](../../includes/d365fin_md.md)] zodanig instellen dat betalingen aan of incasso's van dezelfde bankrekening automatisch worden gecombineerd.  

Als u akkoord gaat met het voorstel, moet het in een betaalrun worden verwerkt.  

> [!NOTE]  
>  Over het algemeen kan voor alle openstaande leveranciers- en klantenposten een voorstel worden gegenereerd als dat aan een aantal criteria voldoet. Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.  

## <a name="payment-histories"></a>Betaalruns  
Een betaalrun is eigenlijk precies hetzelfde als een voorstel, het enige verschil is dat gegevens in een betaalrun niet kunnen worden gewijzigd. De betalings- of incassogegevens zijn gereed om naar de bank te worden geëxporteerd en verzonden.  

 Zie voor meer informatie [Betaalrun maken en exporteren](how-to-create-and-export-payment-history.md).  

## <a name="bank-statements"></a>Bankafschriften  
 Voor alle financiële interacties die via uw bank plaatsvinden, kan de bank u elektronische bankafschriften toesturen. Deze afschriften kunnen in de Bank-/Giroboeken worden geïmporteerd. Als u wilt kunt u [!INCLUDE[d365fin](../../includes/d365fin_md.md)] deze afschriften tijdens het importproces automatisch laten reconciliëren en kan worden vastgesteld of een afschrift kan worden vereffend met openstaande posten voor de betreffende leverancier/klant.  

 Zie [Bankafschriften importeren en reconciliëren](how-to-import-and-reconcile-bank-statements.md) voor meer informatie.  

## <a name="exchange-protocols"></a>Uitwisselingsprotocollen  
 Voor zowel het exporteren als importeren is een aantal protocollen gedefinieerd. [!INCLUDE[d365fin](../../includes/d365fin_md.md)] ondersteunt de volgende protocollen:  

- BTL91 (exporteren)  
- BBV (exporteren)  
- PAYMUL (exporteren)  
- Rabobank mut.asc (importeren)  
- Rabobank vvmut.asc (importeren)  
- Rabobank ASCII (importeren)  
- SEPA CAMT  

## <a name="see-also"></a>Zie ook  
 [Verkopen factureren](../../sales-how-invoice-sales.md)   
 [Inkopen vastleggen](../../purchasing-how-record-purchases.md)   
 [Voorstellen maken.](how-to-create-proposals.md)   
 [Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)
