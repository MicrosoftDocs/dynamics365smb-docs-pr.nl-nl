---
title: Gebruikers en rollen beheren
description: Leer hoe u gebruikersprofielen beheert in Business Central.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics-365-business-central
ms.topic: how-to
ms.date: 07/26/2024
ms.custom: bap-template
ms.search.form: '9171,'
---
# <a name="manage-user-profiles"></a>Gebruikersprofielen beheren

Wijs alle gebruikers toe aan profielen die het volgende weerspiegelen:

* Hun zakelijke rol
* De afdeling waar ze werken
* Een ander type categorisatie

Met profielen kunnen beheerders centraal definiëren en beheren tot welke verschillende soorten gebruikers toegang hebben in Business Central.

Het typische zakelijke gebruik van een profiel is een rol. Een profiel wordt daarom genoemd *Profiel (rol)* in de gebruikersinterface.

Als beheerder maakt en beheert u profielen op de pagina **Profielen (rollen)**. Elk profiel heeft een kaart waarop u de instellingen voor de gerelateerde rol beheert. De kaart bevat de volgende informatie:

* Naam van de rol
* Gebruikersconfiguratie
* Het rolcentrum dat door het profiel wordt gebruikt

Zie voor meer informatie over gebruikersinstellingen en rolcentra [Basisinstellingen wijzigen](ui-change-basic-settings.md).

Voordat u gebruikersprofielen kunt beheren, moeten de gebruikers worden gemaakt en toegevoegd via het Microsoft 365-beheercentrum. U kunt vervolgens machtigingen toewijzen aan elke gebruiker of gebruikersgroep. Machtigingen definiëren de functies waartoe gebruikers toegang hebben. Zie [Machtigingen toewijzen aan gebruikers en groepen](ui-define-granular-permissions.md) voor meer informatie over machtigingsinstellingen.

## <a name="page-customization"></a>Pagina-aanpassing

