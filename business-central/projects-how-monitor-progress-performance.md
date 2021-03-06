---
title: Een OHW-methode definiëren en projectvoortgang controleren| Microsoft Docs
description: Beschrijft hoe u een OHW-methode (onderhanden werk) kunt maken en OHW kunt berekenen om de financiële waarde van projecten in te schatten terwijl ze bezig zijn.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, KPI, work in process, work in progress
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: fac1c041108cacfcabf18b04d128949d05e1d283
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938118"
---
# <a name="monitor-job-progress-and-performance"></a>Voortgang en prestaties van projecten bewaken
Naarmate een project vordert, worden materialen, resources en overige zaken verbruikt en moeten hiervoor boekingen plaatsvinden op het project. Onderhanden werk (OHW) is een functie waarmee u de financiële waarde van projecten in het grootboek kunt schatten gedurende de projecten. In veel gevallen kunt u kosten voor een project boeken voordat u het project factureert. Wanneer alleen kosten zijn geboekt, klopt het financiële afschrift niet. Zie [OHW-methoden](projects-understanding-wip.md) voor meer informatie.

Als u de waarde in het grootboek wilt volgen, kunt u het OHW-bedrag berekenen en de waarde boeken in het grootboek.

U kunt het OHW-bedrag berekenen op basis van de volgende zaken:

* Kostprijs
* Verkoopprijs
* Kostprijs van omzet
* Percentage voltooid
* Contract voltooid

Als u het resultaat met een andere methode wilt bekijken, kunt u de methode wijzigen en het OHW-bedrag nogmaals berekenen. U kunt net zo vaak het OHW-bedrag berekenen als u wilt. Het OHW-bedrag wordt alleen berekend en wordt niet geboekt in het grootboek. Na het berekenen van het OHW-bedrag, kunt u het OHW-bedrag boeken in het grootboek.

## <a name="to-create-a-job-wip-method"></a>Een OHW-methode voor een project maken
U kunt een OHW-methode voor een project maken die de behoeften van uw organisatie weerspiegelt. Nadat u deze methode hebt gemaakt, kunt u deze instellen als standaard OHW-berekeningsmethode voor een project die wordt gebruikt in uw organisatie.  

> [!NOTE]
> Nadat u uw nieuwe methode hebt gebruikt om OHW-posten te maken, kunt u de methode niet meer verwijderen of wijzigen.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **OHW-methoden taak** in en kies de gerelateerde koppeling.  
2. Kies de actie **Nieuw** en vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Sluit de pagina.   
4. Als u van deze nieuwe methode de standaard wilt maken, kiest u pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voert u **Projectinstellingen** in en kiest u vervolgens de gerelateerde koppeling.  
5. Kies in het veld **Standaard OHW-methode** de methode uit de lijst.

## <a name="to-define-a-wip-method-for-a-job"></a>Een OHW-methode voor een project definiëren
Wanneer u een nieuw project maakt, moet u opgeven welke OHW-methode voor het project van toepassing is. In sommige gevallen is de OHW-methode voor het project die u kunt gebruiken standaard voor u ingesteld.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projecten** in en kies de desbetreffende koppeling.
2. Kies de actie **Nieuw**. Zie voor meer informatie [Projecten maken](projects-how-create-jobs.md).  
3. Selecteer op de pagina **Projectkaart** in het veld **OHW-methode** een OHW-methode uit de lijst. Als een standaardmethode is gedefinieerd, kunt u indien nodig een andere optie selecteren.  

## <a name="to-calculate-wip"></a>OHW berekenen
U kunt het OHW-bedrag bepalen dat moet worden geboekt naar balansrekeningen voor eindrapportage van een periode. U gebruikt hiervoor de batchverwerking **OHW voor project berekenen**.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **OHW voor project berekenen** in en kies de gerelateerde koppeling.  
2. Kies de actie **OHW berekenen**.
3. Vul op de pagina **OHW voor project berekenen** indien nodig de velden in.
4. Kies de knop **OK**.  

> [!NOTE]  
>   De batchverwerking berekent alleen het OHW. Het wordt niet geboekt in het grootboek. Hiervoor moet u de batchverwerking **OHW naar GB boeken** uitvoeren wanneer u het onderhanden werk hebt berekend. Zie de volgende procedure voor meer informatie.

## <a name="to-post-wip"></a>OHW boeken
Wanneer u OHW hebt berekend, kunt u het boeken naar balansrekeningen voor de einddatumrapportage. Hiervoor gebruikt u de batchverwerking **Project-OHW naar GB boeken**.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Project-OHW naar GB boeken** in en kies de gerelateerde koppeling.  
2. Vul op de pagina **Project-OHW naar GB boeken** indien nodig de velden in.  
3. Kies de knop **Ok**.

## <a name="to-calculate-and-post-job-completion-entries"></a>Projectvoltooiingsposten berekenen en boeken
Wanneer u alle activiteiten voor een project hebt uitgevoerd, waaronder gebruiksboekingen en -facturering, moet u het project bijwerken om de **Status** in te stellen op **Voltooid**. Vervolgens moet u eventueel OHW tegenboeken dat naar het grootboek is geboekt.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projecten** in en kies de desbetreffende koppeling.  
2. Selecteer een open project en kies vervolgens de actie **Bewerken**.
3. Selecteer in het veld **Status** de optie **Voltooid**.
4. Volg de hulpstappen om OHW te berekenen en te boeken. Of volg stap 5 en 6 om dit handmatig te doen.  
5. Kies de actie **OHW berekenen**.
6. Vul op de pagina **OHW voor project berekenen** indien nodig de velden in.  

     De OHW-posten voor het project die worden gemaakt door het uitvoeren van de batchverwerking, hebben nu een vinkje in het selectievak **Project voltooid** om aan te geven dat het voltooiingsposten zijn.  
7. Kies de actie **Project-OHW naar GB boeken**.
8. Vul op de pagina **Project-OHW naar GB boeken** indien nodig de velden in.  

     De OHW-grootboekposten voor het project die worden gemaakt door het uitvoeren van de batchverwerking hebben nu een vinkje in het selectievak **Project voltooid** om aan te geven dat het voltooide posten zijn.

## <a name="to-view-job-ledger-entries"></a>Projectposten bekijken
Alle posten met betrekking tot een project worden in projectjournalen opgeslagen en sequentieel genummerd, te beginnen met 1. Vanuit het projectjournaal hebt u een overzicht van alle projectposten.    

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projectjournalen** in en kies de gerelateerde koppeling.
2. Selecteer een relevant journaal en kies vervolgens de actie **Projectposten**.

De pagina **Projectposten** wordt geopend, waarin u de posten die zijn gekoppeld aan een project, kunt bekijken.  

## <a name="see-also"></a>Zie ook
[Projecten beheren](projects-manage-projects.md)
[Voorraadkosten beheren](finance-manage-inventory-costs.md)   
[Financiën](finance.md)  
[Inkoop](purchasing-manage-purchasing.md)         
[Verkoop](sales-manage-sales.md)      
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
