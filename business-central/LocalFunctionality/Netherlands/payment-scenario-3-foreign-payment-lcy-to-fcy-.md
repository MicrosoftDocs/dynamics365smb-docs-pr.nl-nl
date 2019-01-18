---
title: Betalingsscenario 3 - een buitenlandse betaling (LV naar VV)
description: U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 10/01/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: 33b900f1ac9e295921e7f3d6ea72cc93939d8a1b
ms.openlocfilehash: e3bca57217ba5ca28a0cd04e9483c312e7ae70d5
ms.contentlocale: nl-nl
ms.lasthandoff: 11/26/2018

---
# <a name="payment-scenario-3---foreign-payment-lcy--to-fcy"></a>Betalingsscenario 3 - een buitenlandse betaling (LV naar VV)
U kunt telebankieren gebruiken voor handel met binnenlandse en buitenlandse klanten en leveranciers. Dit onderwerp beschrijft een scenario waarin de handel met buitenlandse klanten en leveranciers geschiedt die een andere valuta dan uw lokale valuta gebruiken.  

1.  Leverancier/klant maken.  
2.  Bankrekening leverancier/klant maken.  
3.  Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken.  
4.  Voorstel maken.  
5.  Betaalrun maken.  
6.  Betaalrun exporteren.  
7.  Bankafschrift importeren.  

> [!NOTE]  
>  In de volgende voorbeelden zijn enkele standaard-CRONUS-gegevens gebruikt. En in plaats van een leverancier/klant en een Bankrekening leverancier/klant te maken, zou u ook bestaande gegevens kunnen gebruiken.  

## <a name="create-vendorcustomer"></a>Leverancier/klant maken  
 Maak een leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in vreemde valuta voor uw lokale bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

> [!NOTE]  
>  U kunt alleen een bankrekening in het veld **Bankrekening** invullen als er Bankrekeningen leverancier/klant beschikbaar zijn. Zie hieronder.  

### <a name="example"></a>Voorbeeld  
Hernandez Ortiz (code **ORTIZ**) is een van onze Mexicaanse leveranciers. Inkoopfacturen worden door middel van onze nationale bankrekening (code **ABN**) aan zijn bankrekening (code **HOBA**) betaald. Terwijl onze bankrekening ABN in lokale valuta (LV) wordt uitgedrukt, wordt de bankrekening van Hernandez Ortiz, HOBA, in Mexicaanse peso's (MXN) uitgedrukt. Daarom stellen we op de leverancierskaart van Hernandez Ortiz het veld **Valutacode** in op **MXN**, vullen we in het veld **Transactiewijze** **ABN** in, wat aan onze bankrekening, ABN, is gekoppeld en stellen we het veld **Bankrekening** in op **HOBA**.  

## <a name="create-vendorcustomer-bank-account"></a>Bankrekening leverancier/klant maken  
Maak een bankrekening leverancier/klant en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Bankrekening van voorkeur**: voer een geldig bankrekeningnummer in.  
- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Rekeninghouder**: zorg ervoor dat alle gegevens zijn ingevuld.  

### <a name="example"></a>Opmerking  
De bankrekening van Hernandez Ortiz (code **HOBA**) wordt uitgedrukt in **MXN**. Daarom vullen we op de bankrekeningkaart van leverancier Hernandez Ortiz een geldig nummer in het veld **Bankrekeningnr.** in, stellen we het veld **Valutacode** in op **MXN** en vullen we in de velden op het sneltabblad **Rekeninghouder** de juiste waarden in.  

## <a name="create-and-post-purchase-invoice-for-vendor-or-sales-invoice-for-customer"></a>Inkoopfactuur voor leverancier of verkoopfactuur voor klant maken en boeken  
Maak een inkoop-/verkoopfactuur en vul alle noodzakelijke gegevens in. Besteed extra aandacht aan de volgende velden:  

