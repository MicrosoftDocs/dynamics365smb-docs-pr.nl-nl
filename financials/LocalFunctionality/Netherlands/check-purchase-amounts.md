---
title: Inkoopbedragen controleren
description: Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het 'bedrag incl. btw' en het 'btw-bedrag' die vermeld staan op het inkooporderdocument gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels.
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
ms.openlocfilehash: 18f14075e673013370981c2af906f9bd781b4628
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="check-purchase-amounts"></a>Inkoopbedragen controleren
Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkooporderdocument, gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels. Hiervoor moeten de velden **Documentbedrag incl. btw** en **Btw documentbedrag** ingevuld zijn in het venster **Inkoopfactuur** of **Inkoopcreditnota**.  

 Als er slechts één inkoopregel is of als alle regels vallen onder hetzelfde btw-percentage, wordt het juiste **Btw documentbedrag**-veld automatisch berekend wanneer u de inkoopregels en het veld **Documentbedrag incl. btw** hebt ingevoegd. In het geval dat verschillende regels met verschillende btw-percentages bestaan, moet het veld **Documentbedrag incl. btw** handmatig worden gewijzigd.  

 De totaalbedragen van het inkoopdocument worden standaard gecontroleerd, maar u kunt dit uitschakelen door het selectievakje **Totaalbedragen documenten controleren** in het venster **Inkoopinstellingen** uit te schakelen.  

 Als u wilt weten waarom er een verschil is tussen de totaalbedragen van het document en de totaalbedragen van de ingevoegde inkoopregels, hebt u de mogelijkheid om het totaalbedrag, het totale basisbedrag, het totale btw-bedrag en het totaalbedrag inclusief btw van de ingevoegde inkoopregels te laten berekenen en deze onder aan het inkoopfactuur- of inkoopcreditnotavenster weer te geven.  

 Deze totaalbedragen worden standaard niet weergegeven, maar u kunt dit inschakelen door het selectievakje **Totale op inkoopfactuur/CR-nota weergeven** in te schakelen in het venster **Inkoopinstellingen**.  

> [!NOTE]  
>  Als u dit veld activeert, moeten de totalen van alle inkoopfacturen en creditnota's worden herberekend. Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend. U kunt dit veld niet activeren als er inkoopfacturen en/of creditnota's zijn zonder inkoopregels of als u inkoopfacturen en/of inkoopcreditnota's hebt waarbij geen aantal is opgegeven op de regels.  

## <a name="see-also"></a>Zie ook  
 [Validatie van inkoopbedragen instellen](how-to-set-up-validation-of-purchase-amounts.md)

