---
title: Werkstromen maken | Microsoft Docs
description: U kunt werkstromen maken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd. Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken. Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8685b1d019c2c11bd459ad4e54ac5a007a9ce871
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775819"
---
# <a name="create-workflows"></a>Werkstromen maken
U kunt werkstromen maken om bedrijfsprocestaken te verbinden die door verschillende gebruikers worden uitgevoerd. Systeemtaken, zoals automatische boekingen, kunnen als stappen in werkstromen worden opgenomen, die worden voorafgegaan of gevolgd door gebruikerstaken. Het aanvragen en verlenen van goedkeuringen om nieuwe records te maken, zijn voorbeelden van veelvoorkomende werkstroomstappen.  

Op de pagina **Werkstroom** kunt u een werkstroom maken door de betrokken stappen te vermelden op de regels. Elke stap bestaat uit een werkstroomgebeurtenis, aangepast door gebeurteniscondities, en een werkstroomantwoord met antwoordopties. U definieert werkstroomregels door velden op werkstroomregels te vullen vanuit lijsten met vaste gebeurtenis- en reactiewaarden die scenario's vertegenwoordigen die worden ondersteund door de toepassingscode.  

Wanneer u werkstromen maakt, kunt u de stappen van bestaande werkstromen of van werkstroomsjablonen kopiëren. Werkstroomsjablonen vertegenwoordigen niet-bewerkbare werkstromen die in de algemene versie van [!INCLUDE[prod_short](includes/prod_short.md)] bestaan. De code voor werkstroomsjablonen die door Microsoft worden toegevoegd hebben het voorvoegsel "MS-", zoals in "MS-PIW". Zie voor meer informatie [Werkstromen maken van werkstroomsjablonen](across-how-to-create-workflows-from-workflow-templates.md).  

Als uw bedrijfsscenario werkstroomgebeurtenissen of -reacties vereist die niet worden ondersteund, moet een Microsoft-partner ze implementeren door de toepassingscode aan te passen.  

> [!NOTE]  
>  Alle berichten over werkstroomstappen worden verzonden via een taakwachtrij. Zorg dat de taakwachtrij in uw installatie is ingesteld om werkstroomberichten te verwerken, en dat het selectievakje **Automatisch starten van NAS** is geselecteerd. Zie voor meer informatie [Gebruik van taakwachtrijen om taken te plannen](admin-job-queues-schedule-tasks.md).  

## <a name="to-create-a-workflow"></a>Een workflow maken  
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Werkstromen** in en kies de gerelateerde koppeling.  
2. Kies de actie **Nieuw**. De pagina **Werkstroom** verschijnt.  
3. Voer in het veld **Code** maximaal 20 tekens in om de werkstroom te identificeren.  
4. Als u de werkstroom wilt maken van een werkstroomsjabloon, kiest u op de pagina **Werkstromen** de actie **Werkstroom maken van sjabloon**. Zie voor meer informatie [Werkstromen maken van werkstroomsjablonen](across-how-to-create-workflows-from-workflow-templates.md).  
5. Beschrijf de werkstroom in het veld **Omschrijving**.  
6. Geef in het veld **Categorie** op tot welke categorie de werkstroom hoort.  
7. Geef in het veld **Als gebeurtenis** de gebeurtenis op die zich moet voordoen om de werkstroomstap te starten.  

    Als u het veld kiest, wordt de pagina **Werkstroomgebeurtenissen** geopend waarin u uit alle bestaande werkstroomgebeurtenissen kunt selecteren.  
8. Geef in het veld **Voorwaarde** een of meer voorwaarden op waaraan moet worden voldaan voordat de gebeurtenis in het veld **Als gebeurtenis** zich kan voordoen.  

    Wanneer u het veld **Gebeurtenisvoorwaarden** kiest, wordt de pagina geopend waarin u een keuze maakt u een lijst met filtervelden die relevant zijn als voorwaarden voor de gebeurtenis in kwestie. U kunt nieuwe filtervelden toevoegen die u wilt gebruiken als gebeurtenisvoorwaarden. U stelt filters voor gebeurtenisvoorwaarden in op dezelfde manier als filters op aanvraagpagina's.  

    Als de werkstroomgebeurtenis de wijziging van een specifiek veld in een record is, wordt de pagina **Gebeurtenisvoorwaarden** geopend met opties om het veld te selecteren en het type wijziging.  

    1.  Als u een veldwijziging voor de gebeurtenis wilt opgeven, selecteert u op de pagina **Gebeurtenisvoorwaarden** in het veld **Veld** die wijziging.  
    2.  Selecteer in het veld **Operator** **Afgenomen**, **Toegenomen** of **Aangepast**.  
