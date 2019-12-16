---
title: Elektronische btw- en ICP-aangiften verzenden
description: Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden. Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd op de pagina Elek. aangifte-instellingen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 25d78a832ceb9ca0c253caad9282b96f483b4bbb
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881360"
---
# <a name="submitting-electronic-vat-and-icp-declarations"></a>Elektronische btw- en ICP-aangiften verzenden
Bedrijven moeten maandelijks periodieke btw-aangiften en ICP-aangiften (intracommunautaire leveringen) naar de belastingdienst versturen.  

Btw aangiften moeten op een maandelijkse of driemaandelijkse basis worden verzonden.
ICP-aangiften moeten op een driemaandelijkse basis worden verzonden.

> [!NOTE]  
> ICP-aangiften moeten worden verzonden door bedrijven die goederen of diensten verkopen aan landen binnen de Europese Unie. Inkopen zijn niet opgenomen in deze aangifte. <br /><br />
Een transactie komt alleen in aanmerking voor ICP-aangifte als de handelswaar de grens fysiek heeft overschreden. Het is niet voldoende dat de locatie van een factuuradres of het kantoor van de leverancier of klant in een ander land of een andere regio in een EU-land ligt.  

U kunt de btw-aangiften en ICP-aangiften als volgt verzenden:  

- Meld u aan op de website van het Nederlandse belastingkantoor en voer de informatie handmatig in. Zie voor meer informatie de [website](https://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  

- Maak een elektronische aangifte en verzend het versleutelde bestand via het Digipoort-kanaal naar het Nederlandse belastingkantoor. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden. Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes. De rapporten hebben de XBRL-indeling (eXtensible Business Reporting Language). Zie [Rapporten maken met XBRL](../../bi-create-reports-with-xbrl.md) voor meer informatie.

## <a name="to-prepare-for-electronic-declaration"></a>Elektronische aangifte voorbereiden
Voordat je elektronische aangiften kan versturen naar de belastingdienst moeten eerst de volgende taken zijn uitgevoerd:

1. Controleer of u de certificaten van de overheid hebt ontvangen. Als dat niet zo is, voert u de volgende stappen uit om de certificaten te krijgen:

    - Verkrijg een PKIoverheid-certificaat voor het bedrijf als u er nog geen hebt. Een lijst met certificaatproviders vindt u hier: [https://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps](https://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps).  

    - Registreer een gebruiker van Digipoort, wat u hier kunt doen: [https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw](https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw).

    - Verkrijg een **Digipoort Service-certificaat**, dat kan worden verkregen van de website van de Nederlandse belastingdienst: [https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl).

2. Algemene en persoonlijke gegevens, ontvangen van de belastingdienst, op de pagina **Elek. aangifte-instellingen** invoeren. Zie voor meer informatie [Elektronische btw- en ICP-aangiftes instellen](how-to-set-up-electronic-vat-and-icp-declarations.md).

3. Stel een btw-categoriecode in voor alle XML-elementen in de elektronische btw-aangifte. Zie [Btw-categorieën instellen](how-to-set-up-vat-categories.md) voor meer informatie.

## <a name="to-create-an-electronic-declaration"></a>Een elektronische aangifte aanmaken
1. Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies op de pagina **Overzicht elektronische aangiften** de actie **Nieuw**.  
3. Vul op de pagina **Elektronische aangifte** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]  
4. Kies de knop **OK**.

De XML-elementen met de bijbehorende gegevens van de elektronische aangifte worden weergegeven op het sneltabblad **Regels** op de pagina **Elektronische aangiftekaart**.

De XBRL Reporter zorgt ervoor dat alle rekeningnummers die worden geïmporteerd van Business Central, aan de XBRL-elementen in een rapport worden toegewezen. De XBRL Reporter geeft ook een lijst weer met fouten wegens niet-toegewezen elementen of rekeningen.

## <a name="to-submit-an-electronic-declaration"></a>Een elektronische aangifte versturen
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

## <a name="to-import-a-response-message-from-the-tax-authorities"></a>Een responsbericht van de belastingdienst importeren
De belastingdienst zal voor elke ontvangen aangifte een responsbericht sturen. Deze responsberichten moeten worden opgehaald van de server van de belastingdienst en worden verwerkt. De eerste stap omvat het importeren van het responsbericht in [!INCLUDE[d365fin](../../includes/d365fin_md.md)].

1. Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Responsberichten elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Responsberichten ontvangen**.  
3. Vul op het sneltabblad **Opties** de velden in, zoals in de volgende tabel is beschreven.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**Clientcertificaat**|Selecteer het certificaat **PKIoverheid** voor het bedrijf.|  
    |**Wachtwoord van clientcertificaat**|Voer het wachtwoord in dat wordt gebruikt om het clientcertificaat te versleutelen.|
    |**Servicecertificaat**|Selecteer het certificaat **Digipoortservice**.|  

4. Kies de knop **OK**.

## <a name="to-process-a-response-message-from-the-tax-authorities"></a>Een responsbericht van de belastingdienst verwerken
Wanneer een responsbericht is geïmporteerd, moet het worden verwerkt door de inhoud te valideren aan de hand van de gerelateerde elektronische aangifte. Als er geen fouten worden gevonden in de elektronische aangifte en de gegevens zijn verwerkt door de belastingdienst, wordt het veld **Status** op de pagina **Elektronische aangiftekaart** gewijzigd in **Geaccepteerd**.

1. Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Responsberichten elektronische aangiften** in en kies vervolgens de gerelateerde koppeling.  
2. Kies de actie **Responsberichten verwerken**.  
3. Selecteer de juiste filters op de pagina **Batchverwerking Responsberichten verwerken** en klik vervolgens op de knop **OK**.  

    De verwerkte gegevens over het responsbericht wordt weergegeven op de **Responsberichten elektronische aangiften** pagina.  

4. Als u een bericht of bijlage wilt exporteren, kiest u op het tabblad **Responsbericht exporteren** de actie **Responsbijlage exporteren**.

## <a name="see-also"></a>Zie ook  
[Elektronische btw- en ICP-aangiften instellen](how-to-set-up-electronic-vat-and-icp-declarations.md)  
[Btw-categorieën instellen](how-to-set-up-vat-categories.md)  
[Lijsten met XBRL maken](../../bi-create-reports-with-xbrl.md)  
[Nederlandse lokale functionaliteit](netherlands-local-functionality.md)
