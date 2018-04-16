---
title: Betalingen verrichten met de conversieservice van bankgegevens of SEPA-overmaking | Microsoft Docs
description: Verwerk betalingen aan uw leveranciers door samen met de betalingsgegevens van de dagboekregels een bestand te exporteren.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 11/17/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 99277cb2daf37fbce4548cf637e8967fa6688dbc
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="making-payments-with-bank-data-conversion-service-or-sepa-credit-transfer"></a>Betalingen verrichten met de conversieservice van bankgegevens of SEPA-overmaking
U kunt in het venster **Betalingsdagboek** betalingen naar uw leveranciers verwerken door samen met de betalingsgegevens van de dagboekregels een bestand te exporteren. Vervolgens kunt u het bestand uploaden naar uw elektronische banksite waar de gerelateerde overboekingen worden verwerkt. [!INCLUDE[d365fin](includes/d365fin_md.md)] ondersteunt de indeling voor SEPA-kredietoverboekingen, maar in uw land of regio kunnen andere indelingen voor elektronische betalingen beschikbaar zijn.   

 Voor het mogelijk maken van SEPA-kredietoverboekingen moet u eerst een bankrekening, leverancier, en dagboekbatch instellen waarop het betalingsdagboek is gebaseerd. Bereid vervolgens betalingen aan leveranciers voor door het venster **Betalingsdagboek** automatisch te vullen met verschuldigde betalingen met een opgegeven boekingsdatum.  

> [!NOTE]  
>  Wanneer u hebt gecontroleerd dat de betalingen zijn verwerkt door de bank, kunt u doorgaan met het boeken van de betalingsdagboekregels.  

 In de volgende tabel wordt een reeks taken beschreven, met koppelingen naar de beschrijvende onderwerpen.   

|**Als u dit wilt doen**|**Zie**|  
|------------|-------------|  
|Activeer de conversieservice voor bankgegevens om een bankafschriftbestand te laten converteren naar een indeling die u kunt importeren of om uw geëxporteerde betalingsbestanden te laten converteren naar de indeling die uw bank vereist.|[Conversieservice voor bankgegevens instellen](bank-how-setup-bank-statement-service.md)|  
|Stel een bankrekening, leverancier en betalingsdagboek in voor SEPA-kredietoverboeking.|[SEPA-krediettransfer instellen](finance-how-to-set-up-sepa-credit-transfer.md)|  
|Vul het betalingsdagboek met regels voor verschuldigde betalingen aan leveranciers, met de mogelijkheid boekingsdatums in te voegen op basis van de vervaldatum van de verwante inkoopdocumenten.|[Betalingsverplichtingen beheren](payables-manage-payables.md)|  
|Exporteer betalingsdagboekregels naar een bestand in de SEPA-overmakingsindeling.|[Betalingen naar een bankbestand exporteren](payables-how-export-payments-bank-file.md)|  
|Wanneer de elektronische betaling is verwerkt door de bank, boekt u de betalingen.|[Werken met diversendagboeken](ui-work-general-journals.md)|  

## <a name="see-also"></a>Zie ook  
[Conversieservice voor bankgegevens instellen](bank-how-setup-bank-statement-service.md)  
[SEPA-krediettransfer instellen](finance-how-to-set-up-sepa-credit-transfer.md)  
[Betalingsverplichtingen beheren](payables-manage-payables.md)   
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Betalingen verzamelen via automatische incasso van SEPA](finance-collect-payments-with-sepa-direct-debit.md)   
