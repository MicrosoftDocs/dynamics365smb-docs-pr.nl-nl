---
title: Productie-output wegzetten
description: In dit artikel wordt beschreven hoe u uw productieoutput kunt opslaan.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.date: 08/12/2024
ms.custom: bap-template
ms.search.forms: '9326, 99000831, 9315, 7375'
---
# Productie- of assemblage-output wegzetten

Hoe u de productieoutput opslaat, is afhankelijk van de vestigingsinstellingen van het magazijn. Zie voor meer informatie [Magazijnbeheer instellen](warehouse-setup-warehouse.md).  

Activeer in een basismagazijnconfiguratie voor de inkomende stroom (put-away) op de pagina  **Locatie kaart**  voor de locatie de volgende instellingen:

* Voor productie selecteert u in het veld  **Prod. Output Whse. Handling** de optie  **Inventory Put-away**.
* Assemblageprocessen ondersteunen geen voorraadopslag. U boekt een assemblageorder om output te registreren. Als u opslaglocaties gebruikt, kunt u artikelen later tussen de opslaglocaties verplaatsen. Zie voor meer informatie [Artikelen ad hoc verplaatsen in basismagazijnconfiguraties](warehouse-how-to-move-items-ad-hoc-in-basic-warehousing.md).  
* Voor projecten is wegzetten niet van toepassing.

In geavanceerde magazijnconfiguraties waar een locatie moet worden weggezet, maakt u een intern wegzetdocument of een verplaatsingsdocument om de output weg te zetten.  

## Productieoutput opslaan met een voorraadopslag

De eerste stap bij het opslaan van output is het maken van het inkomende magazijnverzoek. Deze aanvraag informeert het magazijn dat de output van de productie- of assemblageorder gereed is voor opslag.

### Ink.magazijnontvangst maken  

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Vrijgegeven productieorder** in en kies vervolgens de gerelateerde koppeling.  
2. Kies in de productieorder die gereed is voor opslag en kies dan de actie **Ink. magazijnontvangst maken**.  

> [!NOTE]  
> U kunt de inkomende magazijnaanvraag ook maken door het veld **Inkomend verzoek maken** te kiezen bij het vernieuwen van de productieorder. Zie voor meer informatie [Productieorders vernieuwen of opnieuw plannen](production-how-to-replan-refresh-production-orders.md).  

### Om output weg te zetten met een voorraadopslag  

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Voorraadopslag** in en kies vervolgens de gerelateerde koppeling.  
2. Een nieuwe voorraadopslag maken. Zie voor meer informatie [Artikelen opslaan met voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md).
3. Kies de actie **Brondocumenten ophalen** en selecteer de vrijgegeven productieorder om de productieorderoutput te openen.  
4. Vul waar nodig de opslagregels in.
5. Wanneer de regels gereed zijn voor boeken, kiest u de actie **Boeken**. Met Boeking worden de magazijnposten aangemaakt en de uitvoer van de artikelen geboekt.  

    [!INCLUDE [preview-posting-warehouse](includes/preview-posting-warehouse.md)]

Het is ook mogelijk om rechtstreeks vanuit een vrijgegeven productieorder een **Voorraadopslag** te maken. Zie voor meer informatie [Artikelen opslaan met voorraadopslag](warehouse-how-to-put-items-away-with-inventory-put-aways.md).  

Wanneer u een voorraadopslag boekt, wordt ervan uitgegaan dat alle bewerkingen worden geboekt volgens de standaardroutering. [!INCLUDE [prod_short](includes/prod_short.md)]  Dat wil zeggen, het outputaantal wordt geboekt op basis van de laatste bewerking. U kunt het outputdagboek gebruiken om verschillen in het outputaantal en de instel- en bewerkingstijd te boeken. Als u een gedeelte moet boeken nadat u de voorraad hebt weggezet, kunt u dit doen op basis van de insteltijden en hoeveelheden voor alle bewerkingen, behalve de laatste. Het wegzetten van de inventaris bepaalt de laatste bewerking.  

Als u alleen de instel- of uitvoeringstijd van de laatste bewerking wilt boeken, stelt u de uitvoerhoeveelheid van de laatste bewerking in op 0. U kunt ervoor kiezen om de laatste regel helemaal niet te plaatsen door deze te verwijderen.

## Om assemblage- en productie-output in geavanceerde magazijnconfiguraties op te slaan

Wanneer u de output van een productie- of assemblageorder boekt in een magazijn dat gebruikmaakt van gestuurde opslag en pick, gaat de output naar de opslaglocatie die is gedefinieerd in de productie- of assemblageorder. Ga naar  [Artikelen verplaatsen in geavanceerde magazijnconfiguraties voor meer informatie over verschillende manieren om artikelen in het magazijn te verplaatsen met geavanceerde configuraties](warehouse-how-to-move-items-in-advanced-warehousing.md#to-move-items-with-the-warehouse-movement-worksheet).

> [!NOTE]  
> In geen van beide procedures (assembly- of productieoutput) kunt u het brondocumentnummer, zoals het productieordernummer invoeren in de documenten voor interne opslag, opslag of verplaatsing.  

## Zie ook  

[Overzicht van magazijnbeheer](design-details-warehouse-management.md)
[Voorraad](inventory-manage-inventory.md)  
[Magazijnbeheer instellen](warehouse-setup-warehouse.md)  
[Assemblagebeheer](assembly-assemble-items.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)

[!INCLUDE[footer-include](includes/footer-banner.md)]
