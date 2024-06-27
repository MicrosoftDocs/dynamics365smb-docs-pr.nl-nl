---
title: 'Elektronische btw- en ICP-aangiften verzenden [NL]'
description: Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 12/12/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---
# Elektronische btw- en ICP-aangiften verzenden in de Nederlandse versie
Bedrijven moeten maandelijks periodieke btw-aangiften en ICP-aangiften (intracommunautaire leveringen) naar de belastingdienst versturen.  

Btw aangiften moeten op een maandelijkse of driemaandelijkse basis worden verzonden.
ICP-aangiften moeten op een driemaandelijkse basis worden verzonden.

> [!NOTE]  
> ICP-aangiften moeten worden verzonden door bedrijven/regio's die goederen of diensten verkopen aan landen/regio's binnen de Europese Unie. Inkopen zijn niet opgenomen in deze aangifte. <br /><br />
Een transactie komt alleen in aanmerking voor ICP-aangifte als de handelswaar de grens fysiek heeft overschreden. Het is niet voldoende dat de locatie van een factuuradres of het kantoor van de leverancier of klant in een ander land of een andere regio in een EU-land/regio ligt.  

U kunt de btw-aangiften en ICP-aangiften als volgt verzenden:  

- Meld u aan op de website van het Nederlandse belastingkantoor en voer de informatie handmatig in. Zie voor meer informatie de [website](https://go.microsoft.com/fwlink/?linkid=223151) van de Nederlandse belastingdienst.  

- Maak een elektronische aangifte en verzend het versleutelde bestand via het Digipoort-kanaal naar het Nederlandse belastingkantoor. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden. Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes. De rapporten hebben de XBRL-indeling (eXtensible Business Reporting Language). Zie [Rapporten maken met XBRL](../../bi-create-reports-with-xbrl.md) voor meer informatie.

## Elektronische aangifte voorbereiden
Voordat u elektronische aangiften kunt versturen naar de belastingdienst moeten eerst de volgende taken zijn uitgevoerd:

1. Controleer of u de certificaten van de overheid ontvangt. Als dat niet zo is, voert u de volgende stappen uit om de certificaten te krijgen:

    - Verkrijg een PKIoverheid-certificaat voor het bedrijf als u er nog geen hebt. Een lijst met certificaatproviders vindt u hier: [https://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps](https://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps).  

    - Registreer een gebruiker van Digipoort, wat u hier kunt doen: [https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl).

    - Verkrijg een **Digipoort Service-certificaat**, dat kan worden verkregen van de website van de Nederlandse belastingdienst: [https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl).

2. Algemene en persoonlijke gegevens, ontvangen van de belastingdienst, op de pagina **Elek. aangifte-instellingen** invoeren. Zie voor meer informatie [Elektronische btw- en ICP-aangiftes instellen](how-to-set-up-electronic-vat-and-icp-declarations.md).

3. Stel een btw-categoriecode in voor alle XML-elementen in de elektronische btw-aangifte. Zie [Btw-categorieën instellen](how-to-set-up-vat-categories.md) voor meer informatie.

## Een elektronische aangifte aanmaken
1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies op de pagina **Overzicht elektronische aangiften** de actie **Nieuw**.  
3. Vul op de pagina **Elektronische aangifte** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
4. Kies de knop **OK**.

De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** op de pagina **Elektronische aangiftekaart**.

De XBRL Reporter zorgt ervoor dat alle rekeningnummers die worden geïmporteerd van Business Central, aan de XBRL-elementen in een rapport worden toegewezen. De XBRL Reporter geeft ook een lijst weer met fouten wegens niet-toegewezen elementen of rekeningen.

## Een elektronische aangifte versturen
Met de XBRL Reporter kunt u de aangifte van intracommunautaire leveringen (ICP) of de btw-aangifte verzenden in de vereiste XML-indeling. Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd op de pagina **Elek. aangifte-instellingen**.

1. Kies op de pagina **Elektronische aangiftekaart** de actie **Elektronische aangifte versturen**.
2. Vul de velden in zoals beschreven in de volgende tabel.

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Clientcertificaat**|Selecteer het certificaat **PKIoverheid** voor het bedrijf.|  
    |**Wachtwoord van clientcertificaat**|Voer het wachtwoord in dat wordt gebruikt om het clientcertificaat te versleutelen.|
    |**Servicecertificaat**|Selecteer het certificaat **Digipoortservice**.|

3. Kies de knop **OK**.  

De elektronische aangifte wordt verstuurd naar de belastingdienst.

> [!NOTE]  
> Als er geen intracommunautaire leveringen zijn geweest in de aangifteperiode, dan wordt er een elektronische ICP-aangifte aangemaakt zonder XML-elementen voor de leveringen. Als u een dergelijke aangifte verzendt, wordt een foutbericht weergegeven.

## Een responsbericht van de belastingdienst importeren
De belastingdienst zal voor elke ontvangen aangifte een responsbericht sturen. Deze responsberichten moeten worden opgehaald van de server van de belastingdienst en worden verwerkt. De eerste stap omvat het importeren van het responsbericht in [!INCLUDE[prod_short](../../includes/prod_short.md)].

1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Responsberichten elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Responsberichten ontvangen**.  
3. Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Clientcertificaat**|Selecteer het certificaat **PKIoverheid** voor het bedrijf.|  
    |**Wachtwoord van clientcertificaat**|Voer het wachtwoord in dat wordt gebruikt om het clientcertificaat te versleutelen.|
    |**Servicecertificaat**|Selecteer het certificaat **Digipoortservice**.|  

4. Kies de knop **OK**.

## Een responsbericht van de belastingdienst verwerken
Wanneer een responsbericht is geïmporteerd, moet het worden verwerkt door de inhoud te valideren aan de hand van de gerelateerde elektronische aangifte. Als er geen fouten worden gevonden in de elektronische aangifte en de gegevens zijn verwerkt door de belastingdienst, wordt het veld **Status** op de pagina **Elektronische aangiftekaart** gewijzigd in **Geaccepteerd**.

1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Responsberichten elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Responsberichten verwerken**.  
3. Selecteer de juiste filters op de pagina **Batchverwerking Responsberichten verwerken** en klik vervolgens op de knop **OK**.  

    De verwerkte gegevens over het responsbericht wordt weergegeven op de **Responsberichten elektronische aangiften** pagina.  

4. Als u een bericht of bijlage wilt exporteren, kiest u op het tabblad **Responsbericht exporteren** de actie **Responsbijlage exporteren**.

## Zie ook  
[Elektronische btw- en ICP-aangiften instellen](how-to-set-up-electronic-vat-and-icp-declarations.md)  
[Btw-categorieën instellen](how-to-set-up-vat-categories.md)  
[Lijsten met XBRL maken](../../bi-create-reports-with-xbrl.md)  
[Nederlandse lokale functionaliteit](netherlands-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
