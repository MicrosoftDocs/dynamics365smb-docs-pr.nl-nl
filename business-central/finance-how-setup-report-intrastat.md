---
title: Intrastat instellen en rapporteren| Microsoft Docs
description: Leren hoe u Intrastat-rapportagefuncties instelt en hoe u handel rapporteert met bedrijven in andere EU-landen/regio's.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: electronic document, Intrastat, trade, EU, European Union
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: c72d5beafde357c22fac396eb3ab76849a9df775
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775497"
---
# <a name="set-up-and-report-intrastat"></a>Intrastat instellen en rapporteren
Bedrijven uit EU-landen moeten handel met bedrijven uit andere landen/regio's in de EU rapporteren. In uw land/regio moet u de beweging van goederen elke maand doorgeven aan de autoriteiten en moet aangifte bij de belastingdienst worden gedaan. Dit wordt Intrastat-rapportage genoemd. U gebruikt de pagina **Intrastat-dagboek** om periodieke Intrastat-rapporten te voltooien.  

## <a name="required-and-optional-setups"></a>Vereiste en optionele instellingen
Voordat u het Intrastat-dagboek kunt gebruiken om Intrastat-gegevens te rapporteren, moet u meerdere zaken instellen:  

* **Intrastat-instellingen**: de pagina Intrastat-instellingen wordt gebruikt om Intrastat-rapportage in te schakelen en er standaarden voor in te stellen. U kunt opgeven of u Intrastat moet rapporteren vanuit verzendingen, ontvangsten (aankomsten) of beide, afhankelijk van drempelwaarden die door uw lokale verordeningen zijn ingesteld. U kunt ook standaardtransactiesoorten instellen voor normale en retourdocumenten, die worden gebruikt voor de aard van transactierapportage.
* **Intrastat-dagboeksjablonen**: u moet de Intrastat-dagboeksjablonen en -batches instellen die u gaat gebruiken. Aangezien Intrastat maandelijks wordt gerapporteerd, moet u 12 Intrastat-dagboekbatches maken die gebaseerd zijn op dezelfde sjabloon.  
* **Basisproductcodes**: de belastingdienst en de douane hebben numerieke codes om artikelen en service te classificeren. U geeft deze codes op voor artikelen.
* **Transactieaardcode**: landen/regio's hebben verschillende codes voor soorten Intrastat-transacties, zoals de gewone inkoop en verkoop, het ruilen van geretourneerde goederen en het ruilen van niet-geretourneerde goederen. Alle codes instellen die van toepassing zijn op uw land of regio. U gebruikt deze codes in verkoop- en inkoopdocumenten, en bij de verwerking van retouren.  
* **Transportmethoden**: er zijn zeven eencijferige codes voor Intrastat-transportmethoden. **1** voor zee, **2** voor spoor, **3** voor weg, **4** voor lucht, **5** voor post, **7** voor vaste installaties en **9** voor eigen voortdrijving (bijvoorbeeld een auto verplaatsen door ermee te rijden). [!INCLUDE[prod_short](includes/prod_short.md)] vereist deze codes niet, maar we raden aan dat de beschrijvingen een soortgelijke betekenis hebben.  

Eventueel kunt u ook het volgende instellen:

* **Transactieomschrijvingen**: gebruik deze als aanvulling op de omschrijvingen van de transactiesoorten.  
* **Districten**: gebruik deze om extra informatie te geven over landen/regio's.  
* **Invoer-/uitvoerhavens**: gebruik deze om de vestigingen op te geven waar u artikelen naar wilt verzenden of wilt ontvangen naar of uit andere landen/regio's. De luchthaven Heathrow is een voorbeeld van een invoer-/uitvoerhaven. U voert invoer- of uitvoerhavens in op verkoop- of inkoopdocumenten op het sneltabblad **Buitenlandse handel**. Deze gegevens worden tevens gekopieerd van de artikelposten wanneer u het Intrastat-dagboek maakt.  

### <a name="to-set-up-intrastat-templates-and-batches"></a>Intrastat-sjablonen en -batches instellen
De Intrastat-batchtaken bevatten alleen artikelposten en geen grootboekposten. Als u grootboekposten hebt die in aanmerking komen voor Intrastat-rapportage, moet u deze handmatig invoeren. Als u bijvoorbeeld vanuit een ander EU-land/regio een computer aanschaft, wordt de computer niet in de voorraad geplaatst, maar geboekt op een grootboekrekening. U moet handmatig dit soort post invoeren in het Intrastat-dagboek.  

