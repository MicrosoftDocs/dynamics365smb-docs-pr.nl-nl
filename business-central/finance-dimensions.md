---
title: Werken met dimensies om gegevens gemakkelijk te volgen en te analyseren
description: U gebruikt dimensies om posten te categoriseren, bijvoorbeeld per afdeling of project, zodat u gemakkelijk gegevens kunt volgen en analyseren zodat u goede zakelijke beslissingen kunt nemen.
author: edupont04
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: analysis, history, track, business intelligence
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7e3bc7abb3908afc1819ac88c910dff85010c735
ms.sourcegitcommit: cbd00f24fb471381bbfd64670237eda176bd78e5
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2021
ms.locfileid: "5947435"
---
# <a name="working-with-dimensions"></a>Werken met dimensies
Dimensies zijn waarden waarmee posten worden gecategoriseerd, zodat u ze kunt bijhouden en analyseren in documenten, zoals verkooporders. Dimensies kunnen bijvoorbeeld aangeven tot welk project of welke afdeling een post behoort.  

In plaats van voor elke afdeling en project aparte grootboekrekeningen in te stellen, kunt u bijvoorbeeld dimensies gebruiken als basis voor analyse en hoeft u geen ingewikkeld rekeningschema te maken. Zie voor meer informatie [Bedrijfsinformatie](bi.md).

Een ander voorbeeld is een dimensie in te stellen met de naam *Afdeling* en deze dimensie te gebruiken wanneer u verkoopdocumenten boekt. Zo kunt u met BI-programma´s bekijken welke afdeling welke artikelen heeft verkocht. Hoe meer dimensies u gebruikt, hoe gedetailleerder de rapporten waarop u uw bedrijfsbeslissingen kunt baseren. Eén verkooppost kan bijvoorbeeld informatie uit meerdere dimensies bevatten, zoals:  

* De rekening waarnaar de artikelverkoop is geboekt  
* Waar het artikel is verkocht
* Wie het heeft verkocht
* Het soort klant die het artikel heeft gekocht  

## <a name="analyzing-by-dimensions"></a>Analyseren per dimensies
Dimensies spelen een belangrijke rol in bedrijfsinformatie, zoals bij het definiëren van analyseweergaven. Zie voor meer informatie [Gegevens analyseren per dimensies](bi-how-analyze-data-dimension.md).

> [!TIP]
> Een snelle manier om transactiegegevens te analyseren per dimensie is de totalen per dimensie van het actiefilter **Dimensiefilter instellen** te gebruiken in het rekeningschema en op pagina's voor posten.

