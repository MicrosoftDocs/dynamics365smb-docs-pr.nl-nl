---
title: Verbruik of gebruik van projectresources en -artikelen registreren
description: Beschrijft hoe u het verbruik of gebruik van artikelen of resources in projecten registreert om projectbeheer te vergemakkelijken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: project management, consumption
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 65975621fff862b64333c87e70f34b75f8e2cbdb
ms.sourcegitcommit: 93c8681054b059cec38cb29b86de20be37980676
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/23/2021
ms.locfileid: "5938093"
---
# <a name="record-consumption-or-usage-for-jobs"></a>Verbruik of gebruik voor projecten registreren

Op de pagina **Projectplanningsregels** kunt u het gebruik bekijken en vastleggen voor verschillende delen van uw project. Het gebruik wordt automatisch bijgewerkt wanneer u gegevens wijzigt en uitwisselt tussen projecten en projectdagboeken of projectfacturen. Hiervoor moet u een project hebben ingesteld zodat **Gebruikslink toepassen** is ingeschakeld. Zie [Projecten instellen](projects-how-setup-jobs.md) voor meer informatie.  

Zo kunt u bijvoorbeeld voor planningsregels van het soort **Budget** de hoeveelheid van een resource invoeren en aangeven welke hoeveelheid moet worden overgebracht naar het projectdagboek. Als het soort van de planningsregel **Factureerbaar** is, kunt u de hoeveelheid van de resource invoeren en aangeven welke hoeveelheid moet worden overgebracht naar een factuur. Zie voor meer informatie over het factureren van de klant [Projecten factureren](projects-how-invoice-jobs.md). Door de oorspronkelijke hoeveelheid, de resterende hoeveelheid of de geboekte hoeveelheid te vergelijken, kunt u snel gebruiksinformatie bekijken. Voor informatie over het inschatten van gebudgetteerde waarde tijdens planning raadpleegt u [Projectbudgetten beheren](projects-how-manage-budgets.md).  

In de volgende procedures wordt beschreven hoe u werkelijke (gebudgetteerde) hoeveelheden en kosten vastlegt met het projectjournaal. U kunt ook inkoopdocumenten gebruiken om de aankoop voor een project vast te leggen. Zie [Projectvoorraden beheren](projects-how-manage-project-supplies.md) voor meer informatie.

## <a name="to-record-usage-for-a-job-planning-line-of-type-budget"></a>Gebruik vastleggen voor een projectplanningsregel van het soort Budget

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projecten** in en kies de desbetreffende koppeling.  
2. Selecteer het betreffende project en kies vervolgens de actie **Projectplanningsregels**.
3. Selecteer een projectplanningsregel van het soort **Budget** of het soort **Budget en factureerbaar** waarvoor u gebruik wilt vastleggen.  

    > [!NOTE]
    > U kunt ook gebruik vastleggen voor een projectplanningsregel van het soort **Factureerbaar**. Meestal gebruikt u deze regels om facturen te maken, maar u kunt dit ook overbrengen naar een journaal. Zie [Projecten factureren](projects-how-invoice-jobs.md) voor meer informatie <!--However, when you do that, a job planning line of type **Budget** is created to match the billable line. For more information, see [Manage Job Budgets](projects-how-manage-budgets.md).-->

4. In het veld **Aantal te verplaatsen naar dagboek** voert u het aantal in dat u wilt overbrengen. De standaardhoeveelheid is de waarde die u invoert in het veld **Aantal**.

    Het **Resterend aantal** bevat het resterende aantal om het project te voltooien en dat moet worden overgebracht naar het dagboek.  
5. Kies de actie **Projectdagboekregels maken**.

    > [!TIP]
    > Als u meer taakplanningsregels voor deze taak gaat toevoegen, wacht dan met deze stap totdat u alle taakplanningsregels hebt toegevoegd.
6. Vul op de pagina **Projectplanningsregel taakoverdracht** de velden in zoals gewenst en kies vervolgens de knop **OK**. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
7. Kies de actie **Projectdagboek openen**.  
8. Selecteer op de pagina **Projectdagboek** de relevante regel en kies vervolgens de actie **Boeken**.
9. Bekijk op de pagina **Projectplanningsregels** het vastgelegde gebruik door te kijken naar de velden **Aantal**, **Resterend aantal** en **Aantal te verplaatsen naar dagboek**.  
10. Herhaal stap 3 tot en met 8 om aanvullend gebruik vast te leggen.  

## <a name="to-create-job-journal-lines-manually"></a>Handmatig projectdagboekregels maken

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projectdagboeken** in en kies de gerelateerde koppeling.  
2. Kies in het veld **Batchnaam** een relevante projectdagboekbatch.  
3. Voer op een nieuwe regel documentnummer, projectnummer, projecttaaknummer, soort en aantal van het verbruikte soort in.  
4. Wanneer de projectdagboekregels zijn voltooid, kiest u de actie **Boeken**.  

## <a name="to-view-job-usage-estimates-and-post-updates"></a>Projectgebruikschattingen weergeven en updates boeken

U kunt in één stap het projectgebruik tot aan de voltooiing van een project bekijken. Hiervoor gebruikt u de batchverwerking **Project - Resterend gebruik berekenen** voor alle taken tot en met het einde van een project.  

Op deze manier kunt u uw oorspronkelijke schattingen volgen en vergelijken met de werkelijke resultaten en zo nodig wijzigingen aanbrengen of nieuwe posten maken. U hebt bijvoorbeeld mogelijk geschat dat een project 10 uur vereist en tot op heden zijn er al 15 uur aan besteed. U kunt de extra vijf uur aan de bestaande dagboekregel toevoegen of een nieuwe dagboekregel maken om deze vijf uur als overuren te rapporteren. Dit is een ander werksoort. De juiste kosten en prijzen worden berekend die vervolgens naar het dagboek kunnen worden geboekt.  

> [!NOTE]  
>   Artikelposten maken artikeljournaalposten en verkleinen de voorraadhoeveelheid. De batchverwerking **Voorraadwaarde boeken** brengt de kosten van de voorraad over naar het grootboek. Resourceposten maken resourceposten.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projectdagboeken** in en kies de gerelateerde koppeling.  
2. Selecteer een relevant projectdagboek en kies vervolgens de actie **Resterend gebruik berekenen**.  
3. Voer op de pagina **Project - Resterend gebruik berekenen** het documentnummer en de boekingsdatum in die in het dagboek moeten worden ingevoegd, en kies vervolgens de knop **OK**.  
4. Werk het dagboek bij met eventuele wijzigingen die nodig zijn.  
5. Kies de actie **Boeken**.



## <a name="to-review-planning-lines-for-a-job-ledger-entry"></a>Planningsregels voor een projectpost controleren

Nadat u projectdagboekregels hebt geboekt, kunt u de planningsregels zien die zijn gekoppeld aan de projectdagboekposten die zijn geboekt.

> [!NOTE]  
> Hiervoor moet het selectievakje **Gebruikslink toepassen** zijn ingeschakeld voor het project. Zie [Projecten instellen](projects-how-setup-jobs.md) voor meer informatie.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Projectdagboeken** in en kies de gerelateerde koppeling.  
2. Selecteer een relevant projectdagboek en kies vervolgens de actie **Posten**.  
3. Kies op de pagina **Projectposten** de actie **Gekoppelde projectplanningsregels weergeven**.

## <a name="see-also"></a>Zie ook
[Projectbeheer](projects-manage-projects.md)  
[Financiën](finance.md)  
[Inkoop](purchasing-manage-purchasing.md)         
[Verkoop](sales-manage-sales.md)      
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