U kunt de posten exporteren naar een bestand dat u aan de Intrastat-autoriteiten kunt verzenden. U kunt ook een rapport afdrukken, handmatig de informatie invoeren op de formulieren van uw autoriteiten en vervolgens de informatie indienen.

> [!Note]
> Wij raden u aan voor elke maand een Intrastat-dagboekbatch in te stellen.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-dagboeksjablonen** in en kies de desbetreffende koppeling.  
2. Vul indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]. Een sjabloon maken voor elk Intrastat-formulier dat u gebruikt.  
3. Als u batches wilt maken, kiest u de actie **Batches**.  
4. Vul de vereiste velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]. Een sjabloon maken voor elk Intrastat-formulier dat u gebruikt. 

> [!Note]
> In het veld **Statistiekperiode** voert u de statistiekperiode in als getal met vier cijfers. De eerste twee cijfers duiden het jaar aan, de laatste twee cijfers de maand. U kunt bijvoorbeeld 1706 invoeren voor juni 2017.

### <a name="to-set-up-commodity-codes"></a>Basisproductcodes instellen
Alle artikelen die u koopt of verkoopt moeten een basisproductcode hebben.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Basisproductcodes** in en kies de desbetreffende koppeling.  
2. Vul de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  
3. Als u een basisproductcode aan een artikel wilt toewijzen, gaat u naar de pagina **Artikel**, vouwt u het sneltabblad **Kosten en boeking** uit en voert u de code in het veld **Basisproductcode** in.   

### <a name="to-set-up-transaction-nature-codes"></a>Transactieaardcodes instellen
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transactieaardcodes** in en kies de desbetreffende koppeling.  
2. Vul de velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]  

> [!Tip]
> Als u vaak een bepaalde transactieaardcode gebruikt, kunt u van deze code de standaardcode maken. Hiervoor gaat u naar de pagina **Intrastat-instellingen** en kiest u de code.

### <a name="to-set-up-transport-methods"></a>Transportmethoden instellen
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Transportmethodes** in en kies de desbetreffende koppeling.  
2. Vul de benodigde velden in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

### <a name="to-set-up-which-intrastat-report-fields-are-mandatory"></a>Instellen welke Intrastat-rapportvelden verplicht zijn
In sommige landen/regio's, zoals Spanje en het Verenigd Koninkrijk, vereist de belastingdienst dat Intrastat-rapporten bijvoorbeeld de verzendmethode bevatten voor inkopen of andere waarden wanneer de verkoop boven een bepaalde drempel ligt. Op de pagina **Intrastat-instelling** kunt u selecteren dat **Intrastat-controlelijst instellen** verplichte velden instelt op de pagina **Intrastat-dagboek**.

1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-instellingen** in en kies de desbetreffende koppeling.
2. Kiest de actie **Intrastat-controlelijst instellen**.
3. Klik op de pagina **Intrastat-controlelijst instellen** op **Veldnaam** om het Intrastat-rapportveld te kiezen dat u verplicht wilt maken.

## <a name="to-report-intrastat"></a>Intrastat rapporteren
Nadat u het Intrastat-dagboek hebt ingevuld, kunt u het rapport **Controlelijstrapport** uitvoeren om te zorgen dat alle gegevens in het dagboek correct zijn. Verplichte velden die u op de pagina **Intrastat-controlelijst instellen** hebt ingesteld en waarvoor waarden ontbreken, worden weergegeven in het feitenblok Fouten en waarschuwingen op de pagina **Intrastat-dagboek**. Vervolgens kunt u een Intrastat-rapport afdrukken als formulier of een bestand maken om naar de belastingdienst in uw land of regio te verzenden.  

### <a name="to-fill-in-intrastat-journals"></a>Intrastat-dagboeken invullen  
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-dagboek** in en kies de desbetreffende koppeling.  
2. Kies op de pagina **Intrastat-dagboek** de relevante dagboekbatch in het veld **Batchnaam** en kies **OK**.  
3. Kies de actie **Regels voorstellen**. In de velden **Begindatum** en **Einddatum** zijn al de datums opgenomen die voor de statistiekperiode in de dagboekbatch zijn opgegeven.  
4. U kunt een percentage voor transport en verzekering opgeven in het veld **Indirecte kosten %**. Als u een percentage opgeeft, wordt de inhoud van het veld **Statistiekwaarde** verhoudingsgewijs aangepast op basis van dit percentage.  
5. Kies **OK** om de batchverwerking te starten.  