9. Geef in het veld **Dan reactie** het antwoord op dat volgt als de werkstroomgebeurtenis plaatsvindt.  

     Als u het veld kiest, wordt de pagina **Werkstroomreacties** geopend waarin u uit alle bestaande werkstroomantwoorden kunt selecteren en antwoordopties kunt instellen voor het geselecteerde antwoord.  
10. Op het sneltabblad **Opties voor de geselecteerde reactie** geeft u als volgt opties op voor het werkstroomantwoord door waarden te selecteren in de verschillende velden die verschijnen:  

    1.  Als u opties voor een werkstroomantwoord wilt opgeven waarbij het gaat om het verzenden van een melding, vult u de velden in de volgende tabel in.  

        |Veld|Omschrijving|  
        |----------------------------------|---------------------------------------|  
        |**Afzender informeren**|Geef op of de aanvrager van de goedkeuring op de hoogte wordt gebracht in plaats van de ontvanger van de goedkeuringsaanvraag. Als u het selectievakje inschakelt, wordt het veld **Gebruikers-id ontvanger** uitgeschakeld omdat de aanvrager van de goedkeuring, de afzender, wordt geïnformeerd in plaats van de ontvanger. De naam van de werkstroomreactie verandert dienovereenkomstig in **Maak een bericht voor &lt;afzender&gt;**. Als het selectievakje niet is ingeschakeld, is de naam van de werkstroomreactie **Maak een bericht voor &lt;gebruiker&gt;**.
        |**Gebruikers-id ontvanger**|Geef de gebruiker op die de melding moet ontvangen. Opmerking: deze optie is alleen beschikbaar voor werkstroomantwoorden met een tijdelijke aanduiding voor een bepaalde gebruiker. Voor werkstroomantwoorden zonder tijdelijke aanduidingen voor gebruikers, wordt de meldingsontvanger meestal bepaald door de goedkeuringsgebruikersinstelling.|  
        |**Type berichtitem**|Geeft aan of het werkstroombericht wordt geactiveerd door een recordwijziging, een goedkeuringsverzoek of een verstreken vervaldatum.|
        |**Doelpagina van koppeling**|Geef een andere pagina in [!INCLUDE[prod_short](includes/prod_short.md)] op die de koppeling in het bericht opent in plaats van de standaardpagina.<br /><br />De pagina moet dezelfde brontabel moet hebben als de betrokken record.|  
        |**Aangepaste koppeling**|Geef de URL op van een koppeling die wordt toegevoegd aan de melding naast de koppeling naar een pagina in [!INCLUDE[prod_short](includes/prod_short.md)].|  
    2.  Als u opties voor een werkstroomantwoord wilt opgeven waarbij het gaat om het maken van een goedkeuringsaanvraag, vult u de velden in de volgende tabel in.  

        |Veld|Description|  
        |----------------------------------|---------------------------------------|  
        |**Formule van vervaldatum**|Geef het aantal dagen op waarbinnen de goedkeuringsaanvraag moet worden opgelost vanaf de datum waarop de aanvraag is verzonden.|  
        |**Delegeren na**|Geef aan of en wanneer een goedkeuringsaanvraag automatisch aan de relevante vervanger wordt gedelegeerd. U kunt selecteren dat één, twee of, vijf dagen na de datum automatisch wordt gedelegeerd als de goedkeuring is aangevraagd.|  
        |**Soort fiatteur**|Geef op wie de fiatteur is, op basis van de instellingen voor goedkeuringsgebruikers en werkstroomgebruikers.<br /><br /> De volgende opties zijn mogelijk:<br /><br /> -   **Verkoper/Inkoper** geeft aan dat de gebruiker die is ingesteld in het veld **Verkoper/inkoper** op de pagina **Gebruikersinstellingen voor goedkeuring**, de fiatteur bepaalt. Goedkeuringsaanvragen worden vervolgens gemaakt op basis van de waarde in het veld **Limietsoort van fiatteur**.<br />     Zie voor meer informatie [Goedkeuringsgebruikers instellen](across-how-to-set-up-workflow-users.md).|  
        |**Bevestigingsbericht tonen**|Geef aan of er een bevestigingsbericht aan gebruikers wordt weergegeven nadat ze een goedkeuring hebben aangevraagd.|  
        |**Limietsoort van fiatteur**|Geef op wat het effect is van goedkeuringslimieten van fiatteurs als posten voor goedkeuringsaanvragen voor ze worden gemaakt. Een gekwalificeerde fiatteur is een fiatteur met een goedkeuringslimiet die hoger is dan de waarde op de uitgevoerde aanvraag.<br /><br /> De volgende opties zijn mogelijk:<br /><br /> 1. **Fiatteursketting** geeft aan dat posten voor goedkeuringsaanvragen worden gemaakt voor alle fiatteurs van de aanvrager tot en met de eerste gekwalificeerde fiatteur.<br />2. **Directe fiatteur** geeft aan dat een goedkeuringsaanvraagpost alleen wordt gemaakt voor de directe fiatteur van de aanvrager, ongeacht de goedkeuringslimiet van de fiatteur.<br />3. **Eerste gekwalificeerde fiatteur** geeft aan dat een goedkeuringsaanvraagpost alleen wordt gemaakt voor de eerste gekwalificeerde fiatteur van de aanvrager.<br />|  
    3.  Als u opties voor een werkstroomantwoord wilt opgeven waarbij het gaat om het maken van dagboekregels vult u de velden in de volgende tabel in.  

        |Veld|Description|  
        |----------------------------------|---------------------------------------|  
        |**Sjabloonnaam van financieel dagboek**|Geef de naam op van de dagboeksjabloon die binnen de opgegeven dagboekregels worden gemaakt.|  
        |**Batchnaam van financieel dagboek**|Geef de naam op van de dagboekbatch die binnen de opgegeven dagboekregels worden gemaakt.|  

