---
title: 'Validatie van inkoopbedragen instellen [NL]'
description: Activeer de functie Totaalbedragen documenten controleren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt.
author: SorenGP
ms.topic: conceptual
ms.search.keywords: null
ms.date: 06/25/2021
ms.author: edupont
---
# <a name="set-up-validation-of-purchase-amounts-in-the-dutch-version" />Validatie van inkoopbedragen instellen in de Nederlandse versie
In [!INCLUDE[prod_short](../../includes/prod_short.md)] kunt u de functie **Totaalbedragen documenten controleren** activeren om het totaalbedrag van inkoopdocumenten te valideren voordat een inkoopfactuur en inkoopcreditnota worden geboekt. Standaard wordt het totale inkoopdocumentbedrag gevalideerd wanneer u boekt. Het totale bedrag van de ingevoegde inkoopregels moet gelijk zijn aan het bedrag inclusief btw en het btw-bedrag. Als u het inkoopdocumentbedrag automatisch wilt valideren, moet u het documentbedrag inclusief btw en de btw van het documentbedrag op de pagina **Inkoopfactuur** of **Inkoopcreditnota** invoeren.  

Als u slechts één inkoopregel of meer verkoopregels met hetzelfde btw-percentage hebt, wordt de juiste documentbedrag-btw automatisch berekend wanneer u de inkoopregels en het documentbedrag inclusief btw invoegt. Als u verschillende inkoopregels met verschillende btw-percentages hebt, moet de waarde van de documentbedrag-btw handmatig worden gewijzigd.  

U kunt ook bepalen wanneer de documenttotaalbedragen en de totaalbedragen van de ingevoegde inkoopregels verschillen. U kunt de optie **Totale op inkoopfactuur/CR-nota weergeven** activeren om het volgende weer te geven in de ingevoegde inkoopregels:  

- Totaalbedrag  
- Totaalbasisbedrag  
- Totaal btw-bedrag  
- Totaalbedrag incl. btw  

De berekende bedragen worden weergegeven in de inkoopfactuur of de inkoopcreditnota. Standaard wordt dit totaalbedrag niet weergegeven.  

U kunt deze optie alleen inschakelen als de inkoopfactuur of de inkoopcreditnota het volgende heeft:  

- Een minimum van één inkoopregel.  
- Het aantalveld opgegeven.  

## <a name="to-set-up-validation-of-total-amounts-for-purchase-documents" />Validatie van totaalbedragen voor inkoopdocumenten instellen

1.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Inkoopinstellingen** in en kies vervolgens de gerelateerde koppeling.  
2.  Vul in het sneltabblad **Algemeen** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Totale op inkoopfactuur/CR-nota weergeven.**|Selecteren om de totalen opnieuw te berekenen van alle inkoopfacturen en creditnota's. Dit kan een tijdrovend proces zijn, afhankelijk van het aantal documenten dat moet worden herberekend.|  
    |**Totaalbedragen documenten controleren**|Selecteer om de velden **Documentbedrag incl. btw** en **Btw documentbedrag** op de pagina's **Inkoopfactuur** en **Inkoopcreditnota** te wijzigen.|  

3.  Kies de knop **OK**.  

## <a name="see-also" />Zie ook
[Nederlandse lokale functionaliteit](netherlands-local-functionality.md)  
[Inkopen instellen](../../sales-how-work-standard-lines.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
