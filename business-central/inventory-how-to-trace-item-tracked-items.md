---
title: Artikelen met artikeltracering traceren
description: U kunt zien waar een artikel met artikeltracering is gebruikt, inclusief hoe en wanneer dit is ontvangen of geproduceerd, overgebracht, verkocht, verbruikt of geretourneerd. U kunt tevens alle huidige exemplaren van een bepaald serie- of lotnummer in de database vinden. Dit doet u met behulp van de functies Artikeltracering en Posten zoeken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: bbfe0237beb58f22d3be7bc388d7b2726f05d4ba
ms.sourcegitcommit: 0953171d39e1232a7c126142d68cac858234a20e
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/09/2021
ms.locfileid: "6214750"
---
# <a name="trace-item-tracked-items"></a>Artikelen met artikeltracering traceren
U kunt zien waar een artikel met artikeltracering is gebruikt, inclusief hoe en wanneer dit is ontvangen of geproduceerd, overgebracht, verkocht, verbruikt of geretourneerd. U kunt tevens alle huidige exemplaren van een bepaald serie- of lotnummer in de database vinden. Dit doet u met behulp van de functies Artikeltracering en [Posten zoeken](ui-find-entries.md).  

Deze functies zijn vooral handig tijdens het uitvoeren van kwaliteitscontroles wanneer u wilt weten welke klanten producten met een bepaald lotnummer hebben ontvangen of wanneer u wilt weten uit welk lot een defect onderdeel afkomstig is.  

 Op de pagina **Artikeltracering** kunt u voorwaarts en achterwaarts traceren in een reeks van geboekte voorraadtransacties voor het serie- of lotnummer.  

 Op de pagina **Posten zoeken** kunt u niet de reeks transacties bekijken, maar wel alle records van het serie- of lotnummer, zowel geboekte posten als open records.  

 De twee functies kunnen in combinatie worden gebruikt door een getraceerd serie- of lotnummer over te brengen naar de pagina **Posten zoeken** om een volledig traceerscenario te voltooien. <!-- For more information, see [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md).   -->

## <a name="to-trace-item-tracked-items"></a>Artikelen met artikeltracering traceren  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Artikeltracering** in en kies de gerelateerde koppeling.  
2.  In de filtervelden boven aan de pagina geeft u de specifieke artikelnummers op of een filter voor de artikelnummers die u wilt traceren.  
3.  Selecteer in het veld **Onderdelen weergeven** of u ook wilt zien waar de onderdelen voor de artikelen vandaan komen. U beschikt over de volgende opties in dit veld.  

    |Veld|Description|  
    |----------------------------------|---------------------------------------|  
    |**Nee**|Selecteer deze optie als u geen onderdelen wilt weergeven.|  
    |**Met artikeltracering**:|Selecteer deze optie als u alleen onderdelen met lot- of serienummers wilt weergeven.|  
    |**Alle**|Selecteer deze optie als u alle onderdelen wilt weergeven.|  

4.  Selecteer in het veld **Traceringsmethode** de methode waarmee u het artikel wilt traceren. De volgende opties zijn beschikbaar  

    |Veld|Description|  
    |----------------------------------|---------------------------------------|  
    |**Gebruik->Oorsprong**|Met deze methode wordt het artikel getraceerd vanaf waar het is gebruikt tot waar het vandaan kwam. Als een geproduceerd artikel bijvoorbeeld is verkocht aan een klant, ziet u dat op de pagina **Artikeltracering**, waarbij de verkoopverzendingsregel eerst wordt weergegeven. U kunt deze regel uitbreiden om de afkomst van de productieorder te zien.|  
    |**Oorsprong->Gebruik**|Met deze methode wordt het item getraceerd vanaf waar het in de voorraad is opgenomen tot waar het is gebruikt. Als een geproduceerd artikel bijvoorbeeld aan een klant is verkocht, ziet u dit op de pagina **Artikeltracering** waarbij de voltooide productieorder eerst wordt weergegeven. U kunt deze order uitbreiden om de verkoopverzendingsregels waarin het artikel wordt gebruikt weer te geven.|  

5.  Kies de actie **Traceren** om de tracering uit te voeren.  

> [!NOTE]  
>  Als u dezelfde partij via meer transacties hebt ontvangen, worden op de pagina **Artikeltracering** mogelijk niet alle transacties weergegeven. Alleen vereffende transacties worden weergegeven.  

> [!NOTE]  
>  Als al extra transactiegeschiedenis onder een artikeltraceringsregel is getraceerd door een andere bovenliggende regel, wordt het selectievakje **Al getraceerd** ingeschakeld. Voor een eenvoudiger weergave worden dergelijke onderliggende regels niet weergegeven.  
>   
>  Als u de artikeltraceringsregels wilt zoeken waarin de transactiegeschiedenis al is getraceerd, kiest u de knop **Ga naar Reeds getraceerd**. De desbetreffende artikeltraceringsregel is geselecteerd en alle onderliggende regels zijn uitgevouwen.  

## <a name="to-find-item-tracked-items-with-find-entries"></a>Artikelen met artikeltracering zoeken met Posten zoeken  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Posten zoeken** in en selecteer de gerelateerde koppeling.  
2. Kies **Acties** > **Zoeken op** > **Zoeken op artikelverwijzing**.
3. Voer in de velden **Serienr.** en **Lotnr.** de artikeltraceringsnummers in die u wilt traceren.  
4. Kies de actie **Zoeken** om alle exemplaren van het serie- of lotnummer in de database te zoeken.  

## <a name="see-also"></a>Zie ook

[Voorraad](inventory-manage-inventory.md)  
[Werken met serie-, lot- en pakketnummers](inventory-how-work-item-tracking.md)  
[Ontwerpdetails: Artikeltracering](design-details-item-tracking.md)  
[Ontwerpdetails: Artikeltracering en reserveringen](design-details-item-tracking-and-reservations.md)  
[Artikelen reserveren](inventory-how-to-reserve-items.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
<!-- [Walkthrough: Tracing Serial-Lot Numbers](walkthrough-tracing-serial-lot-numbers.md)   -->
[Posten zoeken](ui-find-entries.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]