11. Kies de knop **Inspringing vergroten** en **Inspringing verkleinen** om de gebeurtenisnaam in het veld **Als** in te laten springen om de positie van de stap in de werkstroom bepalen.  
    1.  Geef aan dat stap de volgende in de werkstroomvolgorde door de gebeurtenisnaam onder de gebeurtenisnaam van de vorige stap te laten springen.  
    2.  Geef aan dat de stap een van meer alternatieve stappen die afhankelijk van de voorwaarde toestand kunnen beginnen, door de gebeurtenisnaam op dezelfde inspringing te plaatsen als de andere alternatieve stappen. Rangschik dergelijke optionele stappen overeenkomstig de prioriteit door de belangrijkste stap eerst te plaatsen.  

    > [!NOTE]  
    >  U kunt alleen de inspringing van een stap wijzigen als er geen verdere stap is.  

12. Herhaal stap 7 t/m 11 om meer werkstroomstappen toe te voegen, voor of na de stap die u zojuist hebt gemaakt.  
13. Schakel het selectievakje **Ingeschakeld** in om aan te geven dat de werkstroom wordt gestart zodra de gebeurtenis in de eerste stap van het type **Startpunt** plaatsvindt. Zie voor meer informatie [Werkstromen gebruiken](across-use-workflows.md).  

> [!NOTE]  
>  Schakel het een werkstroom pas in als u zeker weet dat de werkstroom af is en dat de betreffende werkstroomstappen kunnen beginnen.  

> [!TIP]  
>  Als u relaties wilt zien tussen tabellen die in werkstromen worden gebruikt, kiest u het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen") en voert u **Werkstroom - Tabelrelaties** in.  

## <a name="see-also"></a>Zie ook  
[Werkstromen maken van werkstroomsjablonen](across-how-to-create-workflows-from-workflow-templates.md)   
[Goedkeuringsgebruikers instellen](across-how-to-set-up-approval-users.md)   
[Werkstroomberichten instellen](across-setting-up-workflow-notifications.md)   
[Gearchiveerde instanties van werkstroomstappen bekijken](across-how-to-view-archived-workflow-step-instances.md)   
[Werkstromen verwijderen](across-how-to-delete-workflows.md)   
[Procedure: Een werkstroom voor inkoopgoedkeuring instellen en gebruiken](walkthrough-setting-up-and-using-a-purchase-approval-workflow.md)   
[Werkstromen instellen](across-set-up-workflows.md)   
[Werkstromen gebruiken](across-use-workflows.md)   
[Werkstroom](across-workflow.md)      


[!INCLUDE[footer-include](includes/footer-banner.md)]