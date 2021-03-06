---
title: Cashflowanalyse instellen| Microsoft Docs
description: De grafieken in het rolcentrum Rekeningen instellen om de geldstroom in uw bedrijf te helpen analyseren, inclusief kosten en inkomsten, liquiditeit en kasontvangsten minus contante betalingen.
services: project-madeira
documentationcenter: ''
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: money flow, expense and income, liquidity, cash receipts minus cash payments, Cartera, funds
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: e197155f272d4435f838fbc67fb336f339c1a290
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783669"
---
# <a name="setting-up-cash-flow-analysis"></a>Cashflowanalyse instellen
Als u wat hulp wilt bij het bepalen wat u met uw contant geld moet doen, kunt de diagrammen bekijken in het rolcentrum Accountant:  

* **Cashcyclus**  
* **Inkomsten en uitgaven**  
* **Cashflow**  
* **Cashflowprognoses**  

In dit onderwerp wordt beschreven waar de gegevens in de diagrammen van afkomstig zijn en, indien nodig, wat u moet doen als u de diagrammen wilt gaan gebruiken.  
<br><br>  

> [!Video https://www.microsoft.com/en-us/videoplayer/embed/RE4mJhc?rel=0]

## <a name="the-cash-cycle-and-income--expense-charts"></a>De diagrammen Cashcyclus en Inkomsten en uitgaven
De diagrammen **Cashcyclus** en **Inkomsten en uitgaven** zijn gereed voor gebruik, gebaseerd op de rekeningschema's en rapportageschema´s. De rekeningen bevinden zich waar de gegevens uit afkomstig zijn en met rapportageschema´s wordt de relatie tussen verkopen en tegoeden berekend. Er worden enkele rekeningen en rapportageschema´s verschaft. U kunt deze ongewijzigd gebruiken, ze aanpassen en nieuwe toevoegen. Als u grootboekrekeningen toevoegt aan uw rekeningschema, bijvoorbeeld door deze te importeren uit QuickBooks, moet u een koppeling maken naar de rekeningen op de pagina **Rapportageschema´s** voor de volgende rapportageschemanamen:  

| Naam rapportschema | Waar het wordt gebruikt |
| --- | --- |
| **I_CACYCLE** |Cashcyclus |
| **I_CASHFLOW** |Cashflow |
| **I_INCEXP** |Inkomsten en uitgaven |
| **I_MINTRIAL** |Als resultatenrekening als u het rekeningschema niet gebruikt |

**Opmerking:** het is raadzaam de berekeningen te behouden die voor het rapportageschema worden verschaft.  

Voer rekeningen in het veld **Samentelling** voor **Totale opbrengsten**, **Totale tegoeden**, **Totaal schulden** en **Totale voorraad** in. Als u een koppeling wilt maken naar een bereik rekeningen of meer dan één specifieke rekening, voert u de rekeningnummers in die worden gescheiden door respectievelijk ".." of een verticale streep. Bijvoorbeeld **1111..4444** of **2222|3333|5555**.  

**Tip** controleer uw koppeling door de actie **Overzicht** te kiezen.  

## <a name="set-up-the-cash-flow-chart"></a>Het cashflowdiagram instellen
Het cashflowdiagram is gebaseerd op het volgende:  

* Een diagram van cashflowrekeningen.
* Een of meer cashflowinstellingen. Hiermee worden de rekeningen opgegeven die moeten worden gebruikt voor grootboek, inkoop, verkoop, services en vaste activa.  

Om u te helpen aan de slag te gaan zijn er enkele rekeningen en cashflowinstellingen verschaft. U kunt deze toevoegen, veranderen of verwijderen.  

Als u deze wilt instellen, kunt u zoeken naar **cashflowrekeningen**, de koppeling kiezen en vervolgens de velden invullen. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)] Herhaal deze stappen voor **cashflowinstellingen**.  

