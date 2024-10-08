---
title: Rapporten in Power BI Desktop maken om Business Central-gegevens weer te geven
description: Maak uw gegevens als gegevensbron in Power BI beschikbaar en maak krachtige rapporten met de status van uw bedrijf.
author: jswymer
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'business intelligence, KPI, Odata, Power App, SOAP, analysis'
ms.date: 06/12/2024
ms.author: jswymer
ms.service: dynamics-365-business-central
ms.reviewer: jswymer
---

# <a name="building-power-bi-reports-to-display--data"></a>Power BI-rapporten maken om [!INCLUDE [prod_long](includes/prod_long.md)]-gegevens weer te geven

U kunt uw [!INCLUDE[prod_long](includes/prod_long.md)]-gegevens als gegevensbron beschikbaar maken in Power BI Desktop en krachtige rapporten maken over de status van uw bedrijf.

In dit artikel wordt beschreven hoe u aan de slag kunt met Power BI Desktop om rapporten te maken waarin [!INCLUDE[prod_long](includes/prod_long.md)]-gegevens worden weergegeven. Nadat u rapporten hebt gemaakt, kunt u deze publiceren via uw Power BI-service of delen met alle gebruikers in uw organisatie. Zodra deze rapporten zich in de Power BI-service bevinden, kunnen gebruikers die ervoor zijn ingesteld, vervolgens de rapporten bekijken in [!INCLUDE[prod_long](includes/prod_long.md)].

## <a name="get-ready"></a>Bereid u voor

