---
title: 'Scenario 2 - buitenlandse betaling (VV naar VV) [NL]'
description: In dit artikel wordt een scenario 2 beschreven waarin u telebankieren kunt gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 12/08/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# Betalingsscenario 2 - Buitenlandse betaling (VV naar VV) in de Nederlandse versie
U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit artikel beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die dezelfde vreemde valuta gebruiken als waarvoor uw bankrekening is ingesteld.  

De volgende lijst bevat de belangrijkste stappen:  

1.  Leverancier/klant maken.  
2.  Bankrekening leverancier/klant maken.  
3.  Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.  
4.  Voorstel maken.  
5.  Betaalrun maken.  
6.  Betaalrun exporteren.  
7.  Bankafschrift importeren.  

> [!NOTE]  
>  In de volgende voorbeelden zijn enkele standaard CRONUS-gegevens gebruikt. En in plaats van een leverancier/klant en een bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.  

## Leverancier/klant maken  
 Maak een leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

> [!NOTE]  
>  U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn. Zie hieronder.  

### Voorbeeld  
Jannet Carter (code **JANNET**) is een van onze Amerikaanse leveranciers. Inkoopfacturen worden door middel van onze buitenlandse bankrekening (code **ABN-USD**) aan hun bankrekening (code **JCBA**) betaald. Zowel bankrekening ABN-USD als bankrekening JCBA worden uitgedrukt in dezelfde vreemde valuta (VV), in dit geval Amerikaanse dollars (USD). Daarom stellen we op de leverancierskaart van Jannet Carter het veld **Valutacode** in op **USD**, vullen we in het veld **Transactiewijze** **ABN-USD** in, wat aan onze bankrekening ABN-USD is gekoppeld en stellen we het veld **Bankrekening** in op **JCBA**.  

## Bankrekening leverancier/klant maken  
Maak een Bankrekening leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.  
- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.  

### Opmerking  
De bankrekening van Jannet Carter (code **JCBA**) wordt uitgedrukt in vreemde valuta (VV), in dit geval USD. Daarom vullen we op de bankrekeningkaart van leverancier Jannet Carter een geldig nummer in het veld **Bankrekeningnr.** in, stellen we het veld **Valutacode** in op **USD** en vullen we in de velden op het tabblad **Rekeninghouder** de juiste waarden in.  

## Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken  
Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw buitenlandse bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

Standaard worden in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.  

Als de factuur is voltooid, kan deze worden geboekt.  

### Opmerking  
Als we een inkoopfactuur voor Jannet Carter maken, vullen we **JANNET** in het veld **Orderleveranciersnr.** in. Standaard worden in de velden **Valutacode**, **Transactiewijze** en **Bankrekening** waarden overgenomen vanuit de leverancierskaart van Jannet Carter. Daarom wordt in de velden **Valutacode**, **Transactiewijze** en **Bankrekening** respectievelijk **USD**, **ABN-USD** en **JCBA** ingevuld. Deze waarden kunnen echter worden gewijzigd.  

## Voorstel maken  
Open de pagina **Telebank - bankoverzicht** en blader naar de bank die we voor onze betaling willen gebruiken. Open de pagina **Voorstel** en genereer betalingsvoorstellen met de batchverwerking **Voorstelposten ophalen**.  

### Opmerking  
Door middel van de pagina **Telebank - bankoverzicht** openen we de pagina **Voorstel** voor onze bank, ABN-USD. Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier JANNET hebben gemaakt en geboekt.  

## Betalingsgeschiedenis maken  
Vanuit de pagina **Voorstel** verwerken we ons voorstel in een betaalrun. Het voorstel verdwijnt en kan worden gevonden op de pagina **Betaalrunoverzicht** voor dezelfde bank.  

### Opmerking  
We verwerken ons voorstel met betrekking tot de betaling aan de leverancier JANNET en openen de pagina **Betaalrunoverzicht** voor onze bank, ABN-USD. De laatste betalingsgeschiedenis is de betalingsgeschiedenis die we zojuist hebben gemaakt.  

## Betalingsgeschiedenis exporteren  
Open de pagina **Betaalrunoverzicht**, blader naar de relevante betaalrun en kies de actie **Exporteren**. De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt. Voor deze export zijn de juiste filters al automatisch ingevuld. Controleer desgewenst velden van het sneltabblad **Opties** en kies vervolgens de knop **OK** om de betaling te exporteren. Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld **Standaardbestandsnamen** van het exportprotocol, dat nu gereed is voor verzending naar onze bank.  

### Voorbeeld  
Aangezien de transactiewijze die aan onze betaling is gekoppeld ABN-USD is, verschijnt de batchverwerking **BBV** of **PAYMUL**.  

## Bankafschrift importeren  
Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit de pagina **Importprotocoloverzicht** het betreffende importprotocol uit te voeren.  

### Opmerking  
Onze bank stuurt ons het bankafschrift met onze betaling aan Jannet Carter, ABN-USD. Daarom kiezen we **OFFICE NET EXTRA** als het juiste importprotocol.  

## Zie ook  
 [Voorstellen maken.](how-to-create-proposals.md)   
 [Betalingshistorie maken en exporteren](how-to-create-and-export-payment-history.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