## <a name="set-up-cash-flow-forecasts"></a>Cashflowprognoses instellen
In het diagram **Cashflowprognose** worden cashflowrekeningen, cashflowinstellingen en cashflowprognoses gebruikt. Sommige worden verschaft, maar u kunt die van uzelf instellen met behulp van een begeleide instelling. Met de gids kunt u zaken opgeven zoals het aantal keren dat de prognose moet worden bijgewerkt, op welke rekeningen de prognose moet worden gebaseerd, wanneer u belastingen betaalt en of [Azure AI](https://azure.microsoft.com/overview/ai-platform/) moet worden ingeschakeld.  

Cashflowprognoses kunnen Azure AI gebruiken om toekomstige documenten te voorspellen. Het resultaat is een uitvoerigere prognose. De verbinding met Azure AI is al voor u ingesteld. U hoeft het alleen in te schakelen. Wanneer u zich bij [!INCLUDE[prod_short](includes/prod_short.md)] aanmeldt, verschijnt er een melding in een blauwe balk en wordt er een koppeling verschaft naar de standaardcashflowinstellingen. De melding wordt slechts eenmaal weergegeven. Als u de melding sluit, maar besluit Azure AI in te schakelen, kunt u de begeleide instelling gebruiken of een handmatig proces.  

> [!NOTE]  
>   U kunt ook uw eigen voorspellende webservice gebruiken. Zie [Uw eigen voorspellende webservice voor cashflowprognoses maken en gebruiken](#AnchorText).  

De begeleide instelling gebruiken:  

1. Kies in het rolcentrum Accountant onder het diagram **Cashflowprognose** de actie **Begeleide instelling openen**.  
2. Vul de velden in elke stap van de begeleiding in.  
3. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Cashflowprognose** in en kies de desbetreffende koppeling.
4. Kies op de pagina **Cashflowprognose** de actie **Prognose herberekenen**.  

Een handmatig proces gebruiken:  

1. Zoek in het rolcentrum Accountant naar **Cashflowinstellingen** en klik vervolgens op de gerelateerde koppeling.  
2. Vouw het sneltabblad **Azure AI** uit en kies het selectievakje **Azure AI ingeschakeld**.  
3. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Cashflowprognose** in en kies de desbetreffende koppeling.
4. Kies op de pagina **Cashflowprognose** de actie **Prognose herberekenen**.  

> [!TIP]  
>   Overweeg de lengte van de perioden die de service in de berekeningen gebruikt. Hoe meer gegevens u biedt, hoe nauwkeuriger de voorspellingen zullen zijn. Let ook op grote variaties in perioden. Deze zijn ook van invloed op voorspellingen. Als Azure AI niet voldoende gegevens vindt of de gegevens sterk variëren, doet de service geen voorspelling.  

## <a name="design-details"></a>Ontwerpdetails
Abonnementen voor [!INCLUDE[prod_short](includes/prod_short.md)] komen met toegang tot verschillende voorspellende webservices in alle regio's waar [!INCLUDE[prod_short](includes/prod_short.md)] beschikbaar is. Zie de Microsoft Dynamics 365 Business Central Licentiehandleiding voor meer informatie. De gids kan worden gedownload op de [Business Central](https://dynamics.microsoft.com/en-us/business-central/overview/)-website. 

Deze webservices zijn staatloos, wat betekent dat ze gegevens alleen gebruiken om voorspellingen op aanvraag te berekenen. Ze slaan geen gegevens op.

> [!NOTE]  
>   U kunt ook uw eigen voorspellende webservice gebruiken in plaats van de onze. Zie [Uw eigen voorspellende webservice voor cashflowprognoses maken en gebruiken](#AnchorText). 

### <a name="data-required-for-forecast"></a>Vereiste gegevens voor prognoses
Om voorspellingen te doen over toekomstige inkomsten en uitgaven hebben webservices historische gegevens nodig van vorderingen, schulden en belastingen.

#### <a name="receivables"></a>Tegoeden:
Velden **Vervaldatum** en **Bedrag (LV)** van de pagina **Klantenposten**, waar:
- Het documenttype is Factuur of Creditnota.
- De vervaldatum ligt tussen de datum die wordt berekend op basis van de waarden in de velden **Historische perioden** en **Periodesoort** op de pagina **Cashflowinstellingen** en de werkdatum.

Voordat de voorspellende webservice wordt gebruikt, comprimeert [!INCLUDE[prod_short](includes/prod_short.md)] transacties op **Vervaldatum**, gebaseerd op de waarde in het veld **Periodesoort** op de pagina **Cashflowinstellingen**.

#### <a name="payables"></a>Schulden:
Velden **Vervaldatum** en **Bedrag (LV)** op de pagina **Leveranciersposten**, waar:
- Het documenttype is 'Factuur' of 'Creditnota'.
- De vervaldatum ligt tussen de datum die wordt berekend op basis van waarden in de velden **Historische perioden** en **Periodesoort** op de pagina **Cashflowinstellingen** en de werkdatum.

Voordat de voorspellende webservice wordt gebruikt, comprimeert [!INCLUDE[prod_short](includes/prod_short.md)] transacties op **Vervaldatum**, gebaseerd op de waarde in het veld **Periodesoort** op de pagina **Cashflowinstellingen**.

#### <a name="tax"></a>Btw:
Velden **Documentdatum** en **Bedrag (LV)** op de pagina **Btw-posten**, waar:
- Het documentsoort 'verkoop' is.
- De documentdatum ligt tussen de datum die wordt berekend op basis van de waarden in de velden **Historische perioden** en **Periodesoort** op de pagina **Cashflowinstellingen** en de werkdatum.

Voordat de voorspellende webservice wordt gebruikt, comprimeert [!INCLUDE[prod_short](includes/prod_short.md)] transacties op **Documentdatum**, gebaseerd op de waarde in het veld **Periodesoort** op de pagina **Cashflowinstellingen**.

## <a name="create-and-use-your-own-predictive-web-service-for-cash-flow-forecasts"></a><a name="AnchorText"> </a>Uw eigen voorspellende webservice voor cashflowprognoses maken en gebruiken
U kunt uw eigen voorspellende webservice maken op basis van een openbaar model met de naam **Prognosemodel voor Business Central**. Dit voorspellend model is online beschikbaar in de Azure AI-galerie. Ga als volgt te werk om het model te gebruiken:  

1. Open een browser en ga naar de [Azure AI-galerie](https://go.microsoft.com/fwlink/?linkid=828352).  
2. Zoek naar **Prognosemodel voor Microsoft Business Central** en open het model in Azure Machine Learning Studio.  
3. Gebruik het Microsoft-account om u aan te melden voor een werkruimte en kopieer vervolgens het model.  
4. Voer het model uit en publiceer het als een webservice.  
5. Noteer de API-URL en de API-sleutel. U kunt deze aanmeldingsgegevens voor een cashflowinstelling gebruiken.  
6. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Cashflowinstellingen** in en kies de desbetreffende koppeling.  
7. Vouw het sneltabblad **Azure AI** uit en vul de velden in.  

## <a name="see-related-training-at-microsoft-learn"></a>Zie Gerelateerde training op [Microsoft Learn](/learn/modules/forecast-cash-flow-dynamics-365-business-central/index)

## <a name="see-also"></a>Zie ook
[Cashflow in uw bedrijf analyseren](finance-analyze-cash-flow.md)  
[Financiën instellen](finance-setup-finance.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]