- Meld u aan voor de Power BI-service.

  Als u zich nog niet hebt aangemeld, gaat u naar [https://powerbi.microsoft.com](https://powerbi.microsoft.com). Gebruik wanneer u zich aanmeldt uw zakelijke e-mailadres en wachtwoord.

- Download [Power BI Desktop](https://powerbi.microsoft.com/desktop/).

  Power BI Desktop is een gratis toepassing die u op uw lokale computer installeert. Zie voor meer informatie [Snelle start: verbinden met gegevens in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data).

- Zorg dat de gegevens die u in het rapport wilt, beschikbaar zijn als een API-pagina of zijn gepubliceerd als een webservice. Voor meer informatie zie [Gegevens beschikbaar stellen via API-pagina's of OData-webservices](admin-powerbi-setup.md#exposedata).

<!--- For [!INCLUDE[prod_short](includes/prod_short.md)] on-premises, get the following information:

  - The OData URL for [!INCLUDE[prod_short](includes/prod_short.md)].
  
    Typically, this URL has the format `http[s]://[computer]:[port]/[serverinstance]/ODataV4`, for example, `https://localhost:7048/BC190/ODataV4`. If you have a multi-tenant deployment, include the tenant in the URL, for example, `https://localhost:7048/BC190/ODataV4?tenant=tenant1`.
  - A user name and web service access key of a [!INCLUDE[prod_short](includes/prod_short.md)] account.

    To get data from [!INCLUDE[prod_short](includes/prod_short.md)], Power BI uses basic authentication. So, you'll need a user name and web service access key to connect. The account might be your own user account, or your organization may have specific account for this purpose.-->

- Download het [!INCLUDE [prod_short](includes/prod_short.md)]-rapportthema (optioneel).

  Zie [Het [!INCLUDE [prod_short](includes/prod_short.md)]-rapportthema gebruiken](#theme) in dit artikel voor meer informatie.

[!INCLUDE[note-multicompany-reports](includes/note-multicompany-reports.md)]

## <a name="add--as-a-data-source-in-power-bi-desktop"></a><a name="getdata"></a>[!INCLUDE[prod_short](includes/prod_short.md)] als gegevensbron toevoegen in Power BI Desktop

De eerste taak bij het maken van rapporten is het toevoegen van [!INCLUDE[prod_short](includes/prod_short.md)] als een gegevensbron in Power BI Desktop. Als de verbinding tot stand is gebracht, kunt u beginnen met het maken van het rapport.

1. Start Power BI Desktop.
2. Selecteer **Gegevens ophalen**.

    Als u de optie **Gegevens ophalen** niet ziet, selecteert u het menu **Bestand** en vervolgens de optie **Gegevens ophalen**.
3. Selecteer op de pagina **Gegevens ophalen** de optie **Onlineservices**.
4. Voer in het deelvenster **Onlineservices** een van de volgende stappen uit:

    - Om verbinding te maken met [!INCLUDE [prod_short](includes/prod_short.md)] online selecteert u **Dynamics 365 Business Central** en dan **Verbinden**.
    <!--- To connect to  [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, select **Dynamics 365 Business Central (on-premises)**, then **Connect**.-->

5. Meld u aan bij [!INCLUDE [prod_short](includes/prod_short.md)] (eenmalig).

    Als u zich niet hebt aangemeld bij [!INCLUDE [prod_short](includes/prod_short.md)] vanuit Power BI Desktop, wordt u gevraagd zich aan te melden.

    - Voor [!INCLUDE [prod_short](includes/prod_short.md)] online selecteert u **Aanmelden** en kiest u het relevante account. Gebruik hetzelfde account dat u gebruikt om u aan te melden bij [!INCLUDE [prod_short](includes/prod_short.md)]. Wanneer u klaar bent, selecteert u **Verbinden**.

    <!--- For [!INCLUDE [prod_short](includes/prod_short.md)] on-premises, first enter the OData URL for [!INCLUDE[prod_short](includes/prod_short.md)], then select **OK**. When prompted, enter the user name and password of the account to use for connecting to [!INCLUDE[prod_short](includes/prod_short.md)]. In the **Password** box, enter the web service access key. When done, select **Connect**.-->

    > [!NOTE]  
    > Nadat u verbinding hebt gemaakt met [!INCLUDE[prod_short](includes/prod_short.md)], wordt u niet opnieuw gevraagd om in te loggen. [Hoe wijzig of wis ik het account dat ik momenteel gebruik om verbinding te maken met Business Central vanuit Power BI Desktop?](/dynamics365/business-central/power-bi-faq?tabs=designer#perms)

6. Wanneer verbonden, neemt Power BI contact op met de [!INCLUDE [prod_short](includes/prod_short.md)]-service. Het **navigatie**venster verschijnt en toont de beschikbare gegevensbronnen voor het maken van rapporten. Selecteer een map om deze uit te vouwen en de beschikbare gegevensbronnen te bekijken.

   Deze gegevensbronnen vertegenwoordigen alle webservices en API-pagina's die zijn gepubliceerd vanuit [!INCLUDE [prod_short](includes/prod_short.md)], gegroepeerd op omgevingen en bedrijven. Met [!INCLUDE [prod_short](includes/prod_short.md)] online heeft **Navigator** de volgende opbouw:

    - **Omgevingsnaam**
      - **Bedrijfsnaam**
        - **Geavanceerde API's**

          Deze map bevat geavanceerde API-pagina's die door Microsoft zijn gepubliceerd, zoals de [API's voor Business Central-automatisering](/dynamics365/business-central/dev-itpro/administration/itpro-introduction-to-automation-apis) en [aangepaste API-pagina's voor Business Central](/dynamics365/business-central/dev-itpro/developer/devenv-develop-custom-api). Aangepaste API-pagina's zijn verder gegroepeerd in mappen volgens de eigenschappen [APIPublisher](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apipublisher-property)/[APIGroup](/dynamics365/business-central/dev-itpro/developer/properties/devenv-apigroup-property) van de broncode van de API-pagina.

        - **Standaard API's v2.0**

          Deze map bevat de API-pagina's die worden weergegeven door de [Business Central API V2.0](/dynamics365/business-central/dev-itpro/api-reference/v2.0/).

        - **Webservices \(legacy)**

          Deze map bevat pagina's, codeunits en query's die zijn gepubliceerd als webservices in Business Central.

    <!--
    > [!NOTE]
    > The structure for Business Central on-premises is different because it doesn't support API pages.-->

7. Selecteer de gegevensbron of -bronnen die u aan uw gegevensmodel wilt toevoegen en selecteer vervolgens de knop **Laden**.
8. Als u later meer Business Central-gegevens wilt toevoegen, kunt u de vorige stappen herhalen.

Zodra de gegevens zijn geladen, ziet u deze in de rechternavigatie op de pagina. U hebt nu met succes verbinding gemaakt met uw [!INCLUDE[prod_short](includes/prod_short.md)]-gegevens en u kunt uw Power BI-rapport gaan maken.  

> [!TIP]
> Zie [Aan de slag met Power BI Desktop](/power-bi/fundamentals/desktop-getting-started) voor meer informatie over het gebruik van Power BI Desktop.

## <a name="creating-accessible-reports"></a>Toegankelijke rapporten maken

Het is belangrijk om uw rapporten bruikbaar te maken voor zoveel mogelijk mensen. Probeer rapporten zo te ontwerpen dat ze geen speciale aanpassingen nodig hebben om aan specifieke behoeften van verschillende gebruikers te voldoen. Zorg ervoor dat gebruikers dankzij het ontwerp kunnen profiteren van standaard ondersteunende technologieën, zoals schermlezers. Power BI bevat verschillende toegankelijkheidsfuncties, tools en richtlijnen om dit doel te bereiken. Zie voor meer informatie [Power BI-rapporten voor toegankelijkheid](/power-bi/create-reports/desktop-accessibility-creating-reports) in de Power BI-documentatie.

## <a name="creating-reports-to-display-data-associated-with-a-list"></a>Rapporten maken om gegevens weer te geven die aan een lijst zijn gekoppeld

U kunt rapporten maken die worden weergegeven in een feitenblok van een [!INCLUDE [prod_short](includes/prod_short.md)]-lijstpagina. De rapporten kunnen gegevens bevatten over de record die in de lijst is geselecteerd. U kunt deze rapporten op ongeveer dezelfde manier maken als andere rapporten, maar u moet wel een paar dingen doen om ervoor te zorgen dat de rapporten worden weergegeven zoals verwacht. Zie [Power BI-rapporten maken voor het weergeven van lijstgegevens in [!INCLUDE[prod_short](includes/prod_short.md)]](across-how-use-powerbi-reports-factbox.md) voor meer informatie.

## <a name="using-the--report-theme-optional"></a><a name="theme"></a>Het [!INCLUDE [prod_short](includes/prod_short.md)]-rapportthema gebruiken (optioneel)

U wordt aangeraden om voordat u uw rapport maakt het [!INCLUDE [prod_short](includes/prod_short.md)]-themabestand te downloaden en importeren. Het themabestand maakt een kleurenpalet, zodat u rapporten kunt maken met dezelfde kleurstijl als de [!INCLUDE [prod_short](includes/prod_short.md)]-apps zonder dat u aangepaste kleuren hoeft te definiëren voor elk visueel element.

> [!NOTE]
> Deze taak is optioneel. U kunt altijd uw rapporten maken en later alsnog de stijlsjabloon downloaden en toepassen.

### <a name="download-the-theme"></a>Het thema downloaden

Het themabestand is beschikbaar als JSON-bestand in de themagalerij van de Microsoft Power BI-community. Voer de volgende stappen uit om het themabestand te downloaden:

1. Ga naar de themagalerij van de [Microsoft Power BI-community voor Microsoft Dynamics 365 Business Central](https://community.powerbi.com/t5/Themes-Gallery/Microsoft-Dynamics-365-Business-Central/m-p/385875).
2. Selecteer de downloadbijlage **Microsoft Dynamics Business Central.json**.

### <a name="import-the-theme-on-a-report"></a>Het thema in een rapport importeren

Nadat u het [!INCLUDE [prod_short](includes/prod_short.md)]-rapportthema hebt gedownload, kunt u het in uw rapporten importeren. Als u het thema wilt importeren, selecteert u **Weergave** > **Thema's** > **Thema's zoeken**. Zie [Power BI Desktop - aangepaste rapportthema's importeren](/power-bi/create-reports/desktop-report-themes#import-custom-report-theme-files) voor meer informatie.

## <a name="publish-reports"></a>Rapporten publiceren

Nadat u een rapport hebt gemaakt of gewijzigd, kunt u het rapport publiceren naar uw Power BI-service en delen met anderen in uw organisatie. Nadat u een rapport heeft gepubliceerd, is het beschikbaar in Power BI. Het rapport kan ook worden geselecteerd in [!INCLUDE[prod_short](includes/prod_short.md)].

Als u een rapport wilt publiceren, selecteert u **Publiceren** op het tabblad **Start** of in het menu **Bestand**. Als u bent aangemeld bij de Power BI-service, wordt het rapport naar deze service gepubliceerd. Als dat niet het geval is, wordt u gevraagd u aan te melden. 

## <a name="distribute-or-share-a-report"></a>Een rapport distribueren of delen

Er zijn een aantal manieren om rapporten beschikbaar te maken voor uw collega's en anderen:

- U kunt rapporten distribueren als PBIX-bestanden.

    Rapporten worden op uw computer opgeslagen als PBIX-bestanden. U kunt het PBIX-rapportbestand net als elk ander bestand onder gebruikers distribueren. Vervolgens kunnen gebruikers het bestand uploaden naar hun Power BI-service. Zie [Rapporten uploaden vanuit bestanden](across-working-with-powerbi.md#upload).

    > [!NOTE]
    > Als u een rapport op deze manier distribueert, houdt dat in dat iedere gebruiker afzonderlijk de gegevens van dat rapport moet vernieuwen. Deze situatie kan van invloed zijn op de prestaties van [!INCLUDE[prod_short](includes/prod_short.md)].

- Het rapport delen vanuit uw Power BI-service

    Als u een Power BI Pro-licentie hebt, kunt u het rapport rechtstreeks vanuit uw Power BI-service delen met anderen. Zie [Power BI - een dashboard of rapport delen](/power-bi/collaborate-share/service-share-dashboards#share-a-dashboard-or-report) voor meer informatie.

## <a name="how-to-develop-cross-company-or-cross-environment-power-bi-reports"></a>Power BI-rapporten voor meerdere bedrijven of omgevingen maken

De [!INCLUDE[prod_short](includes/prod_short.md)] API-eindpunten hebben allemaal het voorvoegsel `https://api.businesscentral.dynamics.com/v2.0/<environment_name>/api/v2.0`, gevolgd door `/companies({company_id})/accounts({id})` (hier gebruiken we de `accounts` API als illustratie). U kunt deze structuur gebruiken om PowerQuery-query's te maken die gegevens laden voor meerdere bedrijven of meerdere omgevingen als de gebruiker die gegevens leest, er toegang toe heeft.

Volg deze stappen om een query in te stellen om gegevens voor meerdere bedrijven te laden:

1. Neem de PowerQuery-query waarmee gegevens voor één bedrijf worden geladen. Converteer het naar een aangepaste Power Query-functie die de bedrijfs-id (of misschien de omgevingsnaam) als parameters gebruikt. Ga voor meer informatie naar [Aangepaste Power Query-functies gebruiken](/power-query/custom-function).
1. Gebruik nu de nieuwe aangepaste functie in een PowerQuery-query, waarbij u de functie toewijst aan een lijst met bedrijven en vervolgens de gegevenssets samenvoegt met behulp van de functie [Table.Combine](/powerquery-m/table-combine) Power Query.

## <a name="fixing-problems"></a>Problemen oplossen

### <a name="cant-insert-a-record-current-connection-intent-is-read-only-error-connecting-to-custom-api-page"></a>"Kan geen record invoegen. De huidige verbindingsintentie is alleen-lezen." fout bij het verbinden met aangepaste API-pagina

> **VAN TOEPASSING OP:** Business Central online

Vanaf februari 2022 maken nieuwe rapporten die gebruikmaken van [!INCLUDE [prod_short](includes/prod_short.md)]-gegevens, standaard verbinding met een alleen-lezen replica van de [!INCLUDE [prod_short](includes/prod_short.md)]-database. In zeldzame gevallen, afhankelijk van het paginaontwerp, kunt u een foutmelding krijgen wanneer u verbinding probeert te maken en gegevens van de pagina probeert op te halen.

1. Start Power BI Desktop.
2. Selecteer op het lint **Gegevens ophalen** > **Onlineservices**.
3. Selecteer in het deelvenster **Onlineservices** **Dynamics 365 Business Central** en dan **Verbinden**.
4. Selecteer in het venster **Navigator** het API-eindpunt waaruit u gegevens wilt laden.
5. Het voorbeeldvenster toont de volgende fout:

   *Dynamics365BusinessCentral: Aanvraag mislukt: de externe server heeft een fout geretourneerd: (400) Ongeldige aanvraag. (Kan geen record invoegen. Huidige verbindingsintentie is Alleen-lezen. CorrelationId: [...])".*

6. Selecteer **Gegevens transformeren** in plaats van **Laden** zoals u normaal zou doen.
7. Selecteer in de **Power Query-editor** **Geavanceerde editor** vanaf het lint.
8. Vervang op de regel die begint met **Source =**, de volgende tekst:

   ```
   Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, null)
   ```

   door:

   ```
   Dynamics365BusinessCentral.ApiContentsWithOptions(null, null, null, [UseReadOnlyReplica = false])
   ```

9. Selecteer **Gereed**.
10. Selecteer **Sluiten en toepassen** op het lint om de wijzigingen op te slaan en de Power Query-editor te sluiten.

## <a name="see-also"></a>Zie ook

[Uw bedrijfsgegevens inschakelen voor Power BI](admin-powerbi-setup.md)  
[Bedrijfsinformatie](bi.md)  
[Voorbereid zijn om zaken te doen](ui-get-ready-business.md)  
[Bedrijfsgegevens importeren uit andere financiële systemen](across-import-data-configuration-packages.md)  
[Instellen van [!INCLUDE[prod_short](includes/prod_short.md)]](setup.md)  
[Financiën](finance.md)  
[Snelle start: Uw gegevens verbinden in Power BI Desktop](/power-bi/desktop-quickstart-connect-to-data)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
