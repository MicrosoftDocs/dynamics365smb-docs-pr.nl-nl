---
title: Duurzaamheidsposten vastleggen
description: Leer hoe u uitstoot van broeikasgassen vastlegt.
author: altotovi
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'Sustainability, ESG, emission, GHG, CSRD, journal'
ms.search.form: '6216, 6219, 6220'
ms.date: 08/19/2024
ms.author: altotovi
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# Duurzaamheidsposten vastleggen

Gebruikers kunnen de uitstoot van broeikasgassen handmatig registreren in het duurzaamheidsboek met behulp van duurzaamheidsdagboeken of andere inkoopgerelateerde documenten.  

> [!NOTE]
> Vanaf 2024 is het mogelijk om alle soorten aankoopgerelateerde documenten te gebruiken om de uitstoot van broeikasgassen (BKG) te registreren *.*  

## Duurzaamheidsdagboeken

Duurzaamheidsdagboeken zijn ontworpen om duurzaamheidsgerelateerde activiteiten bij te houden en vast te leggen met behulp van dezelfde gebruikerservaring als andere dagboeken in Business Central. Gebruikers die over de benodigde informatie beschikken, kunnen uitstoot handmatig in een journaal invoeren. Als ze de gegevens niet hebben, kunnen ze ook ingebouwde formules gebruiken om de uitstoot nauwkeurig te berekenen op basis van specifieke bekende parameters die overeenkomen met verschillende soorten bronnen en rekeningen.

De informatie die u invoert in een dagboek is tijdelijk en kan in dat dagboek worden gewijzigd. Wanneer u het dagboek boekt, wordt de informatie overgebracht naar duurzaamheidsposten op afzonderlijke duurzaamheidsrekeningen, waar deze niet kunnen worden gewijzigd. U kunt echter wel tegenboekingen of correcties boeken.

### Dagboeksjablonen en -batches gebruiken

Er zijn standaard twee duurzaamheidsdagboeksjablonen: de standaardsjabloon en de periodieke.

Voor elke dagboeksjabloon kunt u uw eigen persoonlijke dagboek instellen als een dagboekbatch. Om dit te doen moet u de actie **Batches** op de pagina **Sjablonen van duurzaamheidsdagboek** kiezen en de nieuwe **duurzaamheidsdagboekbatch** op de nieuwe pagina maken. U kunt bijvoorbeeld voor elk uitstootbereik uw eigen dagboekbatch definiëren met behulp van de optie **Uitstootbereik**, en selecteren uit de drie bestaande bereiken. U kunt ook de **Broncode** en **Redencode** voor elk van de batches toevoegen of wijzigen.

> [!TIP]
> Als u veel regels heeft, kunt u het risico op fouten helpen verkleinen door voor elk uitstoottype één dagboekbatch te hebben. Als alternatief kunt u voor alle uitstoottypen de gemeenschappelijke batch gebruiken.

### Duurzaamheidsdagboeken valideren

U kunt op de pagina **Duurzaamheidsinstelling** een achtergrondcontrole inschakelen om vertragingen bij het boeken te voorkomen. Als er fouten optreden terwijl u in het duurzaamheidsjournaal werkt, wordt u hiervan door de validatie op de hoogte gesteld en wordt voorkomen dat u het dagboek kunt boeken.

Wanneer u de validatie inschakelt, toont het feitenblok **Dagboekcontrole** problemen op de huidige regel en in de hele batch. Validatie vindt plaats wanneer u een dagboekbatch laadt en wanneer u een andere dagboekregel kiest. De tegel **Totaal aantal problemen** in het feitenblok toont het totale aantal problemen dat [!INCLUDE [prod_short](includes/prod_short.md)] heeft gevonden. U kunt de tegel selecteren om een overzicht van de problemen te openen.

### Werken met duurzaamheidsdagboeken

Om met duurzaamheidstijdschriften te werken, volg je de stappen van volgen:

1. Selecteer het ![Lampje dat de functie Vertel me opent 3.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Duurzaamheidsdagboek** in en selecteer vervolgens de gerelateerde koppeling.
2. Op de pagina **Duurzaamheidsdagboek** kunt u zoveel regels invoeren als u van plan bent in dezelfde batch te boeken.
3. U kunt het veld **Documentsoort** leeg laten of u kunt **Factuur** of **Creditnota** selecteren.
4. In het veld **Rekeningnr.** kunt u alleen niet-geblokkeerde duurzaamheidsrekeningen selecteren waarvan het veld **Directe boeking** is geselecteerd en het **Rekeningtype** is ingesteld op **Boeking**. De rekeningen moeten ook zijn geconfigureerd met een categorie en een subcategorie.

    > [!NOTE]
    > Als u een batch gebruikt waar het uitstootbereik is geconfigureerd, moet het **Uitstootbereik** in de duurzaamheidsrekening gelijk zijn aan het **Uitstootbereik** in de gebruikte batch.

5. U kunt de bedragen handmatig boeken of formules gebruiken.

    - Als u over nauwkeurige informatie over de uitstoot beschikt en deze wilt boeken (dat wil zeggen dat u de informatie op de ontvangen factuur hebt), moet u het veld **Handmatige invoer** selecteren om aan te geven dat u de bedragen handmatig invoert. In dit geval kunt u uw gegevens niet rechtstreeks invoeren in de velden **Brandstof/elektriciteit**, **Afstand**, **Aangepast bedrag**, **Installatievermenigvuldiger** en **Tijdfactor**, omdat ze niet-bewerkbaar worden. Maar de velden **Uitstoot CO2**, **Uitstoot CH4** en **Uitstoot N2O** blijven bewerkbaar en u kunt uw gegevens daar rechtstreeks in invoeren.
    - Als u geen nauwkeurige kennis heeft van de uitstoot en deze moet berekenen, selecteer dan niet het veld **Handmatige invoer**. In dit geval worden de velden **Uitstoot CO2**, **Uitstoot CH4** en **Uitstoot N2O** niet-bewerkbaar. U kunt echter uw berekeningsgegevens invoeren op basis van de formule die u gebruikt. Meer informatie over de gebruikte formules die worden gedefinieerd in de **duurzaamheidsrekeningcategorie** vindt u in [Diagram van duurzaamheidsrekeningschema en -grootboek](finance-sustainability-accounts-ledger.md#account-categories).

6. Kies de actie **Boeken** om het dagboek te boeken. Wanneer u boekt in een duurzaamheidsdagboek, worden posten gegenereerd in het duurzaamheidsgrootboek.

Als uw formule is gebaseerd op de optie **Berekenen op basis van grootboek** in de duurzaamheidsrekeningcategorie, moet u de actie **Bedrag van grootboekposten innen** gebruiken voordat u het dagboek boekt om de uitstoot te berekenen op basis van deze gegevensbron. Als u na het invullen van de dagboekregels wijzigingen in de uitstootfactoren heeft aangebracht, moet u ook de actie **Herberekenen** kiezen om het juiste bedrag in het dagboek te krijgen.

### Periodieke dagboeken

Een periodiek dagboek is een duurzaamheidsdagboek met specifieke velden voor het beheer van transacties die u vaak boekt met weinig of geen wijzigingen. Voorbeelden omvatten duurzaamheidstransacties zoals elektriciteit, warmte of andere soortgelijke transacties. Met periodieke dagboeken kunt u vaste en variabele bedragen boeken.

Wanneer u een periodiek dagboek gebruikt, maakt u posten die u regelmatig boekt, slechts eenmaal. Informatie zoals de rekeningen, dimensies en dimensiewaarden worden na het boeken in het dagboek bewaard. Elke keer dat u boekt, kunt u benodigde wijzigingen aanbrengen.

Het veld **Periodieke methode** is belangrijk. Het bepaalt hoe het bedrag op de dagboekregel na het boeken wordt behandeld. Als u bijvoorbeeld elke keer dat u de regel boekt hetzelfde bedrag gebruikt, kunt u de optie **V Vast** selecteren om het bedrag na boeking te behouden. Als u dezelfde rekeningen en dezelfde tekst op de regel wilt gebruiken, maar het bedrag elke keer dat u boekt varieert, kunt u de optie **Variabel** selecteren om het bedrag na boeking te verwijderen.

Het veld **Periodieke frequentie** is ook belangrijk en moet worden ingesteld. Het is een datumformuleveld dat bepaalt hoe vaak de post op de dagboekregel wordt geboekt. Zie voor meer informatie [Datumformules gebruiken](ui-enter-date-ranges.md#use-date-formulas).

De **Vervaldatum** bepaalt de datum waarop de regel voor het laatst wordt geboekt. De regel wordt niet geboekt na deze datum. Voordeel van gebruik van het veld **Vervaldatum** is dat de regel niet onmiddellijk uit het dagboek wordt verwijderd. U kunt een latere datum invoeren, zodat u de regel in de toekomst kunt gebruiken. Als het veld leeg is, wordt de regel steeds geboekt totdat deze uit het dagboek wordt verwijderd.

## Inkoopdocumenten  

Om de registratie van broeikasgasemissies (BKG) in inkoopdocumenten mogelijk te maken, moet u op de pagina  **Duurzaamheidsinstellingen**  de optie  **Emissies gebruiken in inkoopdocumenten**  selecteren.  

Om met aankoopgerelateerde documenten te werken, volgt u de volgende stappen: volgen

1. Selecteer het ![Lampje dat de functie Vertel me opent 3.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), Pictogram en:  
   1. Voer  **Aankoopfacturen** in als u de factuur als  **documenttype** wilt verzenden en selecteer vervolgens de gerelateerde koppelen.  
   2. Voer  **Inkooporders** in als u wilt bestellen als **documenttype** en selecteer vervolgens de gerelateerde koppelen.  
2. Vul de koptekst en regels in op basis van de volgende instructies:  [hoe u met inkoopfacturen en orders werkt](purchasing-how-record-purchases.md).
3. Als u informatie over emissies op de factuur van uw leverancier hebt, selecteert u het juiste **Duurzaamheidsrekeningnummer** in de regels van het document en voegt u emissiewaarden toe met behulp van een van de volgende velden (op basis van wat u wilt bijhouden en de emissies die op uw fysieke factuur staan): **Emissie CO2**, **Emissie CH4** of **Emissie N2O**.

    > [!NOTE]
    > De waarden die u in de emissievelden invoert, zijn vaste bedragen per regel en worden niet vermenigvuldigd met het veld  **hoeveelheid** . U kunt  **Duurzaamheidsrekeningnr.** alleen gebruiken als het **veld** Type **(Optiewaarden**) **Artikel** of **G/L-rekening** is. U kunt geen **Resource** of **Charge (Item)** **Optiewaarden** gebruiken. 

4. Als u de totale emissies wilt zien voordat u ze boekt, kunt u de statistiekenpagina openen en de totale geboekte emissies en emissies voor het boeken per document (alle aankoopgerelateerde documenten) vinden op het sneltabblad  **Duurzaamheid** .   
5. Verstuur de documenten en open een nieuwe **geboekte inkoopfactuur**.
6. Selecteer de actie **Posten zoeken** en u zult zien dat u **Duurzaamheidspost** als een van de gerelateerde posten op de pagina **Posten zoeken** hebt.

> [!NOTE]
> Wanneer u het document boekt, zal het systeem voor elke inkoopregel waarvoor u een  **Duurzaamheidsrekeningnummer** hebt, een onafhankelijke **Duurzaamheidsgrootboekpost** aanmaken met de **Factuur** als **documenttype** en hetzelfde **documentnummer.**

> [!NOTE]
> U kunt ook een **aankoopcreditnota** maken en boeken. U kunt dit handmatig doen of een van de volgende opties gebruiken: **Annuleren**, **Corrigeren** of **Corrigerende creditnota maken** . In dat geval kopieert het systeem de bestaande waarden van de geboekte factuur.  

## Zie ook

[Financiën](finance.md)    
[Overzicht van duurzaamheidsbeheer](finance-manage-sustainability.md)    
[Duurzaamheidsopstelling](finance-sustainability-setup.md)    
[Duurzaamheidsrekeningschema en -grootboek](finance-sustainability-accounts-ledger.md)    
[Adhoc-analyse van duurzaamheidsgegevens](ad-hoc-analysis-sustainability.md)    
[Duurzaamheidsrapporten en analyses in Business Central](sustainability-reports.md)   
[Duurzaamheid-API](/dynamics365/business-central/dev-itpro/api-sustainability/sustainability-api?toc=/dynamics365/business-central/toc.json)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)    

[!INCLUDE[footer-include](includes/footer-banner.md)]
