---
title: Pagina's aanpassen | Microsoft Docs
description: Meer informatie over hoe u de gebruikersinterface kunt aanpassen aan uw manier van werken in Business Central.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: customize, personalize, personalization, hide columns, remove fields, move fields, resize column, change column width
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6069e3d1bcfde5c7aead1daeb33b35201c9f05a4
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783308"
---
# <a name="personalize-your-workspace"></a>Uw werkruimte personaliseren
U kunt uw werkruimte aanpassen aan uw werk- en persoonlijke voorkeuren door pagina's te wijzigen zodat deze alleen de gegevens weergeven die u nodig hebt en waar u die nodig hebt. De personalisatiewijzigingen die u maakt, hebben alleen effect op wat u ziet, niet wat andere gebruikers kunnen zien.

U kunt alle soorten pagina's personaliseren, inclusief de rolcentrumpagina. Zie voor meer informatie over rolcentra [Rolcentrum](ui-change-basic-settings.md#role-center).

Afhankelijk van het soort pagina en wat de pagina bevat, kunt u verschillende wijzigingen aanbrengen, zoals velden, kolommen, acties en hele onderdelen verplaatsen of verbergen, en nieuwe velden toevoegen. De meeste personalisatie moet worden gedaan door eerst de banner **Personaliseren** te activeren, maar enkele zeer eenvoudige aanpassingen, zoals kolombreedte, kunnen direct in elke lijst worden uitgevoerd.

> [!NOTE]
> Beheerders kunnen dezelfde indelingswijzigingen uitvoeren als gebruikers door de werkruimte aan te passen voor een profiel dat aan meerdere gebruikers is toegewezen. Zie voor meer informatie [Pagina's aanpassen voor rollen](ui-personalization-manage.md).<br /><br />
Beheerders kunnen ook personalisering van gebruikers overschrijven of uitschakelen en ze kunnen definiëren welke functies zelfs door gebruikers in alle of specifieke bedrijven kunnen worden gezien. Zie [Business Central aanpassen](ui-customizing-overview.md) voor meer informatie.

## <a name="video-overview"></a>Video-overzicht
De volgende video toont enkele manieren waarop u uw rolcentrum kunt personaliseren.

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4ArUB?rel=0]

## <a name="to-change-the-width-of-a-column"></a>De breedte van een kolom wijzigen
U kunt het formaat van kolommen in elke lijst eenvoudig wijzigen door de grens tussen twee kolommen naar links of rechts te slepen.
1. Selecteer in de koptekst van een lijst de grens tussen twee kolommen.
2. U kunt ook dubbelklikken op de grens tussen twee kolommen om de breedte van de kolom automatisch aan te passen. Dit stelt de breedte in op de optimale grootte voor leesbaarheid.

Wat betreft andere personalisatie, worden de wijzigingen die u aanbrengt in de kolombreedte opgeslagen in uw account en volgen deze u ongeacht op welk apparaat u zich aanmeldt.

## <a name="to-start-personalizing-a-page-through-the-personalizing-banner"></a>Een pagina personaliseren via de banner **Personaliseren**
1. Open een pagina die u wilt personaliseren.
2. In de rechterbovenhoek selecteert u het pictogram ![Instellingen](media/ui-experience/settings_icon_small.png "Pictogram Instellingen voor rolcentrum") en vervolgens kiest u de actie **Personaliseren**.

    De banner **Personaliseren** verschijnt bovenin, waarmee wordt aangegeven dat u wijzigingen kunt gaan aanbrengen.

    > [!NOTE]
    > Gebruik Ctrl+klik op een actie om te navigeren tijdens personalisatie als de actie wordt gemarkeerd door de pijlpunt.

    Als u een ![Personalisatievergrendeling](media/personalization-lock-icon.png "Personalisatievergrendeling") of ![Personalisatie geblokkeerd](media/personalization-blocked-icon.png "Personalisatie geblokkeerd") ziet in de banner, kunt u de pagina niet personaliseren. Zie voor meer informatie [Waarom is een pagina vergrendeld voor personaliseren?](ui-personalization-locked.md).

