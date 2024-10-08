---
title: Financiële rapportages samenstellen met financiële gegevens en accountcategorieën
description: Beschrijft hoe u financiële rapportages gebruikt om diverse weergaven en rapporten te maken om financiële prestatiegegevens te analyseren.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: how-to
ms.date: 03/27/2024
ms.custom: bap-template
ms.search.keywords: 'bi, power BI, analysis, KPI, account schedule, financial report'
ms.search.form: 'Report_25, 103, 104, 108, 195, 196, 197, 198, 488, 489, 490, 764, 765, 766'
ms.service: dynamics-365-business-central
---
# <a name="prepare-financial-reporting-with-financial-data-and-account-categories"></a>Financiële rapportage voorbereiden met financiële gegevens en accountcategorieën

De functie **Financiële rapporten** geeft u inzichten in de financiële gegevens die in uw rekeningschema zijn opgeslagen. U kunt financiële rapporten instellen om cijfers in grootboekrekeningen (GB) te analyseren en grootboekposten te vergelijken met budgetposten. De resultaten worden weergegeven in grafieken en rapporten in uw rolcentrum, zoals het cashflowdiagram, en de rapporten Resultatenrekening en Balans. U opent deze twee rapporten, bijvoorbeeld, met de actie **Financiële overzichten** op de startpagina´s Bedrijfsmanager en Accountant.  

[!INCLUDE[prod_short](includes/prod_short.md)] biedt voorbeelden van financiële rapportages die u meteen als sjablonen kunt gebruiken. U kunt ook uw eigen rapporten instellen om de te vergelijken cijfers op te geven. U kunt bijvoorbeeld financiële rapportages maken om winstmarges te berekenen met behulp van dimensies zoals afdelingen of klantengroepen. Het aantal financiële rapporten dat u kunt maken is onbeperkt en vereist geen tussenkomst van een ontwikkelaar.  

## <a name="prerequisites-for-financial-reporting"></a>Vereisten voor financiële rapportage

Het instellen van financiële rapportages vereist inzicht in de structuur van uw rekeningschema. Er zijn drie belangrijke concepten waar u waarschijnlijk op moet letten voordat u uw financiële rapporten ontwerpt:

- Wijs grootboekboekingsrekeningen toe aan grootboekrekeningcategorieën.
- Ontwerp hoe u dimensies gebruikt.
- Stel grootboekbudgetten in.

