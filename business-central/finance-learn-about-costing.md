---
title: Over voorraadkostenberekening
description: 'Het beheren van voorraadkosten heeft alles te maken met het vastleggen en rapporteren van bedrijfskosten, inclusief het rapporteren van productiekosten en voorraadkosten.'
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 07/26/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="about-inventory-costing"></a>Over voorraadkostenberekening
Voorraadkosten beheren heeft betrekking op het registreren en rapporteren van operationele bedrijfskosten. Dit omvat de rapportage van productie- en voorraadkosten (dus de waarde van artikelen).  

 U dient de volgende centrale principes te begrijpen: met waarderingsmethoden wordt gedefinieerd hoe artikelen worden gewaardeerd wanneer ze de voorraad verlaten, met een herwaardering van kosten worden de kosten bijgewerkt van goederen die worden verkocht met gerelateerde inkoopkosten die na de verkoop zijn geboekt en de voorraadwaarden moeten regelmatig worden geboekt naar speciale grootboekrekeningen.  

 De volgende tabel beschrijft een reeks taken, met koppelingen naar de artikelen waarin deze worden beschreven.   

|**Functie**|**Zie**|  
|------------|-------------|  
|Het verschil te leren tussen de vijf verschillende waarderingsmethoden en hun effect op kostenstromen.|[Ontwerpdetails: Waarderingsmethoden](design-details-costing-methods.md)|  
|Meer te weten te komen over hoe artikelvereffeningsposten voorraadafnames en -toenames dynamisch aan elkaar koppelen om controle te houden over de kostenstromen.|[Ontwerpdetails: Artikelvereffening](design-details-item-application.md)|  
|Meer te weten te komen over hoe de eenheidsprijs van een artikel voortdurend wordt bijgewerkt met de kosten van de recentste transactie ervan volgens de waarderingsmethode van het artikel.|[Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md)|  
|Meer te weten te komen over hoe de gemiddelde kostprijs van een artikel dynamisch wordt berekend aan de hand van de geselecteerde periode voor gemiddelde kostprijsberekening.|[Ontwerpdetails: Gemiddelde kostprijs](design-details-average-cost.md)|  
|Maak onderscheid tussen verwachte kosten (nog niet gefactureerd) en werkelijke kosten en leer hoe deze worden beheerd in grootboek.|[Ontwerpdetails: Verwachte-kostenboeking](design-details-expected-cost-posting.md)|  
|Het herwaarderingsmechanisme voor kosten te begrijpen, dat ervoor zorgt dat kosten naar voren komen, zelfs wanneer voorraadtransacties willekeurig plaatsvinden.|[Ontwerpdetails: Kostenwaardering](design-details-cost-adjustment.md)|  
|Te lezen waarom vaste verrekenprijzen vaak worden gebruikt door productiebedrijven als een waarderingsbasis voor onderdelen en eindartikelen.|[Informatie over het berekenen van vaste verrekenprijzen](finance-about-calculating-standard-cost.md)|  
|Te begrijpen hoe de voorraadwaarde wordt weerspiegeld in het grootboek.|[Voorraadkosten reconciliëren met het grootboek](finance-how-to-post-inventory-costs-to-the-general-ledger.md)|  
|Meer te weten te komen over hoe artikeltoeslagen, zoals verzendkosten en verzekering, extra kostenonderdelen kunnen toewijzen aan de eenheidsprijs van een artikel.|[Artikeltoeslagen gebruiken om extra handelskosten te verantwoorden](payables-how-assign-item-charges.md)|  
|Te lezen hoe voorraadperioden een bedrijf kunnen helpen de voorraadwaarde gedurende de tijd te beheren door kortere perioden te definiëren die gedurende het boekjaar voor boeking kunnen worden gesloten.|[Werken met voorraadperioden](finance-how-to-work-with-inventory-periods.md)|  
|Alle mechanismen in de kostprijsberekeningengine begrijpen, inclusief wat er gebeurt wanneer u assemblage- en productietransacties boekt.|[Ontwerpdetails: Voorraadwaardering](design-details-inventory-costing.md)|  

## <a name="see-also"></a>Zie ook
[Voorraadkosten beheren](finance-manage-inventory-costs.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
