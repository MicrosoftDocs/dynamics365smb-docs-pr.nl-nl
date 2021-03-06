---
title: Veelgestelde vragen over Teams
description: Krijg antwoorden op enkele veelvoorkomende vragen over het werken met Teams en Business Central.
author: jswymer
ms.service: dynamics365-business-central
ms.topic: get-started-article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Teams, MS Teams, Microsoft Teams, Skype, Link, Microsoft 365, collaborate, collaboration, teamwork, faq, errors
ms.date: 05/19/2021
ms.author: jswymer
ms.openlocfilehash: f3c9626fa73247b2109e5f179aef405e80b44b07
ms.sourcegitcommit: 5a916b0aa0a2eef0c22b5722a0af041757e6d7c2
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "6074637"
---
# <a name="teams-faq"></a>Veelgestelde vragen over Teams

[!INCLUDE [online_only](includes/online_only.md)]

In dit artikel worden enkele van de vragen beantwoord die u mogelijk hebt over het werken met Teams en [!INCLUDE [prod_short](includes/prod_short.md)].

## <a name="general"></a>[Alge&meen](#tab/general)

### <a name="how-do-i-sign-in-to-the-prod_shortmd-app-in-teams"></a>Hoe log ik in bij de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app in Teams?

Nadat u de app hebt geïnstalleerd, wordt u gevraagd om in te loggen wanneer u de app voor het eerst gebruikt, wanneer u een [!INCLUDE [prod_short.md](includes/prod_short.md)]-koppeling in Teams-chat plakt of wanneer u de actie **Details** kiest op een kaart in Teams. Afhankelijk van uw Teams-client, moet u mogelijk uw inloggegevens invoeren die u gebruikt om toegang te krijgen tot [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-sign-out-of-the-prod_shortmd-app-in-teams"></a>Hoe log ik uit bij de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app in Teams?

Om u af te melden bij uw huidige gebruikersidentiteit in Teams waarmee u verbinding hebt gemaakt met [!INCLUDE [prod_short.md](includes/prod_short.md)], gaat u naar een willekeurig chatvak, klikt u met de rechtermuisknop op het pictogram [!INCLUDE [prod_short.md](includes/prod_short.md)] eronder en kiest u **Instellingen**. Wanneer het venster verschijnt, controleert u uw momenteel aangemelde identiteit en kiest u vervolgens **Afmelden**.

### <a name="does-the-app-for-teams-connect-to-prod_shortmd-on-premises"></a>Maakt de app voor Teams verbinding met [!INCLUDE [prod_short.md](includes/prod_short.md)] on premises? 

Nee. De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor teams werkt alleen met [!INCLUDE [prod_short.md](includes/prod_short.md)] online. Er zijn geen plannen om [!INCLUDE [prod_short.md](includes/prod_short.md)]-implementatietypen te ondersteunen&mdash;zoals on-premises, hybride cloud of privécloud&mdash;die Microsoft niet rechtstreeks host of beheert.

### <a name="does-the-app-work-with-multiple-companies-and-environments"></a>Werkt de app met meerdere bedrijven en omgevingen? 

Ja. Als u contacten in een ander bedrijf wilt zoeken, gaat u naar [Instellingen](across-teams-settings.md). Wanneer de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app een koppeling uitbreidt tot een kaart, moet de koppeling de omgeving en bedrijfsnamen voor de app bevatten om overeen te komen met de record in het juiste bedrijf. U kunt koppelingen plakken naar alle bedrijven en omgevingen waartoe u toegang heeft binnen uw organisatie en vanuit het [!INCLUDE [prod_short.md](includes/prod_short.md)]-account waarmee u zich heeft aangemeld. Deelnemers aan de chat zien de kaart. Maar ze kunnen de kaartgegevens niet bekijken, tenzij ze machtigingen hebben voor het bedrijf of de omgeving waar die record is opgeslagen.

### <a name="in-which-countries-or-regions-is-the-prod_shortmd-app-available"></a>In welke landen of regio's is de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app beschikbaar? 

De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams is niet beperkt per land of regio. De app is beschikbaar in alle markten die momenteel worden ondersteund door de Teams-marktplaats. 

### <a name="does-the-prod_shortmd-app-work-with-any-localization-of-prod_shortmd"></a>Werkt de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app met elke lokalisatie van [!INCLUDE [prod_short.md](includes/prod_short.md)]? 

Ja. De app is bedoeld om te werken met elke lokalisatie van [!INCLUDE [prod_short.md](includes/prod_short.md)], of die lokalisatie nu rechtstreeks van Microsoft of via een partner wordt aangeboden. Zie voor meer informatie [Beschikbaarheid per land/regio en ondersteunde talen](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json).

### <a name="which-languages-does-the-prod_shortmd-app-support"></a><a name="language"></a>Welke talen ondersteunt de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app?

Twee dingen bepalen de taal die wordt gebruikt voor kaarten en kaartdetails in Teams:

1. Uw taal in Teams, die u kunt zien in uw accountinstellingen in Teams. 
2. Uw taal in [!INCLUDE [prod_short.md](includes/prod_short.md)], die u kunt zien in de [!INCLUDE [prod_short.md](includes/prod_short.md)]-webclient (zie [Basisinstelling wijzigen - taal](ui-change-basic-settings.md#language)).

In de volgende tabel wordt uitgelegd hoe de ervaring verschilt voor berichtauteurs en ontvangers, afhankelijk van de taalinstellingen en de beschikbaarheid van talen.

|Wie|Kaart|Kaartdetails |
|-|----|--------------| 
|Berichtauteur |Wordt weergegeven in de taal die voor u is opgegeven in Teams. Als [!INCLUDE [prod_short.md](includes/prod_short.md)] die taal niet biedt, wordt de kaart weergegeven in het Engels. |Wordt weergegeven in de taal die voor u is opgegeven in [!INCLUDE [prod_short.md](includes/prod_short.md)].  waaronder mogelijk talen van taalapps van partners. |
|Berichtontvanger |Wordt weergegeven in de taal van de auteur van het bericht. |Wordt weergegeven in de taal die voor u is opgegeven in [!INCLUDE [prod_short.md](includes/prod_short.md)]. |

Voor de lijst met ondersteunde talen voor [!INCLUDE [prod_short.md](includes/prod_short.md)] raadpleegt u [Ondersteunde talen](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations?toc=/dynamics365/business-central/toc.json#supported-languages).

### <a name="does-the-prod_shortmd-app-work-with-industry-solutions"></a>Werkt de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app met brancheoplossingen?

Ja. Maar slechts enkele functies van de app werken met [Apps insluiten](/dynamics365/business-central/dev-itpro/deployment/embed-app-overview).

- De app werkt met koppelingen op basis van het patroon **\*.bc.dynamics.com**, dat doorgaans wordt gebruikt met Apps insluiten.
- Zoeken naar contactpersonen is niet beschikbaar voor Apps insluiten die de basistoepassing van Microsoft vervangen.

### <a name="where-can-i-find-teams-integration-inside-the-prod_shortmd-web-client"></a>Waar kan ik Teams-integratie vinden in de [!INCLUDE [prod_short.md](includes/prod_short.md)]-webclient? 

Er is momenteel geen insluiting van Teams-besturingselementen of aanwezigheid van Teams-functies in de [!INCLUDE [prod_short.md](includes/prod_short.md)]-webclient of andere clients.

### <a name="does-prod_shortmd-work-with-the-teams-mobile-app"></a>Werkt [!INCLUDE [prod_short.md](includes/prod_short.md)] met de mobiele Teams-app?

Ja. De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app kan worden geïnstalleerd vanuit de Teams-desktopapp of browser, of door een beheerder voor alle gebruikers. Eenmaal geïnstalleerd is de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app automatisch beschikbaar in Teams voor iOS en Android. Op mobiele apparaten kunt u alleen kaarten bekijken die door anderen zijn verzonden, toegang krijgen tot details of de kaart eruit laten springen voor de volledige ervaring in de mobiele [!INCLUDE [prod_short.md](includes/prod_short.md)]-app. U kunt bij het opstellen van berichten geen koppelingen plakken die tot kaarten worden uitgevouwen, of contacten zoeken. Zie voor minimumvereisten voor mobiel [Minimumvereisten voor het gebruik van Business Central](product-requirements.md).

### <a name="is-the-prod_shortmd-app-for-teams-the-same-as-the-prod_shortmd-app-for-ios-and-android"></a>Is de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor teams hetzelfde als de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor iOS en Android?

Nee. De app voor Teams is een add-in voor Microsoft Teams en is exclusief ontworpen voor samenwerkingservaringen die oplichten binnen Teams. Aan de andere kant biedt de mobiele [!INCLUDE [prod_short.md](includes/prod_short.md)]-app een rijke ervaring voor u om te werken met [!INCLUDE [prod_short.md](includes/prod_short.md)]-gegevens op uw mobiele apparaten.

Mobiele gebruikers worden aangemoedigd om zowel de mobiele app als de app voor Teams te installeren, om maximaal te profiteren van [!INCLUDE [prod_short.md](includes/prod_short.md)]. Als beide zijn geïnstalleerd, kunt u de actie **Nieuw venster** op een kaart in Teams kiezen om de kaartdetails in de mobiele [!INCLUDE [prod_short.md](includes/prod_short.md)]-app te openen. Voor informatie over het installeren van de mobiele [!INCLUDE [prod_short.md](includes/prod_short.md)]- en Teams-app raadpleegt u:

- [Business Central op uw mobiele apparaat krijgen](install-mobile-app.md)
- [De mobiele Teams-app](https://support.microsoft.com/office/download-the-mobile-app-for-teams-5940ebdc-0082-4fb1-83c4-751edc23dcb5) downloaden bij Microsoft-ondersteuning

### <a name="does-the-prod_shortmd-app-work-in-all-teams-clients"></a>Werkt de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app in alle Teams-clients?

Nee. De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams wordt niet ondersteund als deze is geïnstalleerd als pakket voor macOS of Linux. Op deze platforms kunt u Teams in plaats daarvan openen met een ondersteunde browser.

Voor minimumvereisten in [!INCLUDE [prod_short.md](includes/prod_short.md)] raadpleegt u [Minimumvereisten voor het gebruik van Business Central](product-requirements.md#teams).

Zie voor informatie over de keuze van Teams-clients en hoe u deze kunt installeren [Klanten krijgen voor Microsoft Teams](/microsoftteams/get-clients) in de Teams-documentatie.

### <a name="which-teams-client-is-best-for-prod_shortmd"></a>Welke Teams-client is het beste voor [!INCLUDE [prod_short.md](includes/prod_short.md)]?

Er zijn slechts kleine verschillen en beperkingen tussen Teams-clients die van invloed kunnen zijn op uw ervaring met de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams. Houd bij het kiezen van een Teams-client rekening met het volgende:

- De camera en locatie zijn niet toegankelijk vanuit het detailvenster in de Teams-desktopapp.
- Telefoonnummers kunnen niet worden geactiveerd vanuit het detailvenster in Teams voor iOS, Teams voor Android of Teams in de browser.
- Als u Microsoft Edge met Teams in de browser gebruikt, kunt u gemakkelijk met meerdere identiteiten en accounts werken door vanuit verschillende profielen in te loggen bij Teams. Voor meer informatie over het gebruik van profielen in Microsoft Edge raadpleegt u [Aanmelden en meerdere profielen maken in Microsoft Edge](https://support.microsoft.com/office/sign-in-and-create-multiple-profiles-in-microsoft-edge-df94e622-2061-49ae-ad1d-6f0e43ce6435) bij Microsoft Ondersteuning.

### <a name="what-is-the-best-way-for-me-to-demonstrate-prod_shortmd-and-microsoft-teams-to-prospective-customers"></a>Wat is voor mij de beste manier om [!INCLUDE [prod_short.md](includes/prod_short.md)] en Microsoft Teams te demonstreren aan potentiële klanten?

Als u een doorverkopende partner bent, wilt u misschien een omgeving hebben die u potentiële klanten kunt laten zien als onderdeel van pre-sales demonstraties. Om gevolgen voor Microsoft Teams in uw organisatie te voorkomen kunt u een Microsoft 365-demoaccount krijgen op [https://aka.ms/CDX](https://aka.ms/CDX). Met dit account hebt u volledige controle over een onafhankelijke Azure-organisatie die Microsoft Teams en [!INCLUDE [prod_short.md](includes/prod_short.md)] omvat. Zie voor meer informatie [Demonstratieomgevingen voorbereiden van Dynamics 365 Business Central](/dynamics365/business-central/dev-itpro/administration/demo-environment).

### <a name="does-the-prod_shortmd-app-for-teams-cater-for-my-customization-and-personalization"></a>Voorziet de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams in aanpassing en personalisatie?

De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams kan kaarten weergeven voor koppelingen naar klantpagina's en tabellen in [!INCLUDE [prod_short.md](includes/prod_short.md)], zoals de pagina's en tabellen die afkomstig zijn van uw eigen aangepaste extensies of van AppSource.

De velden die op een kaart in Teams worden weergegeven, kunnen ook worden beïnvloed door [!INCLUDE [prod_short.md](includes/prod_short.md)]-aanpassingen die voor uw organisatie zijn geïnstalleerd. Kaarten houden geen rekening met rolspecifieke aanpassingen of gebruikerspersonalisatie. Het venster met kaartdetails toont echter de recorddetails zoals u ze zou zien in [!INCLUDE [prod_short.md](includes/prod_short.md)], inclusief eventuele extensies, rolaanpassingen en gebruikerspersonalisatie.

Wanneer u contacten zoekt, worden de velden die overeenkomen in de tabel **Contacten** en velden die in de zoekresultaten worden weergegeven, niet beïnvloed door enige aanpassing of personalisatie.

### <a name="how-do-the-permissions-required-by-the-app-affect-my-privacy"></a>Hoe beïnvloeden de machtigingen die vereist zijn door de app mijn privacy?

Voordat u de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams installeert, kunt u de minimale machtigingen bekijken die nodig zijn om de app te laten functioneren. Door de app te installeren, gaat u ermee akkoord dat de app toestemming heeft om berichten en gegevens te ontvangen die u verstrekt, en dat Teams toestemming heeft om die berichten op te slaan en te verwerken.

Ook bepaalde [!INCLUDE [prod_short.md](includes/prod_short.md)]-functies vereisen het openen van externe koppelingen of toegang tot uw camera of geografische locatie. Stel dat u een foto van een aankoopfactuur wilt maken voor verwerking. De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app gebruikt deze mogelijkheden niet zonder uw toestemming en ze worden alleen gebruikt door specifieke functies in het venster **Details**. Wanneer u een van deze functies voor het eerst gebruikt, geeft Teams een dialoogvenster weer waarin u wordt gevraagd toegang te verlenen tot de vereiste apparaatfuncties.

- Op het Teams-bureaublad kunt u app-machtigingen bekijken en aanpassen vanuit het venster **Instellingen**. Selecteer uw profielfoto bovenaan de app en selecteer **Instellingen** > **Machtigingen** en selecteer vervolgens de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app.

- Voor Teams in de browser en Teams voor iOS of Android kunt u machtigingen bekijken of aanpassen vanuit uw browser of apparaatinstellingen.

> [!NOTE]
> Precies welke [!INCLUDE [prod_short.md](includes/prod_short.md)]-functies u om toestemming vragen, is afhankelijk van de add-on-apps en aanpassingen die zijn toegepast op de [!INCLUDE [prod_short.md](includes/prod_short.md)]-omgeving waarmee u verbinding maakt.

### <a name="where-can-i-learn-about-my-privacy"></a>Waar kan ik meer te weten komen over mijn privacy? 

Hoe Microsoft met uw gegevens omgaat, leest u in de [Privacyverklaring van Microsoft](https://go.microsoft.com/fwlink/?linkid=2030602). 

Neem contact op met uw beheerder voor informatie over hoe uw organisatie omgaat met de privacy van uw gegevens.

### <a name="how-do-i-uninstall-the-prod_shortmd-app-for-teams"></a>Hoe verwijder ik de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams?

Om de app te verwijderen die u voor uzelf hebt geïnstalleerd, gaat u naar een chatvak en zoekt u het pictogram [!INCLUDE [prod_short.md](includes/prod_short.md)] onderaan, klikt u met de rechtermuisknop op het pictogram en kiest u **Verwijderen**.  

### <a name="will-microsoft-continue-to-improve-the-prod_shortmd-app-for-teams"></a>Zal Microsoft de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams blijven verbeteren?

Bij Microsoft luisteren we constant naar feedback van onze zeer uiteenlopende gebruikerscommunity en handelen we naar de beste suggesties. Om te weten wat de toekomst biedt voor de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams raadpleegt u het [Releaseplan voor Dynamics 365](/dynamics365-release-plan/2021wave1/).

Als u wilt deelnemen aan het verbeteren van de app voor Teams, of als u een idee hebt dat uw werk- of samenwerkingservaringen in Teams zou vereenvoudigen, voeg dan een idee toe of stem op bestaande ideeën op [https://aka.ms/BusinessCentralIdeas](https://aka.ms/BusinessCentralIdeas).

## <a name="searching-for-contacts"></a>[Contacten zoeken](#tab/contacts)

### <a name="which-tables-does-the-app-search-in"></a>In welke tabellen zoekt de app?

Bij het zoeken naar contacten vanuit de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams, worden uw zoektermen vergeleken met records in de tabel **Contacten** in [!INCLUDE [prod_short.md](includes/prod_short.md)]. 

### <a name="which-fields-in-the-contacts-table-can-i-search"></a>Welke velden in de contactentabel kan ik zoeken?

Terwijl u uw zoektermen in het zoekvak typt, worden de termen vergeleken met de meeste velden in de tabel **Contacten**. De velden omvatten bijvoorbeeld de velden **Nee.**, **Naam**, **Adres**-velden, **Telefoonnr.** of **Mobiel telefoonnr.** en **E-mail**. 

Zoektermen komen niet overeen met aangepaste velden die zijn toegevoegd aan de tabel **Contacten** door apps en extensies.

### <a name="do-search-results-include-companies-and-persons"></a>Bevatten zoekresultaten bedrijven en personen?

Ja. In [!INCLUDE [prod_short.md](includes/prod_short.md)] kunnen contacten van het type **Bedrijf** of **Persoon** zijn, waarbij een of meer personen aan een bedrijf kunnen zijn verbonden. In de zoekresultaten hebben bedrijven en personen verschillende pictogrammen.

### <a name="do-contacts-of-any-business-relationship-appear-in-the-results"></a>Komen contacten van een zakelijke relatie in de resultaten voor?

Ja. Sommige contacten vertegenwoordigen mogelijk klanten of leveranciers of beide. Andere contacten zonder gedefinieerde zakelijke relatie vertegenwoordigen doorgaans potentiële klanten. Contacten met andere zakelijke relaties, inclusief eventuele aangepaste relaties die u hebt geconfigureerd in [!INCLUDE [prod_short.md](includes/prod_short.md)], worden ook weergegeven in de zoekresultaten.

### <a name="can-i-look-up-contact-details-during-meetings"></a>Kan ik tijdens vergaderingen contactgegevens opzoeken?

Ja. U kunt contactgegevens, interactiegeschiedenis en gerelateerde documenten voor uw klant of leverancier opzoeken tijdens een Teams-vergadering of bellen terwijl de vergadering plaatsvindt, zonder Teams te verlaten.

U kunt zelfs overal in Teams contactgegevens opzoeken met behulp van het opdrachtvak. U kunt bijvoorbeeld contactgegevens opzoeken in de Teams-agenda om u te helpen bij het opzetten van vergaderingen.

### <a name="how-do-i-view-my-last-interactions-with-a-contact"></a>Hoe bekijk ik mijn laatste interacties met een contact?

In het detailvenster voor een contact worden interactielogboekvermeldingen weergegeven. De interactielogboekvermeldingen geven de geschiedenis weer van interacties die uw organisatie heeft gehad met het specifieke contact. De interacties kunnen bestaan uit e-mails die u hebt uitgewisseld, telefoontjes die u hebt ontvangen of documenten die u hebt verzonden.

Om interacties weer te geven, moet [!INCLUDE [prod_short.md](includes/prod_short.md)] geconfigureerd zijn om interacties bij te houden. Zie voor meer informatie over het loggen van interacties [Interacties met contacten vastleggen](marketing-interactions.md).

### <a name="how-do-i-register-a-teams-call-or-meeting-as-an-interaction"></a>Hoe registreer ik een Teams-gesprek of -vergadering als een interactie?

Zoek in het detailvenster voor een contact de actie **Interactie maken** en kies uit de inkomende of uitgaande oproepen als interactiesjablonen. U kunt ook uw eigen aangepaste interactiesjablonen maken, specifiek voor gebruik met Teams-gesprekken.

### <a name="can-i-call-a-contact-from-the-prod_shortmd-app-for-teams"></a>Kan ik een contactpersoon bellen vanuit de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)] heeft een beperkte integratie met de belmogelijkheden van Teams. Het is niet mogelijk om direct een VOIP-gesprek te starten vanuit de contactkaart of het venster met contactgegevens. Wanneer u echter de contactgegevens in de Teams-desktopapp bekijkt, kunt u het telefoonnummerveld selecteren om dat nummer te bellen als Teams is ingesteld als uw standaardbel-app op uw apparaat. Om vaste lijnen of mobiele telefoonnummers te bellen met PSTN, het traditionele telefoonsysteem, heeft Teams de Microsoft 365 Business Voice-app nodig. Zie voor meer informatie [Wat is Microsoft 365 Business Voice?](/MicrosoftTeams/business-voice/whats-business-voice).

### <a name="how-do-i-view-recent-documents-for-a-customer-or-vendor"></a>Hoe bekijk ik recente documenten voor een klant of leverancier?

[!INCLUDE [prod_short.md](includes/prod_short.md)] relateert een contact doorgaans aan een klant- of leveranciersrecord die op zijn beurt weer gerelateerd is aan zakelijke transactierecords, zoals verkoopoffertes of inkoopfacturen. Om gerelateerde documenten voor een contactpersoon te bekijken, gaat u naar het detailvenster van het contact en kiest u de veldwaarde **Zakenrelatie** of gebruikt u de acties om naar de gekoppelde klant of leverancier te navigeren. Vouw op de klant- of leverancierspagina het feitenblokvenster uit om statistieken weer te geven voor verschillende documenten waarop u kunt inzoomen. Uw ervaring kan verschillen op basis van uw aanpassingen en personalisatie.

### <a name="how-do-i-search-for-contacts-using-special-characters"></a>Hoe zoek ik contacten met speciale tekens?

U kunt zoekcriteria invoeren met bijna alle Unicode-tekens. [!INCLUDE [prod_short.md](includes/prod_short.md)] reserveert echter de volgende symbolen voor ander gebruik: **=**, **.**, **\**_ en _*@**. Als u deze symbolen in uw zoektermen gebruikt, levert dit mogelijk niet de verwachte resultaten op. Als u de verwachte resultaten niet ziet, plaatst u de symbolen in uw zoektermen tussen enkele aanhalingstekens, bijvoorbeeld **Contoso'='2**.

### <a name="how-can-i-search-contacts-stored-in-a-different-company"></a>Hoe kan ik zoeken naar contacten die in een ander bedrijf zijn opgeslagen?

De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams kan zoeken naar klanten, leveranciers en andere contacten in één bedrijf tegelijk.  
Om contacten te zoeken die zijn opgeslagen in een ander [!INCLUDE [prod_short.md](includes/prod_short.md)]-bedrijf, opent u [Instellingen](across-teams-settings.md) en verandert u de omgeving en het bedrijf van daaruit.

### <a name="are-prod_shortmd-contacts-different-than-the-ones-in-the-teams-contacts-screen"></a>Zijn [!INCLUDE [prod_short.md](includes/prod_short.md)]-contacten anders dan de contacten in het Teams-contactenscherm?

Ja. Contacten die zijn opgeslagen in [!INCLUDE [prod_short.md](includes/prod_short.md)], vertegenwoordigen zakelijke contacten die beschikbaar zijn voor uw organisatie. Het zijn contacten waarmee u een gevestigde en goed gedefinieerde zakelijke relatie hebt, of contacten die potentiële klanten vertegenwoordigen. Deze contacten zijn doorgaans externe contacten. Ter vergelijking: de contacten die in de lijst Contacten bellen van Teams worden weergegeven, zijn uw eigen contacten. Deze contacten worden niet noodzakelijkerwijs gedeeld met anderen in uw organisatie en vertegenwoordigen doorgaans interne contacten binnen uw organisatie.

### <a name="does-prod_shortmd-synchronize-contacts-with-teams"></a>Synchroniseert [!INCLUDE [prod_short.md](includes/prod_short.md)] contacten met Teams?

Nee. Contacten die zijn opgeslagen in [!INCLUDE [prod_short.md](includes/prod_short.md)], blijven gescheiden van uw contacten die zijn opgeslagen in Teams.
Er zijn momenteel geen plannen om de twee lijsten samen te synchroniseren.

### <a name="what-is-the-minimum-version-of-prod_shortmd-for-contact-search"></a>Wat is de minimumversie van [!INCLUDE [prod_short.md](includes/prod_short.md)] voor contacten zoeken?

Voor het zoeken naar contacten moet u de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams versie 1.0.4 of hoger hebben geïnstalleerd en u maakt verbinding met [!INCLUDE [prod_short.md](includes/prod_short.md)]-omgevingen van versie 18 of hoger.

### <a name="can-i-search-from-my-mobile-device"></a>Kan ik zoeken vanaf mijn mobiele apparaat?

Zoeken naar contacten is momenteel niet beschikbaar vanuit Teams voor iOS en Teams voor Android.

### <a name="which-permissions-do-i-need-for-contact-search"></a>Welke machtigingen heb ik nodig om contacten te zoeken?

Als u contacten wilt zoeken, hebt u machtiging op objectniveau nodig voor de tabel **Contacten** binnen het [!INCLUDE [prod_short.md](includes/prod_short.md)]-bedrijf dat wordt doorzocht. Om het detailvenster van een contact te bekijken, heeft u ten minste leestoestemming nodig voor de pagina **Contact** binnen het [!INCLUDE [prod_short.md](includes/prod_short.md)]-bedrijf en andere gerelateerde objecten.

### <a name="can-i-use-contact-search-if-im-a-delegated-admin"></a>Kan ik contacten zoeken gebruiken als ik een gedelegeerde beheerder ben?

Ja. U kunt ook contacten en contactgegevens opzoeken als u een gedelegeerde beheerdersrol heeft in een organisatie.

### <a name="is-contact-search-affected-by-api-limits"></a>Wordt het zoeken naar contacten beïnvloed door API-limieten?

Ja. Zoeken naar contacten vanuit Teams is gebaseerd op [!INCLUDE [prod_short.md](includes/prod_short.md)] v2.0-API's en onderhevig aan eventuele API-limieten die het gebruik beheren. U kunt meer lezen over de limieten op [Huidige API-limieten](/dynamics-nav/api-reference/v2.0/dynamics-current-limits).

### <a name="why-does-it-sometimes-ask-me-to-set-up-the-app"></a>Waarom word ik soms gevraagd om de app in te stellen?

Nadat u zich voor de eerste keer hebt aangemeld bij de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams, zal de app proberen uw voorkeursbedrijf te bepalen in [!INCLUDE [prod_short.md](includes/prod_short.md)]. Als de app het bedrijf niet kan bepalen, moet u mogelijk naar de **Instellingen** gaan en het bedrijf kiezen waarin u wilt zoeken. Deze situatie doet zich bijvoorbeeld voor als u toegang heeft tot meerdere bedrijven in verschillende omgevingen in uw organisatie. In dat geval moet u een bedrijf kiezen voordat u kunt gaan zoeken.  

De app kan u ook vragen naar **Instellingen** te gaan als u geen [!INCLUDE [prod_short.md](includes/prod_short.md)]-abonnement hebt, zijn er geen [!INCLUDE [prod_short.md](includes/prod_short.md)]-omgevingen of als uw account geen [!INCLUDE [prod_short.md](includes/prod_short.md)]-licentie heeft.

### <a name="id-like-to-search-for-items-or-records-from-other-tables-can-i-do-this-from-teams"></a>Ik zou graag willen zoeken naar items of records uit andere tabellen. Kan ik dit vanuit Teams doen?

Zoeken in andere tabellen is op dit moment niet mogelijk. De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams zoekt alleen in de [!INCLUDE [prod_short.md](includes/prod_short.md)]-contactenlijst, die leveranciers, klanten en andere contacten kan bevatten.

Als u wilt dat de zoekmogelijkheden evolueren en andere tabellen gaan omvatten, moedigen we onze gemeenschap aan om een idee toe te voegen of op bestaande ideeën te stemmen op https://aka.ms/BusinessCentralIdeas.

## <a name="working-with-cards"></a>[Werken met kaarten](#tab/cards)

### <a name="which-types-of-links-does-the-app-support"></a>Welke soorten koppelingen ondersteunt de app?

De [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams reageert op de meeste [!INCLUDE [prod_short.md](includes/prod_short.md)]-webclientkoppelingen. Als de koppeling verwijst naar een enkele record op een pagina, geeft de kaart velden voor die record weer. De ondersteunde paginatypen zijn: 

- Kaartpagina's, zoals de artikelkaart
- Documentpagina's, zoals het verkooporderdocument
- ListPlus-pagina's die één record vertegenwoordigen die is samengesteld uit andere records, zoals een reconciliatieoverzicht voor een bankrekening
- Eenvoudige lijstpagina's waar een record niet de mogelijkheid biedt om in te zoomen op een afzonderlijke detailpagina, zoals de postcodelijst

Bij het plakken van een koppeling naar de root-URL van de webclient, zoals https://businesscentral.dynamics.com, geeft de kaart in plaats daarvan informatie weer om nieuwe gebruikers op weg te helpen met toegang tot [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="how-do-i-delete-a-card-i-sent-to-a-chat"></a>Hoe verwijder ik een kaart die ik naar een chat heb gestuurd?

U kunt een kaart die u al naar chat hebt verzonden, niet verwijderen. Maar u kunt het hele bericht waarvan de kaart deel uitmaakt, verwijderen.

Als berichtauteur kunt u alle berichten verwijderen die u naar chats met een persoon, groep of kanaal hebt verzonden&mdash;tenzij uw beheerder beleid heeft ingesteld dat het verwijderen van berichten verhindert. Als u een kanaal modereert als kanaaleigenaar, heeft uw beheerder u mogelijk ook toestemming gegeven om berichten in het kanaal te verwijderen, inclusief berichten die door andere gebruikers zijn verzonden.

Als u een bericht verwijdert dat een kaart bevat, worden de gegevens in [!INCLUDE [prod_short.md](includes/prod_short.md)] niet verwijderd of gewijzigd.

### <a name="do-cards-always-show-up-to-date-information"></a>Bevatten kaarten altijd up-to-date informatie?

Nee. De veldwaarden op een kaart in Teams, inclusief eventuele afbeeldingen, zijn gebaseerd op de gegevens die beschikbaar waren toen die kaart naar de chat werd gestuurd. [!INCLUDE [prod_short.md](includes/prod_short.md)]-kaarten worden niet automatisch vernieuwd in Teams. 

### <a name="will-others-see-my-card-if-they-dont-have-the-prod_shortmd-app-for-teams"></a>Zullen anderen mijn kaart zien als ze de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams niet hebben? 

Wanneer u een chatbericht opstelt en verzendt dat een kaart bevat, zullen alle gebruikers de kaart zien&mdash;zelfs als ze de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor Teams niet hebben geïnstalleerd.

### <a name="how-do-i-find-out-which-company-a-card-in-teams-belongs-to"></a>Hoe kom ik erachter tot welk bedrijf een kaart in Teams behoort?

Als u in meerdere [!INCLUDE [prod_short.md](includes/prod_short.md)]-bedrijven werkt, overleg dan met uw beheerder over het inschakelen van een bedrijfsbadge voor elk bedrijf. Indien ingeschakeld, verschijnt deze in het oog springende hint in elk detailvenster in Teams en toont het bedrijf en de omgeving waartoe de record behoort. Zie voor meer informatie over het instellen van een bedrijfsbadge [Een bedrijfsbadge weergeven voor snelle toegang tot bedrijfsgegevens](ui-change-basic-settings.md#badge).

## <a name="working-with-card-details"></a>[Werken met kaartgegevens](#tab/carddetails)

### <a name="where-is-the-save-button-in-the-details-window-in-teams"></a>Waar is de knop Opslaan in het detailvenster in Teams?

[!INCLUDE [prod_short.md](includes/prod_short.md)] slaat automatisch wijzigingen op die u in een veld aanbrengt, zodra u het veld verlaat. Om een veld te verlaten, klikt/tikt u ergens buiten het veld of gebruikt u de Tab-toets om naar het volgende veld te gaan. Als er gegevens verschijnen in een dialoogvenster in het detailvenster, moet u mogelijk de knop **OK** kiezen om [!INCLUDE [prod_short.md](includes/prod_short.md)] uw wijzigingen te laten opslaan.

### <a name="if-i-choose-to-view-details-for-a-card-will-other-users-see-my-details-window"></a>Als ik ervoor kies om details van een kaart te bekijken, zien andere gebruikers dan mijn detailvenster?

Nee. Hoewel iedereen in de chat of vergadering de kaart zelf kan zien, verschijnt het detailvenster alleen voor u op uw apparaat wanneer u **Details** kiest. Andere gebruikers moeten **Details** kiezen als ze het detailvenster op hun apparaat willen zien.

### <a name="can-i-start-a-teams-call-from-the-details-window-in-teams"></a>Kan ik een Teams-gesprek starten vanuit het detailvenster in Teams?

Ja. Als u de Teams-desktopapp gebruikt, start u een gesprek door het gekoppelde nummer te kiezen in een telefoonnummerveld, zoals het veld **Mobiel telefoonnr.** op de kaart **Contact**. Teams moet uw aangewezen belapp zijn.

Als u vanuit Teams lokale of internationale vaste lijnen en mobiele telefoons wilt bellen, vereist Teams dat u een Business Voice-licentie hebt voor zakelijk bellen. Ook moet u Teams instellen als uw gespreksoplossing. Zie voor meer informatie [Uw Teams-spraakoplossing plannen](/microsoftteams/cloud-voice-landing-page) in de Teams-documentatie.

### <a name="can-i-print-documents-from-the-details-window-in-teams"></a>Kan ik documenten afdrukken vanuit het detailvenster in Teams?

Ja. U kunt rapporten en andere documenten afdrukken met behulp van standaardafdrukfunctionaliteit van [!INCLUDE [prod_short.md](includes/prod_short.md)] en elke cloud-compatibele printer die is geconfigureerd op de pagina **Printerbeheer** in [!INCLUDE [prod_short.md](includes/prod_short.md)]. U kunt niet vanuit Teams afdrukken naar lokale printers die op uw clientapparaat bekend zijn, zoals printers waarnaar u normaal gesproken vanuit uw browser afdrukt. Om deze reden kunt u niet rechtstreeks vanuit het rapportvoorbeeldvenster afdrukken, maar alleen vanaf de hoofdpagina voor rapportaanvragen, rechtstreeks naar uw cloudprinters.

Zie voor meer informatie over het instellen van cloudprinters [Printers instellen](ui-specify-printer-selection-reports.md).

### <a name="can-i-access-the-camera-from-the-details-window-in-teams"></a>Heb ik toegang tot de camera vanuit het detailvenster in Teams?

Ja. Alle [!INCLUDE [prod_short.md](includes/prod_short.md)]-functies in het detailvenster die de camera gebruiken, zijn beschikbaar op alle Teams-clients.

### <a name="can-i-access-my-location-from-the-details-window-in-teams"></a><a name="location"></a>Heb ik toegang tot mijn locatie vanuit het detailvenster in Teams?

Als u functionaliteit gebruikt in [!INCLUDE [prod_short.md](includes/prod_short.md)] die toegang heeft tot uw huidige locatiecoördinaten, zoals bij kaarten, moet u Teams in de browser of de mobiele Teams-app gebruiken. Locatie is niet beschikbaar bij gebruik van de Teams-desktop-app. 

## <a name="collaborating-with-guests"></a>[Samenwerken met gasten ](#tab/collaborating)

### <a name="can-i-share-cards-with-users-outside-my-organization"></a>Kan ik kaarten delen met gebruikers buiten mijn organisatie?

Ja. Wanneer u een bericht opstelt en verzendt dat een kaart bevat, zien alle ontvangers in de chat de kaart&mdash;zelfs als het gasten zijn of buiten uw organisatie. Gasten kunnen ook het detailvenster openen als ze toestemming hebben gekregen voor toegang tot die gegevens in [!INCLUDE [prod_short.md](includes/prod_short.md)].

### <a name="is-the-experience-any-different-for-users-that-are-guests"></a>Is de ervaring anders voor gebruikers die gasten zijn?

Ja. Door gastgebruikers van buiten uw organisatie uit te nodigen om deel te nemen aan chat of een kanaal, krijgen ze een vergelijkbare, maar niet identieke ervaring als gebruikers binnen uw organisatie. Als een gast een bericht ontvangt met een kaart, kan hij of zij dit bekijken. Gasten kunnen ook het detailvenster openen als ze toestemming hebben gekregen voor toegang tot die gegevens in [!INCLUDE [prod_short.md](includes/prod_short.md)] en een [!INCLUDE [prod_short.md](includes/prod_short.md)]-licentie binnen uw organisatie toegewezen hebben gekregen. Als een gast een bericht opstelt, worden koppelingen naar hun [!INCLUDE [prod_short.md](includes/prod_short.md)] of de uwe niet uitgebreid naar kaarten.

Zie voor meer informatie over overeenkomsten en verschillen tussen gasten en teamleden [Gastervaring in Teams](/MicrosoftTeams/guest-experience) in de Teams-documentatie.

### <a name="how-does-a-guest-user-install-the-prod_shortmd-app"></a>Hoe installeert een gastgebruiker de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app? 

Gasten hebben geen toegang tot de app-marktplaats om zelf apps te installeren. De app kan echter automatisch voor hen worden geïnstalleerd op basis van het beleid van uw organisatie. Een andere manier voor een gastgebruiker om de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app te installeren is wanneer ze een chatbericht ontvangen met een [!INCLUDE [prod_short.md](includes/prod_short.md)]-kaart. In dit geval kiest de gebruiker de knop **Details** of het menu op de kaart en installeert deze vervolgens de [!INCLUDE [prod_short.md](includes/prod_short.md)]-app voor gebruik met uw organisatie. Na het installeren van de app krijgt een gebruiker niet automatisch toestemming om toegang te krijgen tot gegevens uit uw [!INCLUDE [prod_short.md](includes/prod_short.md)].

---

## <a name="see-also"></a>Zie ook

Overzicht van integratie tussen [[!INCLUDE [prod_short](includes/prod_short.md)] en Microsoft Teams](across-teams-overview.md)  
[De [!INCLUDE [prod_short](includes/prod_short.md)]-app installeren voor Microsoft Teams](across-install-app-for-teams.md)  
[Problemen met Teams oplossen](admin-teams-troubleshooting.md)  
[Ontwikkeling voor Teams-integratie](/dynamics365/business-central/dev-itpro/developer/devenv-develop-for-teams)  

## [!INCLUDE[d365fin](includes/free_trial_md.md)]  


[!INCLUDE[footer-include](includes/footer-banner.md)]