---
title: 'Inkoopbedragen controleren [NL]'
description: 'De toepassing controleert of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkoopdocument, gelijk zijn aan het totaalbedrag van ingevoegde inkoopregels.'
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: null
ms.date: 06/18/2021
ms.author: edupont
---
# <a name="check-purchase-amounts-in-the-dutch-version" />Inkoopbedragen controleren in de Nederlandse versie
Voordat u een inkoopfactuur of creditnota boekt, wordt gecontroleerd of het bedrag incl. btw en het btw-bedrag die vermeld staan op het inkooporderdocument, gelijk zijn aan het totaalbedrag van de ingevoegde inkoopregels. Hiervoor moeten de velden **Documentbedrag incl. btw** en **Btw documentbedrag** ingevuld zijn op de pagina **Inkoopfactuur** of **Inkoopcreditnota**.  

 Als er slechts één inkoopregel is of als alle regels vallen onder hetzelfde btw-percentage, wordt het juiste **Btw documentbedrag**-veld automatisch berekend wanneer u de inkoopregels en het veld **Documentbedrag incl. btw** hebt ingevoegd. In het geval dat verschillende regels met verschillende btw-percentages bestaan, moet het veld **Documentbedrag incl. btw** handmatig worden gewijzigd.  

 De totaalbedragen van het inkoopdocument worden standaard gecontroleerd, maar u kunt dit uitschakelen door het selectievakje **Totaalbedragen documenten controleren** op de pagina **Inkoopinstellingen** uit te schakelen.  

 Als u wilt weten waarom er een verschil is tussen de totaalbedragen van het document en de totaalbedragen van de ingevoegde inkoopregels, hebt u de mogelijkheid om het totaalbedrag, het totale basisbedrag, het totale btw-bedrag en het totaalbedrag inclusief btw van de ingevoegde inkoopregels te laten berekenen en deze onder aan de inkoopfactuur- of inkoopcreditnotapagina weer te geven.  

 Deze totaalbedragen worden standaard niet weergegeven, maar u kunt dit inschakelen door het selectievakje **Totale op inkoopfactuur/CR-nota weergeven** in te schakelen op de pagina **Inkoopinstellingen**.  

> [!NOTE]  
>  Als u dit veld activeert, moeten de totalen van alle inkoopfacturen en creditnota's worden herberekend. Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend. U kunt dit veld niet activeren als er inkoopfacturen en/of creditnota's zijn zonder inkoopregels of als u inkoopfacturen en/of inkoopcreditnota's hebt waarbij geen aantal is opgegeven op de regels.  

## <a name="see-also" />Zie ook
 [Validatie van inkoopbedragen instellen](how-to-set-up-validation-of-purchase-amounts.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
