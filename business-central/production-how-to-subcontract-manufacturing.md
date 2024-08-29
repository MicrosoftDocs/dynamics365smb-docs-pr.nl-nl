---
title: Productie uitbesteden
description: 'Dit artikel geeft een uitgebreid overzicht van de uitgebreide functionaliteit van onderaanneming, inclusief werkcentrumvelden en routing.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: '99000886,'
ms.date: 06/22/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---
# <a name="subcontract-manufacturing"></a>Productie uitbesteden

Veel productiebedrijven besteden bepaalde bewerkingen uit aan leveranciers. Uitbesteden kan een eenmalig gebeuren zijn of een integraal onderdeel uitmaken van alle productieprocessen.

[!INCLUDE[prod_short](includes/prod_short.md)] biedt verscheidene hulpmiddelen voor het beheren van uitbesteed werk:  

- Afdelingen met toegewezen leveranciers: met behulp van deze functie kunt u een afdeling instellen die is gekoppeld aan een leverancier (toeleverancier). Dit werkcentrum wordt een onderaannemingswerkcentrum genoemd. U kunt een uitbestedingsafdeling specificeren bij een bewerking in een bewerkingsplan, waarmee u op eenvoudige wijze de uitbestede activiteit kunt verwerken. Daarnaast kunnen de kosten van de bewerking worden toegewezen op het niveau van het bewerkingsplan of van de afdeling.  
- Afdelingskosten gebaseerd op eenheden of tijd: met behulp van deze functie kunt u opgeven of kosten die samenhangen met de afdeling worden gebaseerd op de productietijd of een vaste toeslag per eenheid. Hoewel toeleveranciers gewoonlijk werken met een vaste toeslag per eenheid die in rekening wordt gebracht voor hun diensten, kan de toepassing overweg met beide opties (productietijd en vaste toeslag per eenheid).  
- Uitbestedingsvoorstel: met behulp van deze functie kunt u de productieorders vinden met materiaal dat gereed is om naar een toeleverancier te worden gezonden en automatisch inkooporders opstellen voor uitbestedingsbewerkingen op basis van productieorderbewerkingsplannen. De toepassing boekt vervolgens automatisch de inkoopordertoeslagen naar de productieorder tijdens het boeken van de inkooporder. Alleen productieorders met de status Vrijgegeven zijn toegankelijk en kunnen worden gebruikt vanuit een uitbestedingsvoorstel.  

## <a name="subcontract-work-centers"></a>Werkcentra voor onderaanneming

Uitbestedingsafdelingen worden op dezelfde manier ingesteld as normale afdelingen met aanvullende informatie. Ze worden op dezelfde manier als andere werkcentra aan routes toegewezen.  

### <a name="subcontract-work-center-fields"></a>Onderaannemingswerkcentrumvelden

Dit veld **Toeleveranciersnr.** geeft aan dat de afdeling een uitbestedingsafdeling is. U kunt het nummer invoeren van de toeleverancier die de afdeling levert. Dit veld kan worden gebruikt voor het beheren van werkcentra die niet intern zijn, maar verwerking op contractbasis uitvoeren.  

Als u elk proces uitbesteedt voor een ander tarief bij de leverancier, schakelt u het selectievakje **Specifieke kostprijs** in. Met deze instelling kunt u op elke routingregel een kostprijs instellen en bespaart u tijd doordat u niet elke inkooporder opnieuw hoeft in te voeren. De kosten op de bewerkingsplanregel worden gebruikt bij de verwerking in plaats van de kosten in de kostenvelden van de afdeling. Als u **Specifieke kostprijs** inschakelt, worden kosten voor de leverancier berekend per bewerkingsplanbewerking.  

Als u tegen één tarief per leverancier uitbesteedt, laat u het veld **Specifieke kostprijs** leeg. De kosten worden ingesteld door de velden  **Directe eenheidskosten**,  **Indirecte kosten %** en  **Overheadtarief**  in te vullen.  

### <a name="routings-that-use-subcontract-work-centers"></a>Routes die gebruikmaken van onderaannemingswerkcentra

Uitbestedingsafdelingen kunnen op dezelfde manier als reguliere afdelingen worden gebruikt voor bewerkingen in bewerkingsplannen.  

U kunt een bewerkingsplan instellen dat gebruikmaakt van een externe afdeling als standaard bewerkingsstap. Aan de andere kant kunt u ook het bewerkingsplan voor een bepaalde productieorder wijzigen zodat deze een externe bewerking bevat. Dit kan nodig zijn in noodgevallen, bijvoorbeeld wanneer een server niet goed werkt, of tijdens een tijdelijke periode van grotere vraag, waarbij werk dat u normaal gesproken intern uitvoert, naar een onderaannemer moet worden gestuurd.  

Zie voor meer informatie [Bewerkingsplannen maken](production-how-to-create-routings.md).  

## <a name="calculate-subcontracting-worksheets-and-create-subcontract-purchase-orders"></a>Bereken onderaannemingswerkbladen en maak onderaannemingsinkooporders

Nadat u het onderaannemingswerkblad hebt berekend, wordt het bijbehorende document aangemaakt. In dit geval een inkooporder.  

