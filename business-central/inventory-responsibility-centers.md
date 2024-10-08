---
title: Hoe te werken met verantwoordelijkheidscentra
description: Divisie als beheercentra helpen bedrijven gebruikersspecifieke weergaven in te stellen van verkoop- en inkoopdocumenten die uitsluitend betrekking hebben op een bepaalde divisie.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.search.forms: '5714, 5715'
ms.date: 05/16/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# <a name="work-with-responsibility-centers"></a>Werken met verantwoordelijkheidscentra

Divisies bieden mogelijkheden voor beheercentra. Een divisie kan een kostencentrum, een winstcentrum, een investeringscentrum of een ander door het bedrijf gedefinieerd administratief centrum zijn. Voorbeelden van divisies zijn een verkoopkantoor, een inkoopafdeling voor meerdere locaties en een planningskantoor voor een fabriek. Bedrijven kunnen bijvoorbeeld gebruikersspecifieke weergaven van verkoop- en inkoopdocumenten met betrekking tot een bepaalde divisie instellen.  

Het gebruik van meerdere locaties in combinatie met verantwoordelijkheidscentra biedt de mogelijkheid om de bedrijfsvoering op flexibele, optimale manieren te beheren.

Bedrijven met meerdere locaties kunnen hun voorraad op meerdere locaties beheren met behulp van één database. De hoekstenen van deze granule zijn twee concepten: locaties en SKU's. Een locatie is een plaats waar de fysieke plaatsing en aantallen van artikelen worden verzorgd. Het concept is breed genoeg om locaties zoals fabrieken of productiefaciliteiten en distributiecentra, magazijnen, showrooms en servicevoertuigen te omvatten. Een SKU is een artikel op een bepaalde locatie en/of een variant. Met SKU's kunnen bedrijven met meerdere locaties aanvullingsgegevens, adressen en bepaalde financiële boekingsgegevens toevoegen op vestigingsniveau. Hierdoor kunnen ze varianten van hetzelfde artikel voor elke locatie aanvullen en artikelen bestellen op basis van locatie-specifieke bevoorradingsinformatie.  

## <a name="to-set-up-a-responsibility-center"></a>Een divisie instellen

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Divisies** in en kies de gerelateerde koppeling.  
2. Kies de actie **Nieuw**.  
3. Vul de vereiste velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

    Als u divisies gebruikt om uw bedrijf te beheren, kan het handig zijn om een standaarddivisie voor uw bedrijf te hebben.
4. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bedrijfsgegevens** in en kies vervolgens de gerelateerde koppeling.
5. Voer op het sneltabblad  **Verzending** in het veld  **Verantwoordelijkheidscentrum** een code voor het verantwoordelijkheidscentrum in.

Deze code wordt in alle inkoop-, verkoop- of servicedocumenten gebruikt als de gebruiker, klant of leverancier geen standaarddivisie heeft. In alle verkoop-, inkoop- of servicedocumenten kunt u een andere divisie invoeren dan de standaarddivisie.

> [!NOTE]  
> Wanneer u een divisiecode in een document invoert, heeft dit invloed op het adres, de dimensies en de prijzen in het document.  

## <a name="to-assign-responsibility-centers-to-users"></a>Divisies toewijzen aan gebruikers

Voor gebruikers kunt u instellen dat [!INCLUDE [prod_short](includes/prod_short.md)] alleen de documenten ophaalt die van toepassing zijn op de werkgebieden van de gebruikers. Gebruikers zijn gekoppeld aan één verantwoordelijkheidscentrum en werken uitsluitend met documenten die betrekking hebben op specifieke toepassingsgebieden in dat specifieke centrum.  

Als u dit wilt instellen, moet u divisies toewijzen aan gebruikers in drie basismodules: Inkoop, Verkoop en CRM - Service.  

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Gebruikersinstellingen** in en kies vervolgens de gerelateerde koppeling.  
2. Ga op de pagina **Gebruikersinstellingen** naar de gebruiker waaraan u een divisie wilt toewijzen. Als de gebruiker niet voorkomt in het overzicht, moet u een gebruikers-id invoeren in het veld **Gebruikers-id**.  
3. In het veld **Verkoopdivisiefilter** voert u de divisie in waaraan de verkooptaken van de gebruiker zijn gekoppeld.  
4. In het veld **Inkoopdivisiefilter** voert u de divisie in waaraan de inkooptaken van de gebruiker zijn gekoppeld.  
5. In het veld **Servicedivisiefilter** voert u de divisie in waaraan de servicebeheertaken van de gebruiker zijn gekoppeld.  

> [!NOTE]  
> Gebruikers kunnen alleen die geboekte documenten bekijken die betrekking hebben op hun eigen verantwoordelijkheidscentrum. Ze kunnen echter alle grootboekposten bekijken en vanuit de grootboekposten naar andere geboekte documenten navigeren.

## <a name="see-also"></a>Zie ook

[Inventaris instellen](inventory-setup-inventory.md)    
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)    
[Voorraad](inventory-manage-inventory.md)    
[Overzicht van magazijnbeheer](design-details-warehouse-management.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    
[Definieer een beleid voor het boeken van facturen voor gebruikers](admin-setup-invoice-posting-policy.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