Grootboekrekeningcategorieën vereenvoudigen de definities van uw financiële rapporten en zorgen ervoor dat ze beter bestand zijn tegen veranderingen in de rekeningschemastructuur. Meer informatie vindt u op [GB-rekeningcategorieën gebruiken om de indeling van uw financiële overzichten te wijzigen](bi-row-definitions.md#use-gl-account-categories-to-change-the-layout-of-your-financial-statements).

Door dimensies in te stellen, kunt u uw financiële gegevens opsplitsen op manieren die zinvol zijn voor uw organisatie. Zie [Werken met dimensies](finance-dimensions.md) voor meer informatie. 

Als u grootboekposten wilt weergeven als percentages van budgetposten, moet u grootboekbudgetten maken. Zie voor meer informatie [GB-budgetten maken](finance-how-create-budgets.md).

## <a name="financial-reports"></a>Financiële rapporten

Financiële rapporten rangschikken rekeningen uit uw rekeningschema op een manier die het gemakkelijker maakt om gegevens te presenteren. U kunt verschillende indelingen instellen om de informatie te definiëren die u wilt betrekken uit het rekeningschema. In financiële rapporten kunnen ook berekeningen worden uitgevoerd die niet rechtstreeks in het rekeningschema kunnen worden uitgevoerd. U kunt bijvoorbeeld subtotalen maken voor groepen rekeningen en dat totaal vervolgens opnemen in andere totalen. Een ander voorbeeld is winstmarges te berekenen op dimensies zoals afdelingen of klantengroepen. Daarnaast kunt u grootboekposten en budgetposten filteren, op bijvoorbeeld mutatie of debetbedragen.

> [!NOTE] 
> Denk wiskundig gezien aan een financieel rapport zoals gedefinieerd door twee dingen:
>
> - Een vector van rijdefinities die definiëren wat er moet worden berekend.
> - Een vector van kolomdefinities die de gegevens voor de berekening definiëren.
>
> Het financiële rapport is dan het buitenste product van deze twee vectoren, waarbij elke celwaarde wordt berekend op basis van de formule in de rij die wordt toegepast op de gegevensdefinitie uit de kolom.

:::image type="content" source="media/financial-report-definition.svg" alt-text="Laat zien hoe een financieel rapport is opgebouwd uit een rijdefinitie en een kolomdefinitie." lightbox="media/financial-report-definition.svg":::

De pagina **Financiële rapporten** laat zien hoe alle financiële rapporten een patroon volgen dat uit de volgende kenmerken bestaat:

- Naam (code)
- Omschrijving
- Rijdefinitie
- Kolomdefinitie

:::image type="content" source="media/financial-reports.png" alt-text="Laat zien hoe alle financiële rapporten worden opgebouwd uit een rijdefinitie en een kolomdefinitie." lightbox="media/financial-reports.png":::

> [!NOTE]
> De voorbeeldfinancieringsrapporten in [!INCLUDE[prod_short](includes/prod_short.md)] zijn niet kant-en-klaar voor gebruik. Afhankelijk van de manier waarop u uw grootboekrekeningen, dimensies, grootboekrekeningcategorieën en budgetten instelt, moet u de voorbeeldrij- en kolomdefinities en de financiële rapporten waarin ze worden gebruikt, aanpassen aan uw instellingen.

U kunt ook formules gebruiken om twee of meer financiële rapporten en kolomdefinities te vergelijken. Met vergelijkingen kunnen de volgende dingen worden gedaan:

- Aangepaste financiële rapporten maken
- Zo veel financiële rapporten maken als u nodig hebt, elk met een eigen naam.
- Verschillende rapportindelingen instellen en de rapporten afdrukken met de huidige cijfers.

## <a name="learning-path-create-financial-reports-in-microsoft-dynamics-365-business-central"></a>Leertraject: Financiële rapporten maken in Microsoft Dynamics 365 Business Central

Wilt u leren hoe u budgetten kunt maken en vervolgens financiële rapporten, dimensies en rij- en kolomdefinities kunt gebruiken om de financiële rapporten te genereren die bedrijven doorgaans nodig hebben?

Start met het volgende leertraject: [Financiële rapporten maken in Microsoft Dynamics 365 Business Central](/training/paths/create-financial-reports-dynamics-365-business-central)

## <a name="create-a-new-financial-report"></a>Een nieuw financieel rapport maken

U gebruikt financiële rapporten voor het analyseren van grootboekrekeningen of om grootboekposten te vergelijken met budgetposten. U kunt bijvoorbeeld de grootboekposten weergeven als percentages van de begrotingsposten.

De financiële rapporten in de standaardversie van [!INCLUDE[prod_short](includes/prod_short.md)] past mogelijk niet bij uw zakelijke behoeften. Als u snel uw eigen financiële rapporten wilt maken, kunt u beginnen met een bestaand rapport te kopiëren, zoals hieronder is beschreven in stap drie.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent 1.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.  
1. Kies op de pagina **Financiële rapporten** de actie **Nieuw** om een nieuwe naam voor een financieel rapport te maken. Als alternatief kunt u, als u instellingen uit een bestaand financieel rapport opnieuw wilt gebruiken, de actie **Financieel rapport kopiëren** kiezen.
1. Vul de korte naam van het rapport in (u kunt de naam later wijzigen) en de beschrijving.
1. Kies een rijdefinitie en een kolomdefinitie.
1. Kies optioneel analyseweergaven voor de rij- en kolomdefinities.
1. Kies de actie **Financieel rapport bewerken** om toegang te krijgen tot meer eigenschappen in het financiële rapport.
1. Op het sneltabblad **Opties** kunt u de rapportbeschrijving bewerken, de rij- en kolomdefinities wijzigen en definiëren hoe datums worden weergegeven. Voor datums kan een hiërarchie van dag, week, maand, kwartaal, jaar worden gebruikt of er kunnen boekhoudperioden worden gebruikt. Ga voor meer informatie naar [Boekingsperioden vergelijken met behulp van periodeformules](bi-column-definitions.md#comparing-accounting-periods-using-period-formulas).
1. Op het sneltabblad **Dimensies** kunt u dimensiefilters voor het rapport definiëren.
1. U kunt een voorbeeld van het rapport bekijken in het gebied onder het sneltabblad **Dimensies**.

> [!TIP]
> Nadat u een financieel rapport hebt gemaakt, kunt u de pagina **Financieel rapport** gebruiken om een voorbeeld te bekijken en het te valideren. Kies de actie **Financieel rapport weergeven** om de pagina te openen.  

> [!NOTE]
> Wanneer u een financieel rapport opent in de weergave- of bewerkingsmodus, is het filtervenster beschikbaar. Gebruik het deelvenster Filter niet om filters in te stellen voor de gegevens in uw rapport. Dergelijke filters kunnen fouten veroorzaken of filteren de gegevens mogelijk niet daadwerkelijk. Gebruik in plaats daarvan de velden op de sneltabbladen **Opties** en **Dimensies** om filters voor het rapport in te stellen.

### <a name="create-or-edit-a-row-definition"></a>Een rijdefinitie maken of bewerken

Rijdefinities in financiële rapporten bieden een plaats voor berekeningen die niet rechtstreeks in het rekeningschema kunnen worden uitgevoerd. U kunt bijvoorbeeld subtotalen maken voor groepen rekeningen en dat totaal vervolgens opnemen in andere totalen. Ook kunt u tussenstappen berekenen die niet in het eindrapport staan.

Ga voor meer informatie naar [Rijdefinities in financiële rapportage](bi-row-definitions.md).

### <a name="create-or-edit-a-column-definition"></a>Een kolomdefinitie maken of bewerken

Gebruik kolomdefinities om op te geven welke kolommen u in het rapport wilt opnemen. U kunt bijvoorbeeld een rapportindeling maken om mutatie en saldo te vergelijken voor dezelfde periode dit jaar en vorig jaar. U kunt maximaal 15 kolommen in een kolomdefinitie hebben. Meerdere kolommen zijn bijvoorbeeld handig voor het weergeven van budgetten voor 12 maanden met een kolom die het totaal laat zien.

Ga voor meer informatie naar [Kolomdefinities in financiële rapportage](bi-column-definitions.md).

## <a name="using-dimensions-in-financial-reports"></a>Dimensies gebruiken in financiële rapporten

In financiële analyses is een dimensie informatie die u toevoegt aan een post als een soort markering. Deze informatie wordt gebruikt om posten met vergelijkbare kenmerken te groeperen, zoals klanten, regio's, producten en verkopers, en om deze groepen eenvoudig op te kunnen roepen voor analyse. U kunt dimensies gebruiken voor posten in dagboeken, documenten en budgetten.

Elke dimensie beschrijft de focus van de analyse. Een tweedimensionale analyse is bijvoorbeeld verkoop per gebied. Door bij het maken van een boeking meer dan twee dimensies te gebruiken, kunt u een complexere analyse uitvoeren. Een voorbeeld van een complexe analyse is het verkennen van de verkoop per verkoopcampagne per klantengroep per gebied. Zo krijgt u een beter inzicht in uw bedrijf, zoals hoe goed uw bedrijf draait, waar de zaken floreren en waar juist niet en waar meer resources moeten worden ingezet. Dat inzicht helpt u beter gefundeerde zakelijke beslissingen te nemen. Ga voor meer informatie naar [Werken met dimensies](finance-dimensions.md).

## <a name="set-up-financial-reports-with-overviews"></a>Financiële rapporten met overzichten instellen

U kunt een financieel rapport gebruiken om een rekeningoverzicht te maken waarin grootboekcijfers en begrotingscijfers worden vergeleken.

1. Kies het pictogram ![Lampje dat de functie Vertel me 3 opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Selecteer op de pagina **Financiële rapporten** een financieel rapport.  
1. Kies de actie **Rijdefinitie bewerken**  
1. Selecteer op de pagina **Rijdefinitie** in het veld **Naam** de naam van het standaard financiële rapport.
1. Kies de actie **Grootboekrekeningen invoegen**.  
1. Selecteer de rekeningen die u in het rekeningoverzicht wilt opnemen en kies dan **OK**.

    De rekeningen worden opgenomen in uw financieel rapport. Indien gewenst kunt u ook de kolomdefinitie wijzigen.  
1. Kies de actie **Financieel rapport bewerken**.  
1. Stel op de pagina **Financieel rapport** op het sneltabblad **Dimensies** het budgetfilter in op de filternaam die u wilt gebruiken.  
1. Klik op **OK**.  

Nu kunt u het budgetoverzicht kopiëren en in een spreadsheet plakken.  

## <a name="integrate-financial-reports-with-excel"></a>Financiële rapporten integreren met Excel

U kunt een financieel rapport integreren met een Excel-werkmapsjabloon, de lay-out aanpassen aan uw behoeften en vervolgens de Excel-sjabloon bijwerken met gegevens uit [!INCLUDE[prod_short](includes/prod_short.md)]. Deze integratie maakt het bijvoorbeeld eenvoudiger om uw maandelijkse en jaarlijkse financiële overzichten te genereren in een indeling die voor u werkt.

### <a name="set-up-excel-integration-for-a-financial-report-create-an-excel-template"></a>Excel-integratie instellen voor een financieel rapport (een Excel-sjabloon maken)

Om Excel-integratie voor een financieel rapport in te stellen volgt u deze stappen om een ​​Excel-sjabloon voor een rapport te maken.

1. Kies het pictogram ![Lampje dat de functie Vertel me opent 4.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Selecteer op de pagina **Financiële rapporten** het financiële rapport dat u met Excel wilt inschakelen en kies vervolgens de actie **Exporteren naar Excel**.
1. Kies de actie **Nieuw document maken**. Met deze actie wordt een Excel-sjabloonwerkmap gedownload met één werkblad genoemd naar de rapportnaam.
1. Kopieer het werkblad en hernoem het naar **Gegevens**.
1. Hernoem het rapportwerkblad naar wens.
1. Markeer in het rapportwerkblad alle cellen die gegevens uit het financiële rapport weergeven (inclusief kolom- en rijkoppen). Ga op het lint **Home** naar het menu **Nummer** en kies **Algemeen** als de indeling.
1. Kies de meest linkse cel van het gebied met gegevens uit het financiële rapport en stel een verwijzing in naar de equivalente cel in het werkblad Gegevens. Sleep de formule naar rechts om deze uit te breiden naar alle cellen in de eerste rij, en sleep de rij vervolgens omlaag om alle rijen in het financiële rapport te bestrijken.
1. Verberg het werkblad **Gegevens**.
1. Deel het rapportwerkblad in volgens uw behoeften.
1. Sla de werkmap op in OneDrive of een vergelijkbare plaats waar een back-up van het bestand wordt gemaakt en versiebeheer wordt uitgevoerd.
1. Sluit de werkmap.

### <a name="run-a-financial-report-with-an-excel-template"></a>Een financieel rapport uitvoeren met een Excel-sjabloon

Volg deze stappen om een financieel rapport uit te voeren met een Excel-sjabloon:

1. Kies het pictogram ![Lampje dat de functie Vertel me 4 opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Selecteer op de pagina **Financiële rapporten** het financiële rapport dat u met Excel wilt inschakelen en kies vervolgens de actie **Exporteren naar Excel**.
1. Kies de actie **Kopie van bestaand document bijwerken**.
1. Upload uw Excel-sjabloon (sluit de Excel-werkmap voordat u deze uploadt).
1. Kies op de pagina **Naam/waarde Opzoeken** het werkblad Gegevens.
1. [!INCLUDE[prod_short](includes/prod_short.md)] voert het financiële rapport uit en voegt de resulterende gegevens samen met uw Excel-sjabloon.

## <a name="print-and-save-financial-reports"></a>Financiële rapporten afdrukken en opslaan

U kunt financiële rapporten afdrukken met de afdrukservices van uw apparaat. [!INCLUDE[prod_short](includes/prod_short.md)] biedt ook opties om rapporten op te slaan als Excel-werkmappen, Word-documenten, pdf- en XML-bestanden.

1. Kies het pictogram ![Lampje dat de functie Vertel me 4 opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Selecteer op de pagina **Financiële rapporten** het rapport dat u wilt afdrukken en kies vervolgens de actie **Afdrukken**.
1. Vul de vereiste velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]
1. Selecteer in het veld **Printer** het apparaat waarnaar het rapport wordt verzonden.
    1. De optie **(Afgehandeld door de browser)** geeft aan dat er geen aangewezen printer is voor het rapport. In dit geval zal de browser de afdruk afhandelen en de standaardafdrukstappen weergeven, waarbij u een lokale printer kunt kiezen die op uw apparaat is aangesloten. **(Afgehandeld door de browser)** is niet beschikbaar in de mobiele app [!INCLUDE[prod_short](includes/prod_short.md)] of de app voor Teams.
1. Kies de actie **Afdrukken**.

### <a name="schedule-a-financial-report-or-save-as-a-pdf-word-or-excel-document"></a>Plan een financieel rapport of sla het op als pdf-, Word- of Excel-document

U kunt een financieel rapport opslaan in bestandsindelingen, zoals PDF, XML, Word of Excel. [!INCLUDE[prod_short](includes/prod_short.md)] kan ook terugkerende financiële rapporten genereren.

1. Kies het pictogram ![Lampje dat de functie Vertel me 4 opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Kies op de pagina **Financiële rapporten** de actie **Afdrukken**.
1. Stel het rapport dienovereenkomstig in en kies vervolgens de actie **Verzenden naar**.
1. Selecteer de bestandsindeling of de actie **Schema** en kies **OK**.
1. Vul de velden in om een gepland of terugkerend financieel rapport te genereren. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)].<br><br>Stel voor terugkerende financiële rapporten de velden **Vroegste begindatum/-tijd** en **Vervaldatum/-tijd** met respectievelijk de eerste en laatste datum om het financiële rapport te genereren. Selecteer ook op welke dagen het rapport wordt gegenereerd door het veld **Formule voor volgende uitvoeringsdatum** in te stellen conform de indeling uitgelegd in de sectie [Datumformules gebruiken](ui-enter-date-ranges.md#use-date-formulas).


## <a name="best-practices-for-working-with-financial-report-definitions"></a>Best practices voor het werken met definities van financiële rapporten

Er is geen versiebeheer van definities van financiële rapporten. Wanneer u een rapportdefinitie wijzigt, wordt de oude versie vervangen wanneer uw wijziging in de database wordt opgeslagen. De volgende lijst bevat enkele best practices voor het werken met definities van financiële rapporten:

- Als u rapportdefinities toevoegt, kiest u een goede code en vult u het beschrijvingsveld in met een betekenisvolle tekst, terwijl u nog weet waarvoor u het rapport gebruikt. Deze informatie helpt uw ​​collega's (en uzelf in de toekomst) om met het rapport te werken en eventueel de rapportdefinitie te wijzigen.
- Voordat u een rapportdefinitie wijzigt, kunt u overwegen er een kopie van te maken als back-up, voor het geval uw wijziging niet werkt zoals verwacht. U kunt de definitie gewoon kopiëren (geef deze een goede naam) of exporteren. Als u meer wilt weten, gaat u naar [Definities van financiële rapporten importeren of exporteren](#import-or-export-financial-report-definitions).
- Als u een nieuwe kopie nodig heeft van een definitie die [!INCLUDE[prod_short](includes/prod_short.md)] voorziet, kunt u er eenvoudig een krijgen door een nieuw bedrijf op te richten dat alleen instellingsgegevens bevat. Exporteer vervolgens de definitie en importeer deze in het bedrijf waar de definitie moet worden vernieuwd.

## <a name="import-or-export-financial-report-definitions"></a>Definities van financiële rapporten importeren of exporteren

U kunt definities van financiële rapporten importeren en exporteren als RapidStart-configuratiepakketten. Configuratiepakketten zijn bijvoorbeeld handig om informatie te delen met andere bedrijven. Het pakket wordt gemaakt vanuit een .rapidstart-bestand, dat de inhoud comprimeert.

> [!NOTE]
> Wanneer u financiële rapportdefinities importeert, worden bestaande records met dezelfde naam als de records die u importeert, vervangen door de nieuwe definities. Het configuratiepakket voor een rapportdefinitie overschrijft geen bestaande rij- of kolomdefinities die in de rapportdefinitie worden gebruikt.

Volg deze stappen om definities van financiële rapporten te importeren of exporteren:

1. Kies het pictogram ![Lampje dat de functie Vertel me opent 4.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële rapporten** in en kies vervolgens de gerelateerde koppeling.
1. Kies het financiële rapport en kies vervolgens de actie **Financieel rapport importeren** of **Financieel rapport exporteren**, afhankelijk van wat u wilt doen.

Ga naar de volgende artikelen voor meer informatie over het importeren of exporteren van rij- of kolomdefinities voor financiële rapporten: 

- [Rijdefinities van financiële rapporten importeren of exporteren](bi-row-definitions.md#import-or-export-financial-reporting-row-definitions) of
- [Kolomdefinities van financiële rapporten importeren of exporteren](bi-column-definitions.md#import-or-export-financial-report-column-definitions)

## <a name="see-also"></a>Zie ook

[Rijdefinities in financiële rapportage](bi-row-definitions.md)  
[Kolomdefinities in financiële rapportage](bi-column-definitions.md)  
[Rapporten uitvoeren en afdrukken](ui-work-report.md)  
[Financiële Business Intelligence](bi.md)  
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Het grootboek en het rekeningschema](finance-general-ledger.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