De pagina **Uitbestedingsvoorstel** werkt als het **Planningsvoorstel** door de benodigde voorziening te berekenen van, in dit geval inkooporders, die u in het voorstel bekijkt en vervolgens met de functie **Planningsboodschap uitvoeren** maakt.  

> [!NOTE]  
> Alleen productieorders met de status **Vrijgegeven** zijn toegankelijk en kunnen worden gebruikt vanuit een uitbestedingsvoorstel.  

### <a name="to-calculate-the-subcontracting-worksheet"></a>Het uitbestedingsvoorstel berekenen

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Uitbestedingsvoorstel** in en kies vervolgens de gerelateerde koppeling.  
2. Als u het voorstel wilt berekenen, klikt u op de actie **Uitbestedingen berekenen**.  
3. Op de pagina  **Ondercontracten berekenen**  kunt u filters instellen voor de uitbestede bewerkingen of de werkcentra waar ze worden uitgevoerd, om alleen de relevante productieorders te berekenen.  
4. Kies de knop **OK**.  

    Bekijk de regels op de pagina **Uitbestedingsvoorstel**. De informatie in dit voorstel is afkomstig van de productieorder en de productieorderbewerkingsplanregels en gaat naar de inkooporder op het moment dat dit document wordt aangemaakt. U kunt een rij uit het voorstel verwijderen zonder dat dit gevolgen heeft voor de oorspronkelijke informatie, net zoals u met andere voorstellen kunt. De informatie verschijnt opnieuw de volgende keer dat u de functie **Uitbestedingen berekenen** uitvoert.  

### <a name="to-create-the-subcontract-purchase-order"></a>De uitbestedingsinkooporder genereren

1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen") voer **Uitbestedingsvoorstel** in en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Planningsboodschap uitvoeren**.  
3. Plaats een vinkje in het veld **Orders afdrukken** om de inkooporder af te drukken wanneer deze wordt gemaakt.  
4. Kies de knop **OK**.  

Als alle uitbestede bewerkingen naar dezelfde leveranciersvestiging worden gestuurd, wordt slechts één inkooporder opgesteld.  

De voorstelregel waarvan een inkooporder is gemaakt, wordt verwijderd uit het voorstel. Nadat een inkooporder is aangemaakt, verschijnt deze niet meer in het werkblad.  

## <a name="posting-subcontract-purchase-orders"></a>Het boeken van onderaannemingsinkooporders

Nadat de inkooporders voor onderaannemers zijn aangemaakt, kunnen ze worden geboekt. Bij ontvangst van de order wordt een capaciteitspost geboekt op de productieorder en bij het factureren van de order worden de directe kosten van de inkooporder geboekt op de productieorder.  

## <a name="to-post-a-subcontract-purchase-order"></a>Een uitbestedingsinkooporder boeken
 
1. Kies het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Inkooporders** in en selecteer vervolgens de gerelateerde koppeling  
2. Open een inkooporder die op basis van het uitbestedingsvoorstel is gemaakt.  

    Op de inkooporderregels kunt u dezelfde gegevens zien als die in het voorstel stonden. De velden **Prod.-ordernr.**, **Prod.-orderregelnr.**, **Bewerkingsnr.** en **Afdelingsnr.** worden ingevuld met de informatie van de bronproductieorder.  

3. Kies de actie **Boeken**.  

Wanneer de inkoop als ontvangen wordt geboekt, wordt er automatisch een uitvoerjournaalpost geboekt voor de productieorder als de uitbestedingsbewerking de laatste bewerking is in de productieorderroute.  

> [!CAUTION]  
> De output automatisch boeken voor een voortdurende productieorder wanneer uitbestede artikelen worden ontvangen, is mogelijk niet wenselijk. De redenen voor dit zouden kunnen zijn dat het verwachte outputaantal dat wordt geboekt verschilt van het werkelijke aantal en dat de boekdatum van de automatische output misleidend is.  
>
> Om te voorkomen dat de verwachte uitvoer van een productieorder wordt geboekt wanneer de uitbestedingsinkopen worden ontvangen, moet u ervoor zorgen dat de uitbestede bewerking niet de laatste is. Of voeg een nieuwe laatste bewerking voor het laatste outputaantal in.  

Wanneer de inkooporder wordt geboekt als gefactureerd, worden de directe kosten van de inkooporder naar de productieorder geboekt.  

> [!NOTE]  
> Verwachte kosten worden alleen beheerd voor artikeltransacties. Verwachte kosten gelden niet voor immateriële transactietypen, zoals capaciteit die is geboekt via inkooporders voor onderaanneming. Raak niet in de war door het feit dat het posten van een ontvangstbewijs kan leiden tot trigger posten van de uitvoer. Deze transacties zijn gescheiden en de verwachte kosten van de output worden onafhankelijk berekend.  

## <a name="see-also"></a>Zie ook

[Productie](production-manage-manufacturing.md)    
[Productie instellen](production-configure-production-processes.md)  
[Gepland](production-planning.md)      
[Voorraad](inventory-manage-inventory.md)  
[Inkoop](purchasing-manage-purchasing.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]
