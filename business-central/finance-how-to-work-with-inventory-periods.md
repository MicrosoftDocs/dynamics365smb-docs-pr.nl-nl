---
title: Werken met inventarisperiodes
description: U kunt bepalen in welke periode mensen wijzigingen in voorraad kunnen boeken door voorraadperioden te definiëren.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'inventory, periods'
ms.search.form: 5828
ms.date: 07/29/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Werken met inventarisperiodes

Een voorraadperiode is een periode waarin gewijzigde voorraadwaarden kunnen worden geboekt. Een voorraadperiode wordt begrensd door een einddatum. Wanneer u een voorraadperiode Sluiten gebruikt, kunt u vóór deze einddatum geen wijzigingen in de voorraad doorvoeren, noch verwacht noch gefactureerd. U kunt vóór de einddatum geen nieuwe waarden naar de inventaris boeken. Als u openstaande posten hebt in de afgesloten periode, dat wil zeggen positieve hoeveelheden die nog niet zijn toegepast op uitgaande transacties, kunt u uitgaande hoeveelheden nog steeds op deze posten toepassen, zelfs als de periode is afgesloten.  

In de volgende secties wordt uitgelegd hoe u:

* Voorraadperioden maken.  
* Voorraadperioden afsluiten.  
* Voorraadperioden opnieuw openen.  

## Een voorraadperiode maken

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Voorraadperioden** in en kies vervolgens de gerelateerde koppeling.  
2. Een nieuwe regel maken.  
3. Voer in het veld **Einddatum** de laatste datum van de voorraadperiode in die u wilt definiëren. Wanneer de periode is afgesloten, kunt u vóór deze datum geen voorraadwijzigingen meer boeken.  
4. Typ een beschrijvende naam in het veld **Naam**. Kies de knop **Ok**.  

## Naar Sluiten inventarisperiodes

Het veld **Gesloten** geeft aan of de voorraadperiode afgesloten is voor wijzigingen in voorraadwaarden. U kunt dit veld niet bewerken.  

U kunt Sluiten gebruiken voor elke inventarisperiode, als het volgende van toepassing is:  

* De periode bevat geen openstaande uitgaande artikelposten, dat wil zeggen negatieve voorraad.  
* De kosten van alle artikelen zijn aangepast met gebruik van de batchverwerking **Kostprijs herwaarderen - Artikelposten**.  

Dit betekent dat alle uitgaande transactieaantallen, zoals de aantallen van verkooporders, uitgaande transfers, verkoopfacturen, inkoopretourorders of inkoopcreditnota's, moeten worden vereffend met bestaande aantallen in de voorraad.  

### Een voorraadperiode afsluiten  

1. Voordat u een voorraadperiode sluit, kiest u de actie **Kosten corrigeren – Artikelposten** om ervoor te zorgen dat alle kostencorrecties worden geboekt.

    Voer het rapport **Sluiten Inventarisperiode – Test**  uit om te bepalen of er openstaande uitgaande artikelposten zijn binnen de inventarisperiode of artikelen waarvan de kosten nog niet zijn aangepast.  
2. Kies de actie **Testrapport**.  

    Voer de batchverwerking **Voorraadwaarde boeken** uit om ervoor te zorgen dat alle kosten naar het grootboek zijn geboekt.  
3. Kies de actie **Van Voorraadbeheer naar GB boeken**.  
4. Selecteer op de pagina **Voorraadperioden** de voorraadperiode die u wilt sluiten.  
5. Kies de actie **Periode afsluiten**. Nadat de inventarisperiode is afgesloten, kunt u geen inventariswijzigingen meer boeken vóór de einddatum. U dient de kosten van alle artikelen te herwaarderen met de batchverwerking **Kostprijs herwaarderen - Artikelposten** voordat u de voorraadperiode afsluit.  
6. Kies de knop **Ja** om te bevestigen dat u de periode wilt afsluiten of kies **Nee** om het afsluiten te annuleren.  
7. De inventarisatieperiode is gesloten en er wordt een bevestigingsbericht weergegeven wanneer deze is afgelopen.  

## Heropening van inventarisperiodes  
Nadat u de inventarisperiode hebt gesloten, kunt u deze niet meer verwijderen. U kunt de periode echter wel weer opnieuw openen als u boekingen vóór de einddatum van de voorraadperiode wilt toestaan. Wanneer u een periode opnieuw opent, worden alle voorraadperioden met latere einddatums ook weer geopend.  

### Een voorraadperiode opnieuw openen  
1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Voorraadperioden** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer de voorraadperiode die u opnieuw wilt openen.  
3. Kies de periodeactie **Periode opnieuw openen**. Bevestig dat u de periode opnieuw wilt openen.  
4. Alle voorraadperioden met latere einddatums dan de geselecteerde periode worden eveneens opnieuw geopend.  

## Zie ook  
[Ontwerpdetails: Inventarisperioden](design-details-inventory-periods.md)    
[Financiën](finance.md)    
[Voorraad](inventory-manage-inventory.md)    
[Werken met Financials](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]