> [!NOTE]
> Analyseweergaven gebruiken vaak gegevens uit dimensies. Als u ontdekt dat een onjuiste dimensie is gebruikt voor geboekte grootboekposten, kunt u de dimensiewaarden corrigeren en uw analyseweergaven bijwerken. Zo blijven uw financiële rapporten en analyses nauwkeurig. Zie [Problemen met dimensies oplossen en dimensies corrigeren](finance-troubleshooting-correcting-dimensions.md#changing-dimension-assignments-after-posting) voor meer informatie

## <a name="dimension-sets"></a>Dimensiesets
<!--we describe what they are, but not their value.-->
Een dimensieset is een unieke combinatie dimensiewaarden. Een dimensieset wordt als dimensiesetposten in de database opgeslagen. Elke dimensiesetpost vertegenwoordigt één dimensiewaarde. De dimensiesetpost wordt geïdentificeerd door een gemeenschappelijke dimensieset-id die is toegewezen aan elke dimensiesetpost die tot de dimensieset behoort.  

Wanneer u een dagboekregel, documentkop of documentregel maakt, kunt u een combinatie van dimensiewaarden opgeven. In plaats van elke dimensiewaarde expliciet in de database op te slaan, wordt een dimensieset-id toegewezen aan de dagboekregel, documentkop of documentregel om zo de dimensieset op te geven.  

## <a name="setting-up-dimensions"></a>Dimensies instellen
U kunt de dimensies en dimensiewaarden definiëren om dagboeken en documenten te categoriseren, zoals verkooporders en inkooporders. U stelt dimensies op de pagina **Dimensies** in. Op deze pagina maakt u één regel voor elke dimensie, zoals *Project*, *Afdeling*, *District* en *Verkoper*.

U stelt ook waarden voor dimensies in. Waarden kunnen bijvoorbeeld afdelingen in uw bedrijf zijn. Dimensiewaarden kunnen worden ingesteld in een hiërarchische structuur, vergelijkbaar met het rekeningschema, zodat gegevens kunnen worden onderverdeeld in verschillende niveaus en zodat subsets van dimensiewaarden kunnen worden opgeteld. U kunt zoveel dimensies en dimensiewaarden definiëren als u nodig hebt en iedereen in uw bedrijf kan deze gebruiken.

Als dimensies en waarden zijn ingesteld, kunt u globale dimensies en shortcutdimensies definiëren op de pagina **Boekhoudinstellingen** die altijd beschikbaar is, om te selecteren als velden op dagboek- en documentregels en posten, zonder eerst de pagina **Dimensies** te hoeven openen. Zie [Globale dimensies en shortcutdimensies instellen](finance-dimensions.md#to-set-up-global-and-shortcut-dimensions) voor meer informatie.

* **Globale dimensies** worden als filters gebruikt, bijvoorbeeld in rapporten, batchverwerkingen en XMLports. U kunt slechts twee globale dimensies gebruiken. Kies dus dimensies die u vaak gebruikt.
* **Shortcutdimensies** zijn beschikbaar als velden in dagboeken, en documentregels en posten. U kunt er maximaal acht maken.  

### <a name="to-set-up-default-dimensions-for-customers-vendors-and-other-accounts"></a>Standaarddimensies voor klanten, leveranciers en andere accounts instellen
U kunt een standaarddimensie toewijzen voor een specifieke rekening. De dimensie wordt naar het dagboek of document gekopieerd wanneer u het rekeningnummer op een regel invoert, maar u kunt de code op de regel desgewenst verwijderen of wijzigen. U kunt ook een dimensie maken die is vereist om een post te boeken met een specifiek rekeningsoort.  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Dimensies** in en kies de desbetreffende koppeling.  
2.  Selecteer op de pagina **Dimensies** de relevante dimensie en kies de actie **Std. dimensierekeningsoort**.  
4.  Vul een regel in voor elke nieuwe standaarddimensie die u wilt instellen. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]  
>  Als u een dimensie verplicht wilt maken maar geen standaardwaarde aan de dimensie wilt toewijzen, laat u het veld **Dimensiewaardecode** leeg en selecteert u vervolgens **Code verplicht** in het veld **Waardeboeking**.  

> [!WARNING]  
>  Als een rekening wordt gebruikt in de batchverwerking **Wisselkoers herwaarderen** of de batchverwerking **Voorraadwaarde boeken**, selecteert u **Verplicht** of **Zelfde** niet. U kunt geen dimensiecodes gebruiken voor deze batchverwerkingen.  

> [!NOTE]  
>  Als een rekening een andere dimensie moet hebben dan de standaarddimensie voor het rekeningsoort, moet u een standaarddimensie voor deze rekening instellen. De standaarddimensie voor de rekening vervangt dan de standaarddimensie voor het rekeningtype.  

### <a name="to-set-up-default-dimension-priorities"></a>Standaarddimensieprioriteiten instellen  
U kunt verschillende standaarddimensies instellen voor verschillende rekeningsoorten, bijvoorbeeld een klantrekening en een artikelrekening. Er kunnen dus meerdere standaarddimensies worden voorgesteld voor een dimensie op een post. Als u dergelijke conflicten wilt voorkomen, kunt u prioriteitregels toepassen op verschillende bronnen.  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Standaarddimensieprioriteiten** in en kies de desbetreffende koppeling.  
2.  Voer op de pagina **Standaarddimensieprioriteiten** in het veld **Broncode** de broncode voor de invoertabel in waarop prioriteiten voor standaarddimensies van toepassing zijn.  
3.  Vul een regel in voor elke prioriteit voor standaarddimensies die u wilt instellen voor de geselecteerde broncode.
4.  Herhaal de procedure voor elke broncode waarvoor u prioriteiten voor standaarddimensies wilt instellen.  

> [!IMPORTANT]  
>  Als u twee tabellen instelt met dezelfde prioriteit voor dezelfde broncode, selecteert [!INCLUDE[prod_short](includes/prod_short.md)] altijd de tabel met de laagste tabel-ID.  

### <a name="to-set-up-dimension-combinations"></a>Dimensiecombinaties instellen  
U kunt bepaalde combinaties van twee dimensies blokkeren of beperken om te voorkomen dat u posten boekt met tegenstrijdige of onjuiste dimensies. Een geblokkeerde dimensiecombinatie betekent dat u beide dimensies niet naar dezelfde post kunt boeken, ongeacht de dimensiewaarden. Voor een beperkte dimensiecombinatie kunt u beide dimensies naar dezelfde post boeken, maar alleen voor bepaalde combinaties van dimensiewaarden.

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Dimensiecombinaties** in en kies de desbetreffende koppeling.  
2.  Kies op de pagina **Dimensiecombinaties** het veld met de dimensiecombinatie en selecteer een van de volgende opties.  

    |Veld|Description|
    |----------------------------------|---------------------------------------|  
    |**Geen beperking**|Deze dimensiecombinatie heeft geen beperkingen. Alle dimensiewaarden zijn toegestaan.|  
    |**Beperkt**|Deze dimensiecombinatie heeft beperkingen afhankelijk van de dimensiewaarden die u invoert. U moet de beperkingen opgeven op de pagina **Dimensiewaardecombinatie**.|  
    |**Geblokkeerd**|Deze dimensiecombinatie is niet toegestaan.|  

3.  Als u de optie **Beperkt** hebt geselecteerd, moet u opgeven welke combinaties van dimensiewaarden u wilt blokkeren. Kies hiervoor het veld om de dimensiecombinatie te definiëren.  
4.  Selecteer vervolgens de dimensiewaardecombinatie die is geblokkeerd en voer **Geblokkeerd** in het veld in. Met een leeg veld geeft u aan dat de dimensiewaardecombinatie is toegestaan. Herhaal deze stap als meerdere combinaties zijn geblokkeerd.  

> [!NOTE]  
>  In rijen en kolommen worden dezelfde dimensies weergegeven en alle dimensiecombinaties komen daarom twee keer voor. [!INCLUDE[prod_short](includes/prod_short.md)] geeft de instelling automatisch in beide velden weer. U kunt niets in de velden in de linkerbovenhoek en daaronder selecteren, omdat deze velden dezelfde dimensie bevatten in de rijen en de kolommen.  
>   
>  De geselecteerde optie is niet zichtbaar voordat u het veld sluit.  
>   
>  Als u de naam van de dimensies wilt weergeven en niet de code, klikt u op het veld **Kolomnaam weergeven**.

### <a name="to-set-up-global-and-shortcut-dimensions"></a>Globale dimensies en shortcutdimensies instellen
Globale dimensies en shortcutdimensies kunnen als filter worden gebruikt in [!INCLUDE[prod_short](includes/prod_short.md)], inclusief in rapporten, batchverwerkingen, pagina's met posten en analyseweergaven. Globale dimensies en shortcutdimensies zijn altijd beschikbaar om direct te worden ingevoegd zonder eerst de pagina **Dimensies** te openen. Op dagboek- en documentregels kunt u globale dimensies en shortcutdimensies selecteren in een veld op de regel. U kunt twee globale dimensies en acht shortcutdimensies instellen. Kies de dimensies die u het vaakst gebruikt.

> [!Important]  
> Het wijzigen van een globale of shortcutdimensie vereist dat alle met de dimensie geboekte posten worden bijgewerkt. Als u een globale dimensie wilt wijzigen, gebruikt u de functie **Globale dimensies wijzigen**, maar het kan enige tijd duren, kan vertragend werken en tabellen kunnen tijdens de update worden vergrendeld. Kies daarom uw globale dimensies en shortcutdimensies zorgvuldig, zodat u deze niet later moet wijzigen. Als u een shortcutdimensie wilt wijzigen, gebruikt u de actie **Dimensies wijzigen**. <br /><br />
> Zie voor meer informatie [Globale dimensies wijzigen](finance-dimensions.md#to-change-global-dimensions).

> [!Note]
> Wanneer u een globale of shortcutdimensie toevoegt of wijzigt, wordt u automatisch afgemeld en weer aangemeld, zodat de nieuwe waarde voorbereid is voor gebruik.

1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Grootboek instellen** in en kies de desbetreffende koppeling.
2. Vul de velden van het sneltabblad **Dimensies** in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

#### <a name="to-change-global-dimensions"></a>Globale dimensies wijzigen
Wanneer u een globale of shortcutdimensie wijzigt, worden alle met de betreffende dimensie geboekte posten bijgewerkt. Omdat dit proces tijdrovend kan zijn en de prestaties kan beïnvloeden, zijn er twee verschillende modi beschikbaar om het proces aan te passen aan de grootte van de database.  

1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Grootboek instellen** in en kies de desbetreffende koppeling.
2. Kies de actie **Globale dimensies wijzigen**.
3. Selecteer bovenaan de pagina een van de volgende opties om te definiëren in welke modus de batchtaak wordt uitgevoerd.

    |Optie|Omschrijving|
    |-|-|
    |**Sequentieel**|(Standaard) De wijziging wordt in één transactie uitgevoerd, waarbij alle posten worden teruggebracht naar de dimensies die ze hadden vóór de wijziging.<br /><br />Deze optie wordt aanbevolen als het bedrijf relatief weinig geboekte vermeldingen bevat en de voltooiing ervan zo kort mogelijk duurt. Het proces vergrendelt meerdere tabellen en blokkeert andere gebruikers totdat het klaar is. Merk op dat in grote databases het proces mogelijk niet kan worden voltooid in deze modus. Gebruik in dat geval de optie **Parallel**.|
    |**Parallel**|De dimensiewijziging vindt plaats in meerdere achtergrondsessies en de bewerking wordt opgesplitst in meerdere transacties. Om deze optie te gebruiken, zet u de schakelaar **Parallelle verwerking** aan. <br /><br />Deze optie wordt aanbevolen voor grote databases of bedrijven met veel geboekte posten, omdat de voltooiing ervan zo kort mogelijk duurt. Merk op dat in deze modus het updateproces niet start als er meer dan één actieve databasesessie is.|  

4. Voer in de velden **Code globale dimensie 1** en/of **Code globale dimensie 2** de nieuwe dimensiecode(s) in. De huidige afmetingen worden grijs weergegeven achter de velden.
5. Voer, afhankelijk van de modus, een van de volgende handelingen uit:
    * Kies in de modus **Sequentieel** de actie **Starten**.
    * Kies in de modus **Parallel** de actie **Voorbereiden**.

    Het tabblad **Logposten** wordt gevuld met informatie over de afmetingen die zullen worden gewijzigd.
7. Meld u af bij [!INCLUDE[prod_short](includes/prod_short.md)] en meld u vervolgens weer aan.
8. Kies de actie **Starten** om de parallelle verwerking van de dimensieveranderingen te starten. <!--is this also dependent on the mode?-->

### <a name="example-of-dimension-setup"></a>Voorbeeld van dimensie-instelling
Stel dat uw bedrijf transacties wil traceren op basis van organisatorische structuur en geografische locaties. Hiervoor kunt u twee dimensies instellen op de pagina **Dimensies**:

* **DISTRICT**  
* **AFDELING**  

| Code | Name | Codebijschrift | Filterbijschrift |
| --- | --- | --- | --- |
| DISTRICT |District |Districtcode |Districtfilter |
| KSTNPLAATS |Kostenplaats |Afdelingscode |Kostenplaatsfilter |

Voor **DISTRICT** voegt u de volgende dimensiewaarden toe:

| Code | Name | Dimensiewaardesoort |
| --- | --- | --- |
| 10 |Noord- en Zuid-Amerika |Begintotaal |
| 20 |Noord-Amerika |Standaard |
| 30 |Stille Oceaan |Standaard |
| 40 |Zuid-Amerika |Standaard |
| 50 |Noord- en Zuid-Amerika, totaal |Eindtotaal |
| 60 |Europa |Begintotaal |
| 70 |EU |Standaard |
| 80 |Niet-EU |Standaard |
| 90 |Europa, totaal |Eindtotaal |

Voor de twee belangrijke geografische gebieden, Noord- en Zuid-Amerika en Europa, voegt u subcategorieën toe voor regio's door de dimensiewaarden te laten inspringen. Zo kunt u rapporteren over verkoop of kosten in regio's en totalen ophalen voor de grotere geografische gebieden. U kunt er ook voor kiezen landen of regio's te gebruiken als uw dimensiewaarden, of provincies of plaatsen. Dit hangt af van uw bedrijf.

> [!NOTE]  
>   Als u een hiërarchie wilt instellen, moeten de codes op alfabetische volgorde staan Dit omvat de codes van de dimensiewaarden die worden verschaft in [!INCLUDE[prod_short](includes/prod_short.md)].  

Voor **AFDELING** voegt u de volgende dimensiewaarden toe:

| Code | Name | Dimensiewaardesoort |
| --- | --- | --- |
| ADMIN |Beheer |Standaard |
| PROD |Productie |Standaard |
| VERKOOP |Verkoop |Standaard |

Met deze instellingen kunt u uw twee dimensies toevoegen als twee globale dimensies op de pagina **Boekhoudinstellingen**. Dit betekent dat u DISTRICT en AFDELING kunt gebruiken als filters voor grootboekposten, evenals in alle rapporten en rapportageschema's. Beide globale dimensies kunnen ook automatisch worden gebruikt als shortcutdimensies in postregels en documentkoppen.

## <a name="getting-an-overview-of-dimensions-used-multiple-times"></a>Een overzicht krijgen van dimensies die meerdere keren zijn gebruikt
Op de pagina **Standaarddimensies - Multi** wordt opgegeven hoe een groep rekeningen gebruikmaakt van dimensies en dimensiewaarden. Markeer meerdere rekeningen en geef standaard dimensies en dimensiewaarden op voor de rekeningen die u hebt gemarkeerd in het overzicht met rekeningen. Wanneer u standaarddimensies voor de gemarkeerde rekeningen opgeeft, worden deze dimensies en dimensiewaarden voorgesteld wanneer een van deze rekeningen wordt gebruikt, bijvoorbeeld op een dagboekregel. Dit maakt het boeken van een post eenvoudiger voor de gebruiker, omdat de dimensievelden automatisch worden ingevuld. De voorgestelde dimensiewaarden kunnen echter worden gewijzigd, bijvoorbeeld op een dagboekregel.

De pagina **Standaarddimensies - Multi** bevat de volgende velden:

|Veld|Description|
|-----|-----------|  
|**Dimensiecode**|Bevat die dimensies die zijn ingesteld als standaarddimensies in een of meer gemarkeerde rekeningen. Kies het veld voor een overzicht van de beschikbare dimensies. Als u een dimensie selecteert, wordt de geselecteerde dimensie voor de gemarkeerde rekeningen ingesteld als standaard dimensie.|
|**Dimensiewaardecode**|Bevat een dimensiewaarde of de term (Conflict). Als het veld een dimensiewaarde bevat, hebben de gemarkeerde rekeningen dezelfde standaard dimensiewaarde voor een dimensie. Bevat het veld de term (Conflict), dan hebben niet alle gemarkeerde rekeningen dezelfde standaard dimensiewaarde voor een dimensie. Kies het veld voor een overzicht van de beschikbare dimensiewaarden voor een dimensie. Als u een dimensiewaarde selecteert, wordt de geselecteerde dimensiewaarde ingesteld als standaard dimensiewaarde voor de gemarkeerde rekeningen.|
|**Waardeboeking**|Bevat een regel voor waardeboeking of de term (Conflict). Als het veld een regel voor waardeboeking bevat, hebben de gemarkeerde rekeningen dezelfde regel voor waardeboeking voor een dimensiewaarde. Bevat het veld de term (Conflict), dan hebben niet alle gemarkeerde rekeningen dezelfde regel voor waardeboeking voor een dimensiewaarde. Kies het veld Waardeboeking voor een overzicht van de regels voor waardeboeking. Als u een regel voor waardeboeking selecteert, wordt de geselecteerde regel voor waardeboeking toegepast op de gemarkeerde rekeningen.|

## <a name="using-dimensions"></a>Dimensies gebruiken
In een document zoals een verkooporder kunt u dimensiegegevens toevoegen voor een afzonderlijke documentregel en voor het document zelf. Op de pagina **Verkooporder** kunt u bijvoorbeeld dimensiewaarden invoeren voor de eerste twee shortcutdimensies op de afzonderlijke verkoopregels, en u kunt meer dimensiegegevens toevoegen als u de knop **Dimensies** kiest.  

Als u in plaats daarvan in een dagboek werkt, kunt u ook op dezelfde manier dimensiegegevens toevoegen aan een post als u shortcutdimensies direct als velden hebt ingesteld op dagboekregels.  

U kunt standaarddimensies instellen voor rekeningen of rekeningsoorten, zodat dimensies en dimensiewaarden automatisch worden ingevuld.

### <a name="to-view-global-dimensions-in-ledger-entry-pages"></a>Globale dimensies bekijken op pagina's met posten  
Globale dimensies zijn altijd gedefinieerd en benoemd door het bedrijf. Als u de globale dimensies voor het bedrijf wilt bekijken, opent u de pagina **Boekhoudinstellingen**.  

Op een pagina met posten kunt u bekijken of er globale dimensies van toepassing zijn op de posten. In tegenstelling tot de overige dimensies kunnen de twee globale dimensies overal in [!INCLUDE[prod_short](includes/prod_short.md)] als filter worden toegepast.  

1.  Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Rekeningschema** in en kies de desbetreffende koppeling.  
2.  Kies op de pagina **Rekeningschema** de actie **Posten**.  
3.  Stel een of meer filters op de pagina in om alleen de gewenste posten weer te geven.  
4.  Als u alle dimensies voor een post wilt zien, selecteert u de post en kiest u vervolgens de actie **Dimensies**.  

> [!NOTE]  
>  Op de pagina **Postdimensies** worden de gegevens per post weergegeven. Als u de posten doorloopt, wordt de inhoud op de pagina **Postdimensies** hieraan aangepast.

## <a name="see-related-training-at-microsoft-learn"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/dimensions-dynamics-365-business-central/index)

## <a name="see-also"></a>Zie ook
[Bedrijfsinformatie](bi.md)  
[Financiën](finance.md)  
[Gegevens analyseren per dimensie](bi-how-analyze-data-dimension.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]