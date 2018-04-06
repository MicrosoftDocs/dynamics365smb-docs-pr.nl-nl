---
title: Elektronisch bankieren voor Nederland
description: Met de functionaliteit voor elektronisch bankieren kunt u bestanden voor elektronische betaling en bestanden voor automatische incasso maken, en elektronische bankafschriften importeren vanuit ondersteunde banksoftware.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/26/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: 9aea4a234f988c2199b0ab823051f86faa9439fb
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="dutch-electronic-banking"></a>Elektronisch bankieren voor Nederland
Met de functionaliteit voor elektronisch bankieren kunt u bestanden voor elektronische betaling en bestanden voor automatische incasso maken, en elektronische bankafschriften importeren vanuit ondersteunde banksoftware.  

## <a name="telebanking"></a>Telebankieren  
Met Telebankieren kunt u betalingen exporteren, bankafschriften importeren en gegevens verzamelen om naar de bank te sturen. Zie [Telebankieren](telebanking.md) voor meer informatie.  

U kunt betalingsvoorstellen maken en bankrekeningen reconciliëren in de kas-, bank- en giroboeken.  

### <a name="payment-files"></a>Betalingsbestanden  
U kunt betalingsvoorstellen maken voor het betalen van openstaande facturen aan leveranciers. Betalingsvoorstellen kunnen handmatig worden bewerkt voordat ze worden verwerkt, om betalingsfacturen toe te voegen of te verwijderen of om betalingsbedragen te wijzigen. Nadat een voorgestelde betalingsbatch is verwerkt, kunt u bestanden voor elektronische betaling naar de bank verzenden. Als er een fout wordt aangetroffen in het betalingsbestand tijdens het importeren in de banksoftware, kunt u een kopie maken van het betalingsbestand die u later opnieuw naar de bank kunt verzenden.  

U kunt binnenlandse betalingen en international betalingen verrichten in de aangewezen indelingen. Zie [Telebankieren](telebanking.md) voor meer informatie.  

### <a name="direct-debit-files"></a>Bestanden voor automatische incasso  
U kunt een betalingsvoorstel maken om betalingen te innen van bankrekeningen van klanten. Betalingsvoorstellen kunnen handmatig worden bewerkt om betalingsfacturen toe te voegen of te verwijderen of om inningsbedragen te wijzigen. Nadat een voorgestelde betalingsbatch is verwerkt, kunt u bestanden voor elektronische automatische incasso naar de bank verzenden. Als er een fout wordt aangetroffen in het bestand voor automatische incasso tijdens het importeren in de banksoftware, kunt u een kopie maken van het bestand voor automatische incasso die u later opnieuw naar de bank kunt verzenden.  

Momenteel kunt u alleen binnenlandse betalingen innen. Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.  

### <a name="bank-statement-import"></a>Importeren van bankafschriften  
U kunt bankafschriften importeren vanuit ondersteunde banksoftware en deze reconciliëren met binnenkomende en uitgaande betalingen. Ook kunt u bankkosten en ontvangen rente reconciliëren.  

Bestanden van elektronische bankafschriften worden voor de volgende banken ondersteund:  

- ABN AMRO Bank \(SWIFT MT940\)  
- ING Bank \(SWIFT MT940, PAYMUL\)  
- Rabobank \(MUT.ASC, VVMUT.ASC, BBV en ASCII\)  
- Postbank \(SWIFT MT940\)  

### <a name="bank-account-number-validation"></a>Validatie van bankrekeningnummer  
Bankrekeningnummers worden gevalideerd door te controleren of ze uit 9 of 10 cijfers bestaan en of ze het “elftest”-algoritme ondersteunen. Bij girorekeningen moet het rekeningnummer uit minder dan acht cijfers bestaan.  

## <a name="see-also"></a>Zie ook  
 [Telebankieren](telebanking.md)   
 [Kas\-Bank\-Giro](cash-bank-giro.md)   
 [Bankafschriften importeren en reconciliëren](how-to-import-and-reconcile-bank-statements.md)