- **Valutacode**: stel in dit veld de vreemde valuta (VV) in.  
- **Transactiewijze**: selecteer een geschikte standaardtransactiewijze, dat wil zeggen, een transactiewijze die geschikt is voor betalingen in lokale valuta voor uw lokale bank.  
- **Bankrekening van voorkeur**: selecteer een geschikte standaardbankrekening van leveranciers/klanten met dezelfde valutacode als de leverancier/klant zelf.  

Standaard zijn in deze drie velden waarden ingevuld die zijn overgenomen uit de leveranciers-/klantenkaart.  

Als de factuur is voltooid, kan deze worden geboekt.  

### <a name="example"></a>Voorbeeld  
Als we een inkoopfactuur voor Hernandez Ortiz maken, vullen we **ORTIZ** in het veld **Orderleveranciersnr.** in. Standaard zijn in de velden **Valutacode**, **Transactiewijze** en **Bankrekening** waarden overgenomen vanuit de leverancierskaart van Hernandez Ortiz. Daarom is in de velden **Valutacode**, **Transactiewijze** en **Bankrekening** respectievelijk **MXN**, **ABN** en **HOBA** ingevuld. Deze waarden kunnen echter worden gewijzigd.  

## <a name="create-proposal"></a>Voorstel maken  
Open de pagina **Telebank - bankoverzicht** en blader naar de bank die we voor onze betaling willen gebruiken. Open de pagina **Voorstel** en genereer betalingsvoorstellen met de batchverwerking **Voorstelposten ophalen**.  

### <a name="example"></a>Opmerking  
Door middel van de pagina **Telebank - bankoverzicht** openen we de pagina **Voorstel** voor onze bank, ABN. Met de batchverwerking wordt één voorstelregel gemaakt voor de inkoopfactuur die we zojuist voor de leverancier ORTIZ hebben gemaakt en geboekt. Het bedrag van de betaling wordt uitgedrukt in lokale valuta (LV).  

## <a name="create-payment-history"></a>Betaalrun maken  
Vanuit de pagina **Voorstel** verwerken we ons voorstel in een betaalrun. Het voorstel verdwijnt en kan worden gevonden op de pagina **Betaalrunoverzicht** voor dezelfde bank.  

### <a name="example"></a>Opmerking  
We verwerken ons voorstel met betrekking tot de betaling aan leverancier ORTIZ en openen de pagina **Betaalrunoverzicht** voor onze bank ABN. De laatste betaalrun is de betaalrun die we zojuist hebben gemaakt.  

## <a name="export-payment-history"></a>Betaalrun exporteren  
Open de pagina **Betaalrunoverzicht**, blader naar de relevante betaalrun en kies vervolgens de actie **Exporteren**. De exportbatchverwerking voor het exportprotocol dat aan deze betaling is gekoppeld, verschijnt. Voor deze export zijn de juiste filters al automatisch ingevuld. Controleer desgewenst velden van het sneltabblad **Opties** en kies vervolgens de knop **OK** om de betaling te exporteren. Er wordt een tekstbestand gegenereerd met een bestandsnaam zoals die is gedefinieerd in het veld **Standaardbestandsnamen** van het exportprotocol, dat nu gereed is voor verzending naar onze bank.  

### <a name="example"></a>Opmerking  
Aangezien de transactiewijze die aan onze betaling is gekoppeld *ABN** is, verschijnt de batchverwerking **BBV** of **PAYMUL**.  

## <a name="import-bank-statement"></a>Bankafschrift importeren  
Nadat we elektronische bankafschriften van onze bank hebben ontvangen, kunnen we ze importeren door vanuit de pagina **Importprotocoloverzicht** het betreffende importprotocol uit te voeren.  

### <a name="example"></a>Opmerking  
Het bankafschrift met onze betaling aan Hernandez Ortiz wordt door onze bank, ABN, naar ons gestuurd. Daarom moeten we **OFFICE NET EXTRA** als het juiste importprotocol kiezen.  

## <a name="see-also"></a>Zie ook  
 [Voorstellen maken.](how-to-create-proposals.md)   
 [Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)

