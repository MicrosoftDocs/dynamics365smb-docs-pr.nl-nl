---
title: Betalingsscenario 1 - binnenlandse betalingen (LV naar LV).
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.
documentationcenter: ''
author: SorenGP
services: project-madeira
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2020
ms.author: edupont
ms.openlocfilehash: 6caef5f8fed18a15b85481c0a24c00ae7b3183a6
ms.sourcegitcommit: ff2b55b7e790447e0c1fcd5c2ec7f7610338ebaa
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2021
ms.locfileid: "5382825"
---
# <a name="payment-scenario-1---domestic-payments-lcy-to-lcy"></a>Betalingsscenario 1 - binnenlandse betalingen (LV naar LV).
U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel geschiedt met binnenlandse klanten en leveranciers.  

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

## <a name="create-vendorcustomer"></a>Leverancier/klant maken  
Maak een leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: laat dit veld leeg; het wordt ingesteld op de lokale valuta (LV).  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

> [!NOTE]  
>  U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn. Zie hieronder.  

### <a name="example"></a>Voorbeeld  
Olek Johansson (code **OLEK**) is een van uw lokale leveranciers. Inkoopfacturen worden door middel van onze nationale bankrekening (code **ABN**) aan zijn bankrekening (code **OJBA**) betaald. Zowel bankrekening ABN als bankrekening OJBA worden uitgedrukt in lokale valuta (LV). Daarom laten we op de leverancierskaart van Olek Johansson het veld **Valutacode** leeg, vullen we in het veld **Transactiewijze** **ABN** in, wat is gekoppeld aan onze bankrekening, ABN, en stellen we het veld **Bankrekening** in op **OJBA**.  

## <a name="create-vendorcustomer-bank-account"></a>Bankrekening leverancier/klant maken  
Maak een Bankrekening leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.  
- **Valutacode**: laat dit veld leeg; het wordt ingesteld op de lokale valuta (LV).  
- **Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.  

### <a name="example"></a>Opmerking  
De bankrekening van Olek Johansson (code **OJBA**) wordt uitgedrukt in lokale valuta (LV). Daarom vullen we op de bankrekeningkaart van leverancier Olek Johansson een geldig nummer in het veld **Bankrekeningnr.** in, laten we het veld **Valutacode** leeg en vullen we in de velden op het sneltabblad **Rekeninghouder** de juiste waarden in.  

## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a>Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken  
Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: laat dit veld leeg; het wordt ingesteld op de lokale valuta (LV).  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.  

Als de factuur is voltooid, kan deze worden geboekt.  

### <a name="example"></a>Voorbeeld  
Als we een inkoopfactuur voor Olek Johansson maken, vullen we **OLEK** in het veld **Orderleveranciersnr.** in. Standaard zijn in de velden **Valutacode**, **Transactiewijze** en **Bankrekening** waarden ingevuld die zijn overgenomen uit de leverancierskaart van Olek Johansson. Daarom zijn de velden **Valutacode**, **Transactiewijze** en **Bankrekening** respectievelijk **<empty>**, **ABN** en **OJBA**. Deze waarden kunnen echter worden gewijzigd.  

## <a name="create-proposal"></a>Voorstel maken  
Open de pagina **Telebank - bankoverzicht** en blader naar de bank die we voor onze betaling willen gebruiken. Open de pagina **Voorstel** en genereer betalingsvoorstellen met de batchverwerking **Voorstelposten ophalen**.  

### <a name="example"></a>Opmerking  
Door middel van de pagina **Telebank - bankoverzicht** openen we de pagina **Voorstel** voor onze bank, ABN. Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor leverancier OLEK hebben gemaakt en geboekt.  

## <a name="create-payment-history"></a>Betaalrun maken  
Vanuit de pagina **Voorstel** verwerken we ons voorstel in een betaalrun. Het voorstel verdwijnt en kan worden gevonden op de pagina **Betaalrunoverzicht** voor dezelfde bank.  

### <a name="example"></a>Opmerking  
We verwerken ons voorstel met betrekking tot de betaling aan leverancier OLEK en openen de pagina **Betaalrunoverzicht** voor onze bank, ABN. De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.  

## <a name="export-payment-history"></a>Betaalrun exporteren  
Open de pagina **Betaalrunoverzicht**, blader naar de relevante betaalrun en kies de actie **Exporteren**. De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt. Voor deze export zijn de juiste filters al automatisch ingevuld. Controleer desgewenst velden van het sneltabblad **Opties** en kies vervolgens de actie **OK** om de betaling te exporteren. Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld **Standaardbestandsnamen** van het exportprotocol, dat nu gereed is voor verzending naar onze bank.  

## <a name="import-bank-statement"></a>Bankafschrift importeren  
Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit de pagina **Importprotocoloverzicht** het betreffende importprotocol uit te voeren.  

### <a name="example"></a>Opmerking  
Het bankafschrift met onze betaling aan Olek Johansson wordt door onze bank ABN naar ons gestuurd. Daarom moeten we **OFFICE NET EXTRA** als het juiste importprotocol kiezen.  

## <a name="see-also"></a>Zie ook  
 [Voorstellen maken.](how-to-create-proposals.md)   
 [Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]