U kunt paginalay-outs voor een profiel aanpassen, zodat alle gebruikers aan wie het profiel is toegewezen de aangepaste pagina's zien. Als beheerder kunt u pagina's aanpassen met dezelfde functionaliteit die gebruikers gebruiken wanneer ze personaliseren. Zie [Pagina's aanpassen voor profielen](ui-personalization-manage.md) voor meer informatie over het aanpassen van pagina-indelingen.

## <a name="create-a-profile"></a>Maak een profiel aan

Als u geen bestaand profiel kunt kopiëren, kunt u handmatig een nieuw profiel maken.

1. Selecteer  ![Zoeken naar pagina of rapport.](media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken") Pictogram, voer  **Profielen (Rollen)** in en selecteer vervolgens de gerelateerde koppelen.  
2. Selecteer op de pagina **Profielen (rollen)** de actie **Nieuw** .  
3. Vul de vereiste velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

> [!TIP]
> Als u wilt dat een bepaald profiel alleen beschikbaar is voor zeer specifieke gebruikers, kunt u het veld **Beschrijving** instellen op `Navigation menu only.`. Op deze manier wordt het profiel uitgesloten van de lijst met beschikbare rollen in **Mijn instellingen**.

## <a name="copy-a-profile"></a>Een profiel kopiëren

Om tijd te besparen kunt u een nieuw profiel maken door een bestaand profiel te kopiëren. Kopieer er een met vergelijkbare instellingen als die u wilt maken.

Wanneer u een profiel kopieert, worden ook alle gerelateerde pagina-aanpassingen gekopieerd, zowel de door de gebruiker gemaakte aanpassingen als de aanpassingen die van uitbreidingen zijn afgeleid.

1. Selecteer op de pagina  **Profielen (rollen)** de regel voor het profiel dat u wilt kopiëren en selecteer vervolgens de actie  **Profiel kopiëren** .
2. Vul de velden  **Profiel-ID** en  **Weergavenaam** in en selecteer vervolgens de knop  **OK** .
3. Open op de pagina **Profielen (rollen)** de nieuw gemaakte profielkaart en bewerk vervolgens andere velden indien nodig.

## <a name="edit-a-profile"></a>Een profiel bewerken

U kunt een profiel bewerken door de velden te wijzigen op de pagina **Profielen (rollen)**. De wijzigingen zijn echter pas zichtbaar voor de gebruiker aan wie het profiel is toegewezen na af- en weer aanmelden.

> [!Caution]
> Wijzig de naam van het profiel niet terwijl er gebruikers aan wie het profiel is toegewezen, aangemeld zijn, omdat het product dan kan vastlopen en opnieuw opgestart moet worden.

## <a name="assign-a-profile-to-a-user"></a>Een profiel toewijzen aan een gebruiker

Gebruikers kunnen zichzelf een rol toewijzen (die een profiel vertegenwoordigt) door het veld **Rol** te kiezen op de pagina **Mijn instellingen**. Als beheerder kunt u hetzelfde doen via de pagina **Profielen (rollen)**.

1. Selecteer op de pagina  **Profielen (rollen)** het profiel dat u wilt toewijzen en selecteer vervolgens de actie  **Lijst met gebruikerspersonalisatie** .
2. Selecteer op de pagina **gebruikersinstellingen** de gebruiker waaraan u het profiel wilt toewijzen en selecteer vervolgens de actie **Bewerken** .
3. Selecteer in het veld **Profiel-id** het relevante profiel.

Als u een ander profiel aan een gebruiker toewijst, blijven eventuele aanpassingen die door de gebruiker met het vorige profiel zijn aangebracht, behouden.

## <a name="define-user-settings-for-a-profile"></a>Gebruikersinstellingen voor een profiel definiëren

Op de pagina **Mijn instellingen** kunnen gebruikers basisgedrag van hun account definiëren, zoals het rolcentrum, de taal en welke meldingen ze ontvangen. Zie voor meer informatie over gebruikersinstellingen [Basisinstellingen wijzigen](ui-change-basic-settings.md).

Als beheerder kunt u instellingen voor een profiel definiëren. De instellingen zijn van toepassing op alle gebruikers die aan de rol zijn toegewezen.

1. Selecteer het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), Pictogram, voer  **Profielen (Rollen)** in en selecteer vervolgens de gerelateerde koppelen.
2. Selecteer de regel voor het profiel waarvoor u de gebruikersinstellingen wilt wijzigen en selecteer vervolgens de actie  **Lijst met personalisaties voor gebruikers** .
3. Open op de pagina **Persoonlijke gebruikersinstellingen** de kaart voor de gebruiker van wie u de instellingen wilt wijzigen.
4. Bewerk indien nodig op de pagina **Gebruikerspersonalisatiekaart** de velden.

## <a name="activate-a-profile"></a>Activeer een profiel

Wanneer u een profiel maakt, kunt u bepalen of, waar en hoe het profiel en de bijbehorende informatie beschikbaar zijn voor gebruikers.

Schakel op de pagina **Profielen (rollen)** de volgende selectievakjes in:

* **Ingeschakeld** om aan te geven of de gerelateerde rol zichtbaar is op de pagina **Beschikbare rollen** voor gebruikers om uit te kiezen.  
* **Als standaardprofiel gebruiken** om het profiel op te geven dat van toepassing is op gebruikers aan wie geen specifieke rol is toegewezen.
* **Personalisatie uitschakelen** om aan te geven of gebruikers van de gerelateerde rol hun werkruimte kunnen personaliseren.
* **Weergeven in Rollenverkenner** om op te geven of acties op zakelijke functies in het profiel moeten worden weergegeven in de uitgebreide weergave van de rollenverkenner, een functieoverzicht. Zie voor meer informatie over de rolverkenner [Pagina's zoeken met de rolverkenner](ui-role-explorer.md).

## <a name="export-profiles"></a>Profielen exporteren

U kunt profielen exporteren uit [!INCLUDE[prod_short](includes/prod_short.md)] en ze hergebruiken in een andere tenant. De profielen worden geëxporteerd naar een zipbestand dat AL-bestanden (Application Language) bevat. U kunt de AL-bestanden opnieuw gebruiken om extensies te ontwikkelen. Zie [De client gebruiken om profielen en pagina-aanpassingen te maken](/dynamics365/business-central/dev-itpro/developer/devenv-design-profiles-using-client) voor meer informatie over het exporteren van profielen.

* Selecteer op de pagina **Profielen (rollen)** de actie **Profielen exporteren** .

    Deze actie exporteert een zipbestand dat AL-bestanden voor alle profielen bevat.

## <a name="import-profiles"></a>Profielen importeren

U kunt profielen importeren die worden geëxporteerd vanuit Business Central. De stappen zijn min of meer het tegenovergestelde van de stappen om profielen te exporteren.

1. Selecteer op de pagina **Profielen (rollen)** de actie **Profielen importeren** .
1. Volg de stappen in de wizard **Profielen importeren**.

    Als u alleen geselecteerde profielen wilt importeren, gebruikt u het selectievakje **Geselecteerd** om aan te geven welke u wilt importeren.
1. Selecteer de knop  **Geselecteerde importeren** .

    Deze actie importeert een zipbestand dat AL-bestanden voor de geselecteerde profielen.

## <a name="delete-a-profile"></a>Een profiel verwijderen

U kunt een profiel verwijderen door de actie **Verwijderen** te kiezen op de pagina **Profielen (rollen)**. De volgende beperkingen zijn echter van toepassing:

* U kunt een profiel dat aan een gebruiker of een gebruikersgroep is toegewezen, niet verwijderen.
* U kunt geen profielen verwijderen die afkomstig zijn van extensies. De extensie moet eerst worden verwijderd.
* U kunt slechts één profiel tegelijk verwijderen.

## <a name="delete-personalizations"></a>Personalisaties verwijderen

### <a name="delete-all-personalizations-made-by-a-specific-user"></a>Verwijder alle personalisaties die door een specifieke gebruiker zijn gemaakt

U kunt alle wijzigingen die een gebruiker aan een pagina aanbrengt, verwijderen. De pagina's worden dan teruggezet naar de oorspronkelijke indeling. Personalisaties zijn niet gekoppeld aan een profiel (rol). Als een gebruiker een pagina personaliseert, ervaart hij of zij de personalisaties op de pagina, ongeacht welke rol hij of zij gebruikt.<!--Deleting changes can be useful, for example, if an employee changes role and no longer needs them. The profile defines the page layout and deletions restore it back to that definition.--> 

1. Selecteer het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), Pictogram, voer  **gebruikersinstellingen** in en selecteer vervolgens de gerelateerde koppelen.

    Op de pagina **gebruikersinstellingen** worden alle gebruikers weergegeven<!--who make personalizations-->.

2. Selecteer de gebruiker waarvan u de personalisaties wilt verwijderen.
3. Selecteer op de pagina **gebruikersinstellingen** kaart de actie **Gepersonaliseerde pagina's wissen**  en accepteer het bericht dat verschijnt.

De gebruiker ziet de wijzigingen de volgende keer dat hij/zij inlogt.

U kunt ook alle pagina-aanpassingen voor een profiel verwijderen. Zie voor meer informatie [Alle aanpassingen voor een profiel verwijderen](ui-personalization-manage.md#delete-all-customizations-for-a-profile).

### <a name="delete-personalizations-for-specific-pages"></a>Personalisaties voor specifieke pagina's verwijderen

U kunt personalisaties verwijderen die een of meer gebruikers aanbrengen op specifieke pagina's. Personalisaties verwijderen kan bijvoorbeeld handig zijn als een gewijzigd bedrijfsproces betekent dat een personalisatie niet langer moet worden gebruikt. Door verwijderingen wordt de paginalay-out teruggezet naar wat door het profiel wordt gedefinieerd.

1. Selecteer het ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), Pictogram, voer  **Gepersonaliseerde pagina's** in en selecteer vervolgens de gerelateerde koppelen.

    Op de pagina  **Gepersonaliseerde pagina's** worden alle gepersonaliseerde pagina's weergegeven, samen met de gebruiker waartoe ze behoren.

    <!--A checkmark in the **Legacy Personalization** field indicates that the personalization was done in an older version of [!INCLUDE[prod_short](includes/prod_short.md)], which handled personalization differently. Users who try to personalize these pages are locked from doing so unless they choose to unlock the page.-->

2. Selecteer de regel voor de paginapersonalisatie die u wilt verwijderen en selecteer vervolgens de actie  **Verwijderen** .

De gebruiker ziet de wijzigingen de volgende keer dat hij of zij zich aanmeldt.  

U kunt ook afzonderlijke pagina-aanpassingen voor een profiel verwijderen. Zie voor meer informatie [Aanpassingen voor specifieke pagina's voor een profiel verwijderen](ui-personalization-manage.md#delete-customization-for-specific-pages-for-a-profile).

## <a name="managing-user-sessions"></a>Gebruikerssessies beheren

Als beheerder van [!INCLUDE[prod_short](includes/prod_short.md)] online kunt u gebruikerssessies beheren in het beheercentrum. Zie voor meer informatie [Sessies beheren][def] in de beheerinhoud.  

Voor [!INCLUDE[prod_short](includes/prod_short.md)] on-premises kunt u sessies beheren met bijvoorbeeld SQL Server Management Studio. Zie voor meer informatie [Technische documentatie over SQL Server](/sql/sql-server).  

## <a name="see-also"></a>Zie ook

[Machtigingen toewijzen aan gebruikers en groepen](ui-define-granular-permissions.md)  
[Pagina's aanpassen voor profielen](ui-personalization-manage.md)  
[Uw werkruimte personaliseren](ui-personalization-user.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]

[def]: /dynamics365/business-central/dev-itpro/administration/tenant-admin-center-manage-sessions
