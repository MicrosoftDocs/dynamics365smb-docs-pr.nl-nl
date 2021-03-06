---
title: Verkooprapporten en analyses
description: Bekijk welke verkooprapporten en analyses beschikbaar zijn in de standaardversie van Business Central, zodat u uw bedrijf kunt volgen.
author: AndreiPanko
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.search.keywords: reporting
ms.date: 06/01/2021
ms.author: andreipa
ms.openlocfilehash: a8ada1c8488e8c5dec581db98dccf02d89da21c3
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/09/2021
ms.locfileid: "6216339"
---
# <a name="sales-reports-and-analytics-in-business-central"></a>Verkooprapporten en analyses in Business Central

Verkooprapportage in [!INCLUDE [prod_short](includes/prod_short.md)] stelt verkoop- en zakelijke professionals in staat om inzichten en statistieken te krijgen over huidige en vroegere verkoopactiviteiten.  

## <a name="reports"></a>Rapporten

De volgende tabel beschrijft enkele van de belangrijkste rapporten in verkooprapportage.

|Rapport |Object-id|Omschrijving  |
|---------|---------|---------|
|**Klant - Samenvatting orders**|107| Toont de orderdetails met het nog niet verzonden aantal voor elke klant in drie perioden van dertig dagen, vanaf de opgegeven datum. Er zijn ook kolommen met orders die voor en na deze drie perioden moeten worden verzonden en een kolom met het totale orderoverzicht voor elke klant. Gebruik het rapport om het verwachte verkoopvolume van een bedrijf te analyseren. |
|**Klant - Top 10**|111| Toont gegevens over inkopen en saldi van klanten voor een geselecteerde periode. U kunt het nummer opgeven van klanten die u in het rapport wilt opnemen. Klanten worden alleen opgenomen als ze tijdens de periode inkopen hebben gedaan of aan het einde van de periode een saldo hebben.<br>De klanten worden op bedrag gesorteerd en u kunt aangeven of op verkoopbedrag of op saldo moet worden gesorteerd. In het rapport kunt u in een oogopslag zien welke klanten de meeste inkopen hebben gedaan of het hoogste saldo hebben openstaan.|
|**Verkoop klant/artikel**|113|Geeft een overzicht aan van artikelverkopen per klant tijdens een geselecteerde periode. In het rapport vindt u gegevens over aantallen, verkoopbedragen, winstbedragen en mogelijke kortingen. Met de lijst kunt u bijvoorbeeld de klantengroepen van een bedrijf analyseren.|
|**Voorraad - Klantverkoop**|713|Een overzicht vanuit het perspectief van het magazijn. Dit is een andere weergave dan het rapport **Verkoop klant/artikel** en toont eerst het artikel en vervolgens de klant die dit product heeft gekocht.|
|**Klant - Verkooplijst**|119|Toont het verkoopoverzicht voor een periode. De lijst is bedoeld voor de belastingdienst en de douane. U kunt desgewenst alleen klanten opnemen voor wie de totale verkoopcijfers een minimumbedrag overschrijden. U kunt ook aangeven of u de adresgegevens van de klanten in de lijst wilt weergeven.<br>De lijst is gebaseerd op de verkoop (LV) die is vastgelegd in klantenposten. Onder aan de lijst wordt de totale gerapporteerde verkoop weergegeven in lokale valuta. Het totaal is gebaseerd op de klanten die in de lijst zijn opgenomen, dat wil zeggen: de klanten die zijn geselecteerd met de filters op het sneltabblad Klant en waarvan de totale verkoop groter is dan het bedrag in het veld **Bedragen (LV) groter dan** op het sneltabblad **Opties**.|
|**Klant - Saldo t/m datum**|121|Bevat een gedetailleerd saldo voor geselecteerde klanten. Gebruik het rapport bijvoorbeeld bij het afsluiten van een boekhoudperiode of boekjaar.|
|**Klant - Proefbalans**|129|Bevat een gedetailleerd saldo voor geselecteerde klanten. Met de lijst kunt u controleren dat het saldo van een klantboekingsgroep op een bepaalde datum gelijk is aan het saldo van de bijhorende grootboekrekening. Gebruik het rapport bijvoorbeeld bij het afsluiten van een boekhoudperiode of boekjaar. Als u een meer gedetailleerde versie van dit type rapport nodig heeft, gebruikt u het rapport **Proef- en saldibalans klantgegevens** (104).|
|**Verkoopstatistiek**|112|Bevat verkoop, winst, factuur- en contantkortingen in de lokale valuta en winstpercentages per klant. De kosten en winst worden gegeven als oorspronkelijk en geherwaardeerd. De oorspronkelijke kosten en winst zijn berekend op het moment van boeken en de geherwaardeerde kosten en winst weerspiegelen wijzigingen in de oorspronkelijke kosten van de verkochte artikelen. Het kostenwaarderingsbedrag in het rapport is het verschil tussen de oorspronkelijke kosten en de geherwaardeerde kosten.<br>De cijfers zijn verdeeld in drie perioden. U kunt de lengte van deze perioden selecteren, waarbij ze beginnen op een geselecteerde datum. De lijst bevat ook kolommen voor bedragen vóór en na de drie perioden. Gebruik het rapport om bijvoorbeeld een analyse te maken van de opbrengsten per klant en opbrengstenontwikkeling. |
|**Beschikbaar voor levering**|209|Bevat informatie over de beschikbaarheid van artikelen voor verzending op verkoopdocumenten. U bepaalt of u de status van elk document of van elke verkoopregel in de lijst wilt weergeven. Wanneer u de lijst afdrukt, kunt u ook het aantal dat voor verzending beschikbaar is, bijwerken in het veld **Te verzenden aantal** op de verkoopregels. Vervolgens kunt u op basis van de lijst bepalen welke documenten u wilt boeken.<br>Er is ook een mogelijkheid waarmee u de hoeveelheid te verzenden goederen kunt instellen. **opmerking**: dit rapport is niet beschikbaar voor geavanceerde magazijnfunctionaliteit.|
|**Status van magazijnverzending**|7313|Dit rapport kan gebruikt worden voor alle locaties waar het veld **Verzending vereist** is geselecteerd. Het rapport **Verzendstatus magazijn** toont alle niet-geboekte magazijnverzendingsdocumenten, inclusief de locaties, magazijncodes, documentstatus, hoeveelheden, enzovoort. Dit rapport is perfect om een overzicht te krijgen.|
|**Voorraad - Picklijst**|813|Geeft een lijst met verkooporders weer waarin een artikel is opgenomen. De volgende gegevens worden voor elk artikel weergegeven: verkooporderregel met naam van de klant, variantcode, vestigingscode, opslaglocatiecode, verzenddatum, te verzenden aantal en maateenheid. Het te verzenden aantal wordt voor elk artikel opgeteld. U kunt de lijst gebruiken wanneer artikelen uit de voorraad worden verzameld.<br>**opmerking**: dit rapport is niet beschikbaar voor geavanceerde magazijnfunctionaliteit.|
|**Voorraad: verkoopbackorders**|718|Geeft een lijst met orderregels weer waarvoor de verzenddatum is overschreden. De volgende gegevens worden voor de afzonderlijke orders voor elk artikel weergegeven: nummer, klantnaam, telefoonnummer van de klant, verzenddatum, orderaantal en aantal in backorder. In de lijst wordt ook weergegeven of er andere artikelen voor de klant zijn nabesteld.|



## <a name="tasks"></a>Taken

In de volgende artikelen worden enkele van de belangrijkste taken beschreven voor het analyseren van de toestand van uw bedrijf:

* [Analyselijsten maken](bi-how-create-analysis-views-reports.md)  
* [Beschikbaarheid van artikelen weergeven](inventory-how-availability-overview.md)


## <a name="see-also"></a>Zie ook

[Verkopen instellen](sales-setup-sales.md)  
[Verkoop](sales-manage-sales.md)  
[Artikelen reserveren](inventory-how-to-reserve-items.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