Met de batchverwerking worden alle artikelposten in de statistiekperiode opgehaald en als regels in het Intrastat-dagboek ingevoegd. U kunt de regels zo nodig bewerken.  

> [!IMPORTANT]  
>  Tijdens de batchverwerking worden alleen de posten met een land-/regiocode opgehaald waarvoor u een Intrastat-code hebt ingevoerd op de pagina **Landen/regio's**. Het is dus belangrijk dat u Intrastat-codes invoert voor de land-/regiocodes waarvoor u de batchverwerking wilt uitvoeren.  

### <a name="report-intrastat-on-a-form-or-a-file"></a>Intrastat rapporteren in een formulier of een bestand
Als u de gegevens wilt ophalen die nodig zijn op het Intrastat-formulier van de betreffende instanties voor statistiekbeheer, moet u de lijst **Intrastat - Formulier** afdrukken. Voordat u dit kunt doen, moet u het Intrastat-dagboek voorbereiden en invullen. Als u zowel verkoop- als inkooptransacties hebt, moet u een apart formulier invullen voor elke soort. U moet de lijst dus tweemaal afdrukken.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-dagboeken** in en kies de desbetreffende koppeling.  
2. Kies op de pagina **Intrastat-dagboek** de relevante dagboekbatch in het veld **Batchnaam**.  
3. Als u dit nog niet hebt gedaan, vult u het journaal handmatig in of kiest u de actie **Regels voorstellen**.  
4. Kies de actie **Hiermee wordt het Intrastat-dagboek afgedrukt**.  
5. Voeg een filter **Soort** toe in het sneltabblad **Intrastat-dagboekregel** en geef op of dit een **Ontvangst** of **Verzending** is.  
6. Kies **Verzenden** om het rapport af te drukken.  

### <a name="report-intrastat-in-a-file"></a>Intrastat in een bestand rapporteren
U kunt het Intrastat-rapport indienen als bestand. Voordat u het bestand maakt, kunt u een controlelijst afdrukken met dezelfde gegevens als in het bestand.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-dagboek** in en kies de desbetreffende koppeling.  
2. Selecteer op de pagina **Intrastat-dagboek** de relevante dagboekbatch in het veld **Batchnaam**.  
3. Als u dit nog niet hebt gedaan, vult u het journaal handmatig in of kiest u de actie **Regels voorstellen**.  
4. Kies de actie **Bestand maken**.  
5. Kies de knop **OK** op de pagina voor de batchtaak.  
6. Kies **Opslaan**.  
7. Blader naar de locatie waar u het bestand wilt opslaan, voer de bestandsnaam in en kies **Opslaan**.

## <a name="reorganize-intrastat-journals"></a>Intrastat-dagboeken opnieuw indelen
Aangezien u elke maand een Intrastat-rapport moet indienen en u voor elk rapport een nieuwe dagboekbatch maakt, hebt u na verloop van tijd veel dagboekbatches. De dagboekregels worden niet automatisch verwijderd. U wilt de dagboekbatchnamen mogelijk periodiek wijzigen. Hiervoor verwijdert u de dagboekbatches die u niet meer gebruikt. De dagboekregels in deze batches worden ook verwijderd.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Intrastat-dagboeken** in en kies de desbetreffende koppeling.  
2. Als u de opties wilt zien, kiest u het veld **Batchnaam**.  
3. Kies de journaalbatches die u wilt verwijderen en kies de knop **Verwijderen**.  

## <a name="tariff-numbers"></a>Tariefcodes

In veel landen/regio's hanteren de belastingdienst en de douane goederencodes van acht tekens voor verschillende artikelen. Om te zorgen dat artikelposten de benodigde informatie bevatten wanneer het programma ze importeert naar de Intrastat-dagboekregel, moet u de informatie hebben ingevoerd over de tariefcode op de pagina **Tariefcodes**. Zoek de codes voor de artikelen waar uw bedrijf in handelt en geef ze op de pagina **Tariefcodes** op.

Voeg op de pagina **Tariefcodes** alle codes toe die u gebruikt. U moet de codes invoeren op de artikelkaart voordat u kunt beginnen met boeken. Als u de codes hebt ingesteld, voert u ze in het veld **Tariefnr.** op de artikelkaart in. U moet ook het veld **Nettogewicht** op de artikelkaart invullen.

## <a name="see-related-training-at-microsoft-learn"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/process-intrastat-dynamics-365-business-central/index)

## <a name="see-also"></a>Zie ook
[Financieel beheer](finance.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]