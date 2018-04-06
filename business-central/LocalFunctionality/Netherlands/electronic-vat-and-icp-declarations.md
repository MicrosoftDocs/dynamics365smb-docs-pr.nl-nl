---
title: Elektronische btw- en ICP-aangiften
description: Bedrijven moeten periodieke btw- en ICP-aangiften verzenden.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 8341d8b1cb72ea9db0e9c3fc9001915a628b0470
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="electronic-vat-and-icp-declarations"></a>Elektronische btw- en ICP-aangiften
Bedrijven moeten periodieke btw- en ICP-aangiften verzenden.  

Btw aangiften moeten op een maandelijkse of driemaandelijkse basis worden verzonden.  

Bedrijven die goederen of diensten verkopen aan EU-landen, moeten ICP-aangiften (Intracommunautaire leveringen) op kwartaalbasis verzenden. Inkopen zijn niet opgenomen in deze aangifte. Voor deze intracommunautaire transacties moet echter de handelswaar de grens fysiek overschrijden. Het is niet voldoende dat de locatie van een factuuradres of het kantoor van de leverancier of klant in een ander land of een andere regio in een EU-land ligt.  

> [!NOTE]  
>  Voordat u elektronische aangiften naar de belastingdienst verstuurt, dient uw bedrijf aangemeld te zijn voor elektronische aangifte. De informatie die de belastingdienst nodig heeft is afhankelijk van de ondertekeningsmethode die uw bedrijf zal gebruiken, PIN of PKI. Voor beide methoden geldt dat u het formulier "Aanmeldingsformulier voor elektronisch berichtenverkeer met de belastingdienst" naar de belastingdienst moet opsturen.  
>   
>  Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  

## <a name="submitting-electronic-tax-declarations"></a>Elektronische belastingaangiften versturen  
U kunt de btw-aangiften en ICP-aangiften als volgt verzenden:  

- Meld u aan op de website van het Nederlandse belastingkantoor en voer de informatie handmatig in. Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  

    Voor ICP-aangiften kunt u maximaal 99 regels invoeren.  

- Een elektronische aangifte maken en het versleutelde bestand via SMTP (Simple Mail Transfer Protocol) naar het Nederlandse belastingkantoor versturen.  

De elektronische btw-aangifte bevat de geboekte btw en de berekende belasting over een opgegeven periode die aan de douane moet worden betaald. De gegevens van de btw-aangifte zijn gebaseerd op de definitie van de btw-aangifte in de tabel **Btw-aangifteregel**. Zie Btw-aangifteregel voor meer informatie.  

De gegevens van de ICP-aangifte zijn gebaseerd op de tabel **Btw-post**. Zie voor meer informatie Btw-post.  

## <a name="electronic-tax-declaration-methods"></a>Methoden voor elektronische aangiften  
U kunt de btw- en ICP-aangifte op elektronische wijze verzenden naar de belastingdienst met de volgende methoden:  

**PIN-methode (Personal Identification Number)**  
 Gebruikt een PIN-code om de aangifte te ondertekenen. Als u uw aangiften met de PIN-methode verzendt, moet u de PIN-code voor uw bedrijf maken en leveren aan de belastingdienst. Deze code helpt de belastingdienst het bedrijf te identificeren dat de elektronische aangifte heeft verstuurd. Deze PIN-code wordt niet opgeslagen in de database. Daarom moet u de PIN-code op een veilige plaats bewaren.  

> [!WARNING]  
>  De belastingdienst overweegt aangiften te accepteren die met behulp van een PIN-code zijn ondertekend. Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  

**PKI-methode (Public Key Infrastructure)**  
 Gebruikt digitale certificaten om berichten te versleutelen en digitale handtekening te verifiëren. Als u uw aangiften met de PKI-methode verzendt, moet u ook aanvullende certificaten, algemene parameters en andere parameters hebben wanneer u de PKI-methode gebruikt. Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  

## <a name="contact-information"></a>Contactgegevens  
De elektronische btw- en ICP-aangifte bevat contactgegevens over de belastingplichtige of intermediair. Zie voor meer informatie Btw-nummer.  

## <a name="see-also"></a>Zie ook  
 [Elektronische belastingaangiften](electronic-tax-declarations.md)   
 [Btw-categorieën instellen](how-to-set-up-vat-categories.md)   
 [Elektronische btw- en ICP-aangiften maken](how-to-create-electronic-vat-and-icp-declarations.md)   
 [Responsberichten van de belastingdienst verwerken](how-to-process-response-messages-from-tax-authorities.md)