3. Als u een veld wilt toevoegen, kiest u de actie **+ Veld**.
4. Sleep vanuit het deelvenster **Veld toevoegen aan pagina** een veld naar de gewenste positie op de pagina.
5. Als u een UI-element wilt wijzigen, wijst u naar het element, zoals een actie, een veld of een onderdeel. Het element wordt onmiddellijk gemarkeerd met een pijlpunt of rand.
6. Kies het element en kies vervolgens **Verplaatsen**, **Verwijderen**, **Verbergen**, **Weergeven**, **Weergeven onder 'Meer tonen'**, **Weergeven wanneer samengevouwen**, **Altijd weergeven**, **Bevroren deelvenster instellen/wissen** of **Opnemen in/Uitsluiten van snelinvoer**, afhankelijk van het type en de status van het UI-element. Zie [Wat kunt u personaliseren](#What) voor meer informatie.
7. Wanneer u klaar bent met het wijzigen van de indeling van een of meer pagina's, kiest u de knop **Gereed** in de banner **Personaliseren**.

## <a name="what-you-can-personalize"></a><a name="What"></a>Wat kunt u personaliseren

|Wat u wilt doen?|Hoe kunt u het doen?|Opmerkingen|
|----|------------|-------|
|Iets verplaatsen, zoals een veld, een kolom in een lijst, een tegel, een actie of een onderdeel|Wijs naar alles wat u wilt verplaatsen en sleep dit naar de nieuwe positie. De positie wordt aangegeven door een dikke horizontale of verticale lijn.<br /><br />![Pictogram Kan niet hierheen verplaatsen](media/personalization-cannot-move-here.png "Personalisatiemodus - Pictogram Kan niet hierheen verplaatsen") geeft aan dat u het element niet naar de geselecteerde positie kunt verplaatsen.|De onderdelen zijn onderverdelingen of gebieden op een pagina met objecten als meerdere velden, een andere pagina, een grafiek of tegels.<br /><br />Zie voor meer informatie over actiepersonalisering [Acties personaliseren](ui-personalization-user.md#Actions). |
|Iets verbergen, zoals een veld, een kolom in een lijst, een tegel, een actie of een onderdeel.|Kies de pijlpunt en kies <b>Verbergen</b>.|Het element wordt grijs weergegeven wanneer u zich in de personalisatiemodus bevindt. Als het veld dat u verbergt ook in de sneltabbladkop wordt weergegeven wanneer het sneltabblad is samengevouwen, wordt het veld daar niet meer weergegeven.|
|Verborgen acties en onderdelen weergeven.|Kies voor een grijs (verborgen) element de pijlpunt en kies vervolgens <b>Weergeven</b>.|Het verborgen element is weer zichtbaar.|
|Een kolom of veld toevoegen.|Kies in de banner <b>Personaliseren</b> de actie <b>+ Veld</b>.<br /></br>Het deelvenster <b>Veld toevoegen aan pagina</b> wordt aan de rechterkant weergegeven. Hier staan de velden die u aan de pagina kunt toevoegen.<br /><br />Als u een veld wilt toevoegen, moet u het uit het deelvenster slepen naar de positie waar u het hebben wilt. De positie wordt aangegeven door een dikke horizontale of verticale lijn.|Elke pagina bevat een vooraf bepaalde set velden die u kunt weergeven. Gebruik deze procedure om velden of kolommen toe te voegen die niet eerder zijn weergegeven of om velden weer te geven die u hebt verborgen.|
|Een veld weergeven in de kop van een sneltabblad wanneer dit is samengevouwen.|Kies de pijlpunt en kies vervolgens <b>Weergeven wanneer samengevouwen</b>. <br /> <br />Als u deze optie niet ziet, is deze al ingesteld. In dit geval kunt u de weergave van het veld in de sneltabbladkop stoppen door <b>Altijd weergeven</b> te kiezen.|*Sneltabblad* is de term die wordt gebruikt voor een groep velden die onder een gezamenlijke kop worden weergegeven. Gebruik de optie <b>Weergeven wanneer samengevouwen</b> om de belangrijkste velden weer te geven. Als u een veld in de kop selecteert, wordt het sneltabblad geopend met de focus op het geselecteerde veld.<br /><br />Deze optie is alleen van toepassing als een pagina meerdere sneltabbladen bevat. Als er slechts één sneltabblad is, kan het niet worden samengevouwen, dus is de optie <b>Weergeven wanneer samengevouwen</b> niet beschikbaar.|
|Een veld alleen-weergeven maken wanneer u **Meer tonen** selecteert.|Kies de pijlpunt en kies vervolgens <b>Weergeven onder 'Meer tonen'</b>. <br /> <br />Als u de optie <b>Weergeven onder "Meer tonen"</b> niet ziet, is deze al ingesteld. In dit geval kunt u een veld altijd laten weergeven, en niet alleen wanneer u **Meer tonen** selecteert, door <b>Altijd weergeven</b> te kiezen.||
|Het bevroren deelvenster in een lijst in een andere kolom wijzigen. |Kies de pijlpunt van de kolom die u als laatste van het bevroren deelvenster hebben wilt, en kies vervolgens <b>Bevroren deelvenster instellen</b>.<br /><br/>Als u het bevroren deelvenster terug wilt verplaatsen naar de oorspronkelijke positie waarvoor het bestemd was, kiest u de pijlpunt voor de kolom met het huidige bevroren deelvenster en kiest u <b>Bevroren deelvenster wissen</b>. Opmerking: u kunt dit bevroren deelvenster niet verwijderen.|Het bevroren deelvenster geeft de kolommen aan die altijd links worden weergegeven, zelfs als u horizontaal schuift.|  
|Een veld overslaan wanneer u op Enter drukt.|Kies de pijlpunt naast het veld of de kolomkop in een lijst en kies **Uitsluiten van snelinvoer**. <br /><br /> Als u deze optie niet ziet, is het veld al ingesteld om te worden overgeslagen. In dit geval kunt u het overslaan van het veld stoppen door **Opnemen in snelinvoer** te kiezen. |Zie [Gegevensinvoer versnellen met snelinvoer](ui-enter-data.md#QuickEntry)|
|Weergaven die gefilterde lijsten vertegenwoordigen, opnieuw rangschikken en verwijderen.|Kies de pijlpunt naast een weergave en kies vervolgens **Verplaatsen**, **Verwijderen** of **Verbergen**.|Zie [Lijstweergaven opslaan en personaliseren](ui-views.md)|  
|Voeg een nieuwe actie toe aan een pagina of rapport in uw rolcentrum.|Kies op de doelpagina, de rapportverzoekpagina of het venster Vertel me het bladwijzerpictogram.|Zie [Een bladwijzer maken van een pagina of rapport in uw rolcentrum](ui-bookmarks.md)|
|Start een lijst altijd uitgevouwen of samengevouwen|Kies de knop Alles uitvouwen of Alles samenvouwen in de linkerbovenhoek van de lijst of kies de actie Alles uitvouwen of Alles samenvouwen in het menu van de eerste kolom. |Is van toepassing op samenvouwbare hiërarchielijsten|

## <a name="personalizing-actions"></a><a name="Actions"></a>Acties personaliseren

Met personalisatie kunt u bepalen welke acties op de navigatie- en actiebalk en in rolcentra worden weergegeven en waar deze worden weergegeven. U kunt afzonderlijke acties of actiegroepen weergeven, verbergen of verplaatsen. De navigatie- en actiebalk personaliseren gebeurt in wezen op dezelfde manier als met andere elementen van de gebruikersinterface. Wat u precies kunt doen met een actie of groep, hangt er echter vanaf waar de actie of groep zich bevindt. De beste manier om daar achter te komen is de personaliseringsmodus te activeren en de pijlpunten u te laten leiden.

Er zijn enkele termen waarmee u vertrouwd moet zijn om actiepersonalisatie beter te begrijpen: *actiegroep* en *gepromoveerde categorie*.  

Een *actiegroep* is een element dat wordt vergroot om meer acties of groepen weer te geven. Op de pagina **Verkooporders** is de actie **Functies** die wordt weergegeven wanneer u de actie **Acties** kiest, bijvoorbeeld een actiegroep.

Een *gepromoveerde categorie* is een actiegroep die vóór de verticale lijn `|` op de actiebalk wordt weergegeven. De categorieën omvatten meestal de meest gebruikte acties, zodat u deze snel kunt vinden. Bijvoorbeeld op de pagina **Verkooporders** zijn de acties **Order**, **Vrijgeven** en **Boeken** gepromoveerde categorieën.

> [!NOTE]
> U kunt de actiebalk die in onderdelen op de pagina verschijnt, niet personaliseren (bijvoorbeeld het gedeelte met verkoopregels op de pagina **Verkooporder**).

### <a name="to-remove-hide-and-show-actions-and-action-groups"></a>Acties en actiegroepen verwijderen, verbergen en weergeven
Als u een actie wilt weergeven of verbergen, definiëren de opties onder de pijlpunt wat u kunt doen, afhankelijk van de status van de actie.
1. Kies de pijlpunt voor een actie of actiegroep.
2. Kies een van de volgende opties:

|Optie|Wat het doet|
|------|------------
|**Verwijderen**|Deze optie verschijnt als de geselecteerde actie ook ergens anders op de navigatie- of actiebalk wordt weergegeven. Als u deze optie kiest, verwijdert u de actie van de geselecteerde locatie, zodat deze niet meer wordt weergegeven. De actie of actiegroep blijft op de andere locaties. |
|**Verbergen**|Deze optie wordt weergegeven als de actie of groep zich niet ergens anders op de navigatie- of actiebalk bevindt. Net als **Verwijderen** laat het kiezen van deze optie de actie of actiegroep verdwijnen van de navigatie- of actiebalk. In de personalisatiemodus wordt de actie of actiegroep echter nog op de huidige positie weergegeven, behalve dat deze lichtgekleurd wordt weergegeven.|
|**Weergeven**|Deze optie wordt weergegeven als de actie of actiegroep eerder is verborgen (lichtgekleurd). Als u deze optie kiest, wordt de actie of actiegroep weergegeven op de navigatie- of actiebalk.|

### <a name="to-move-actions-and-action-groups"></a>Acties en actiegroepen verplaatsen
Waar u acties of actiegroepen kunt neerzetten wordt aangegeven door een horizontale lijn tussen twee acties of een rand rond een actiegroep. Hier gelden de volgende beperkingen:

- U kunt individuele acties verplaatsen naar gepromoveerde categorieën, maar u kunt de volgorde van de acties in de categorie niet wijzigen.
- U kunt een actiegroep niet naar een gepromoveerde categorie verplaatsen.

1. Als u een actie of actiegroep wilt verplaatsen, sleept u deze naar de gewenste positie, net als met velden en kolommen.
2. Als u een actie of actiegroep verplaatst naar een andere actiegroep die leeg is, sleept u de actie of actiegroep naar de nieuwe groep en zet u deze neer in het kader **Hier een actie neerzetten**.


## <a name="personalizing-parts"></a><a name="Parts"></a>Onderdelen personaliseren

Onderdelen zijn gebieden op een pagina die doorgaans zijn samengesteld uit meerdere velden, grafieken of andere inhoud en die kunnen worden geïdentificeerd door een gekleurde rand wanneer de focus op het onderdeel wordt ingesteld. Een startscherm van een rolcentrum bestaat bijvoorbeeld uit meerdere delen. Vanwege hun goed gedefinieerde grens kunt u het hele onderdeel en de inhoud ervan personaliseren.

- Om een onderdeel te verplaatsen, sleept u het naar de gewenste positie. Een gekleurde lijn geeft geldige posities op het scherm aan. Feitenblokken kunnen bijvoorbeeld alleen worden verplaatst naast andere feitenblokken in het deelvenster Feitenblok.
- U kunt een onderdeel verbergen door de optie **Verbergen** te kiezen onder de pijlpunt.
- Wanneer u begint met personaliseren of naar een nieuwe pagina navigeert, worden alle onderdelen die momenteel verborgen zijn, op de pagina weergegeven met onderscheidende afbeeldingen om aan te geven dat ze verborgen zijn. U kunt een onderdeel zichtbaar maken door de optie **Weergeven** te kiezen onder de pijlpunt.

U kunt alle personalisatiewijzigingen die u in één onderdeel hebt aangebracht, wissen door de optie **Personalisatie wissen** te kiezen onder de pijlpunt van het onderdeel. Personalisatie van een onderdeel wissen heeft alleen invloed op wijzigingen in de inhoud van het onderdeel, niet op de plaatsing of zichtbaarheid van het onderdeel op de pagina.  


## <a name="to-clear-personalization"></a>Personalisatie wissen
Op een bepaald moment wilt u mogelijk sommige of alle personalisatiewijzigingen ongedaan maken die u in de loop van de tijd op een pagina hebt aangebracht.

1. Kies op de banner **Personaliseren** de actie **Personalisatie wissen**.
2. Kies een van de volgende opties. Het wissen van personalisatie kan niet ongedaan worden gemaakt.

|Optie|Wat het doet|
|------|------------
|**Alleen navigatiemenu**|Wist alle personalisatiewijzigingen die u ooit hebt aangebracht in het navigatiemenu dat wordt gedeeld door het rolcentrum en andere pagina's. Dit omvat alle nieuwe acties die als bladwijzers zijn toegevoegd en eventuele wijzigingen in koppelingen en groepen in het menu.|  
|**Alleen acties**|Wist alle personalisatiewijzigingen die u ooit hebt aangebracht in de navigatie- of actiebalk op de pagina.|
|**Alleen velden, kolommen en onderdelen**|Wist alle personalisatiewijzigingen die u ooit hebt aangebracht op de pagina, behalve wijzigingen in de navigatie- of actiebalk. Dit omvat wijzigingen in velden, kolommen, onderdelen en tegels. |
|**Alle**|Wist alle personalisatie die u ooit in de pagina hebt aangebracht, zodat de pagina weer de oorspronkelijke weergave krijgt. Dit omvat wijzigingen in de navigatie- en actiebalk, velden, kolommen, onderdelen en tegels.|

## <a name="additional-points-of-interest"></a>Aanvullende interessante zaken
Er zijn een aantal punten die u in gedachten moet houden als u beter wilt begrijpen hoe personaliseren in zijn werk gaat.

- Als u wijzigingen aanbrengt in een kaartpagina die u kunt openen vanuit een lijst, worden de wijzingen doorgevoerd voor alle records die vanuit die lijst worden geopend. Als u bijvoorbeeld vanuit de lijstpagina Klanten een bepaalde klant opent en vervolgens de pagina personaliseert door een veld toe te voegen. Als u andere klanten vanuit die lijst opent, wordt het veld dat u hebt toegevoegd ook weergegeven.
- De wijzigingen die u aanbrengt worden op al uw rolcentra toegepast. Als u bijvoorbeeld een wijziging in de lijst Klant aanbrengt wanneer het rolcentrum op Bedrijfsleider is ingesteld, kunt u de wijziging op de pagina **Klanten** zien wanneer het rolcentrum op Verkooporderverwerker wordt ingesteld.
- Wijzigingen in een deelvenster van een pagina worden op de pagina toegepast overal waar deze wordt weergegeven.  
- U kunt alleen velden en kolommen toevoegen uit een vooraf gedefinieerde lijst die op de pagina is gebaseerd. U kunt geen nieuwe maken.

## <a name="see-related-training-at-microsoft-learn"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/personalize-ui-dynamics-365-business-central/index)

## <a name="see-also"></a>Zie ook
[Pagina's aanpassen voor profielen](ui-personalization-manage.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  
[Basisinstellingen wijzigen](ui-change-basic-settings.md)  
[Wijzigen welke functies worden weergegeven](ui-experiences.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
