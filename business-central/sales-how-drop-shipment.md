---
title: Doorverzendingen maken
description: Hierin wordt beschreven hoe u een verkooporder kunt maken die is gekoppeld aan een inkooporder om verzending direct van de leverancier naar de klant mogelijk te maken.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: direct shipment
ms.date: 05/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="make-drop-shipments"></a>Doorverzendingen maken

Een doorverzending is de directe verzending van artikelen van een van uw leveranciers naar een van uw klanten.

Wanneer een verkooporder gemarkeerd is voor doorverzending en u een inkooporder maakt met de klant in het veld **Verzenden naar**, **Klantadres**, kunt u de twee documenten koppelen en zo de leverancier instrueren om rechtstreeks naar de klant te verzenden.
<br><br>  
  
> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mOyM?rel=0]

## <a name="to-create-a-sales-order-for-drop-shipment"></a>Een verkooporder voor doorverzending maken

Ter voorbereiding op een doorverzending maakt u een verkooporder voor een artikel en geeft u op de verkoopregel aan dat voor de verkoop doorverzending vereist is.

1. Maak een verkooporder voor een artikel. Zie [Producten verkopen](sales-how-sell-products.md) voor meer informatie.
2. Op de verkooporderregel voor de doorverzending schakelt u het selectievakje **Doorverzending** in. Of selecteer in het veld **Inkoopcode** een inkoopcode waarbij het veld **Doorverzending** is geselecteerd.

> [!TIP]
> Het selectievakje Doorverzending en het veld Inkoopcode zijn standaard niet beschikbaar op de regels. Als dit niet het geval is, kunt u ze toevoegen door het gedeelte van de pagina dat de regels bevat te personaliseren. Zie [Uw werkruimte personaliseren](ui-personalization-user.md) voor meer informatie.

## <a name="to-create-the-purchase-order-for-drop-shipment"></a>De inkooporder voor doorverzendingen maken

Om een doorverzending voor te bereiden geeft u op de inkooporder aan dat deze naar uw klant moet worden verzonden, niet naar uzelf.

1. Inkooporder maken. Vul geen velden op de regels in. Zie voor meer informatie [Inkopen vastleggen](purchasing-how-record-purchases.md).
2. Selecteer in het veld **Verzenden naar**, **Klantadres**.
3. Selecteer in het veld **Klant** de klant aan wie u verkoopt.
4. Kies de actie **Doorverzendingen** en kies vervolgens de actie **Verkooporder ophalen**.
5. Selecteer op de pagina **Verkoopoverzicht** de verkooporder die u hebt voorbereid in [Een verkooporder voor doorverzending maken](#to-create-a-sales-order-for-drop-shipment).
6. Kies de knop **OK**.

De regelgegevens van de verkooporder worden ingevoegd op de inkooporderregel(s).

U kunt uw leverancier nu vertellen om de artikelen rechtstreeks naar de klant te verzenden. U kunt ze bijvoorbeeld de order per e-mail sturen.

Als uw leverancier aanvullende informatie verstrekt, zoals een trackingnummer, kunt u die informatie toevoegen als een commentaar op een inkooporderregel. Als u commentaar op een regel wilt toevoegen, kiest u in het veld **Type** **Commentaar** en voert u vervolgens de informatie in het veld **Beschrijving** in.  

## <a name="to-create-multiple-purchase-orders-for-drop-shipments"></a>Meerdere inkooporders voor doorverzendingen maken

U kunt ook het inkoopvoorstel gebruiken om inkooporders te maken. Het voordeel van het gebruik van het inkoopvoorstel is dat het inkooporders kan maken voor alle openstaande doorverzendingen. Dat betekent dat u niet elke order afzonderlijk hoeft te maken.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Inkoopvoorstellen** in en kies vervolgens de gerelateerde koppeling.
2. Kies de actie **Doorverzendingen** en kies vervolgens de actie **Verkooporder ophalen**.
3. Voer indien nodig filtercriteria in voor de orders die u wilt ontvangen en kies vervolgens de knop **OK**.
4. Bekijk de inkooporderregels en selecteer in het veld **Leveranciersnr.** de leverancier die de goederen levert.
5. Kies de actie **Planningsboodschap uitvoeren** om de regels om te zetten in een inkooporder.

## <a name="to-view-the-linked-purchase-order-from-the-sales-order"></a>De gekoppelde inkooporder weergeven op basis van de verkooporder

Selecteer de verkooporderregel van de doorverzending, kies de actie **Order**, kies de actie **Doorverzending** en kies vervolgens de actie **Inkooporder**.

## <a name="to-post-a-drop-shipment"></a>Een doorverzending boeken

Nadat de leverancier de artikelen heeft verzonden, kunt u de verkooporder boeken als verzonden. U kunt de inkooporder ook boeken, maar alleen met de optie **Ontvangen**, totdat de verkooporder is gefactureerd.

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Verkooporders** in en kies vervolgens de gerelateerde koppeling.
2. Open de verkooporder die u hebt gemaakt in [Een verkooporder voor een doorverzending maken](#to-create-a-sales-order-for-drop-shipment).
3. Geef in het veld **Te verzenden aantal** op hoeveel van de orderhoeveelheid moet worden verzonden, de volledige of gedeeltelijke orderhoeveelheid.
4. Kies de actie **Boeken** of **Boeken en verzenden**.
5. Kies vervolgens **de optie Verzenden** om later te factureren of de optie **Verzenden en factureren** om meteen te factureren.

> [!TIP]
> Vergeet niet dat u de inkooporderfactuur moet boeken.

## <a name="see-also"></a>Zie ook

[Speciale orders maken](sales-how-to-create-special-orders.md)  
[Artikelen inkopen voor een verkoop](purchasing-how-purchase-products-sale.md)  
[Producten verkopen](sales-how-sell-products.md)  
[Inkopen vastleggen](purchasing-how-record-purchases.md)  
[Verkoop](sales-manage-sales.md)  
[Voorraad](inventory-manage-inventory.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
