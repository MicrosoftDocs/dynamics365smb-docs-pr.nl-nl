---
title: Copilot-gegevensverplaatsing tussen geografieën
description: 'Ontdek hoe gegevens die worden gebruikt in copilot-functies in Dynamics 365 Business Central, zich verplaatsen tussen geografieën waar Azure OpenAI Service standaard niet beschikbaar is.'
author: jswymer
ms.author: jswymer
ms.reviewer: jswymer
ms.topic: conceptual
ms.date: 04/16/2024
ms.custom: bap-template
ms.collection:
  - bap-ai-copilot
ms.search.form: 7775
---

# <a name="copilot-data-movement-across-geographies"></a>Copilot-gegevensverplaatsing tussen geografieën

Copilot is beschikbaar in alle ondersteunde [geografische Business Central-landen/regio's](/dynamics365/business-central/dev-itpro/compliance/apptest-countries-and-translations). Copilot gebruikt echter Microsoft Azure OpenAI Service, wat momenteel alleen in bepaalde geografische regio's beschikbaar is voor Business Central. Dit betekent dat als uw omgeving zich elders bevindt, gegevens van de Copilot- en generatieve AI-functies buiten uw geografische regio moeten worden verzonden en mogelijk buiten uw nalevingsgrenzen worden verwerkt en opgeslagen. Gegevens omvatten de AI-prompts en uw bedrijfsgegevens die worden gebruikt of gegenereerd door Copilot. In dit geval moet u inschakelen dat u gegevensverplaatsing naar een Azure OpenAI Service in een andere geografie toestaat. <!--For a list of geographies, refer to the [Azure OpenAI Service geographies](#azure-openai-service-geographies) section that follows.-->

> [!IMPORTANT]
> Als uw omgeving zich in dezelfde Azure-regio bevindt als de Azure OpenAI Service, maakt deze automatisch verbinding met Azure OpenAI Service; er is geen optie en er is geen eenmalige configuratie vereist.

> [!NOTE]
> Individuele Copilot- en generatieve AI-functies zijn mogelijk niet in alle Business Central-landen/regio's beschikbaar. Neem contact op met de uitgever van elke mogelijkheid om de beschikbaarheid te begrijpen.
> 
> Copilot- en generatieve AI-functies van niet-Microsoft-uitgevers, zoals die afkomstig zijn van aanpassingen of AppSource-apps die u installeert, definiëren elk hun eigen specifieke Azure OpenAI Service-regio's. Neem contact op met de uitgever van de extensie om na te gaan welke regionale Azure-services door de extensie worden gebruikt. 

### <a name="azure-openai-service-geographies"></a>Azure OpenAI Service-geografieën

In de volgende tabel ziet u de geografie van de Azure OpenAI Service die door Copilot wordt gebruikt, gebaseerd op de Azure-regio van een Business Central-omgeving. Deze informatie is belangrijk bij de beslissing of u zich wilt aanmelden voor gegevensverplaatsing tussen geografische gebieden. U kunt de Azure-regio voor uw omgeving identificeren in het Business Central-beheercentrum (zie [Omgevingen beheren in het beheercentrum](/dynamics365/business-central/dev-itpro/administration/tenant-admin-center-environments)).

| Omgeving Azure-regio| Azure OpenAI Service-geografie|Beheerdersactie vereist om Copilot te ontgrendelen| 
| - | - | - |
|Azië (Oost, Zuidoost) |Verenigde Staten|Ja|
|Australië (Zuidoost)| Australië |Nr. |
|Brazilië (Zuid) |Verenigde Staten|Ja|
|Canada (Centraal, Oost)|Verenigde Staten|Ja|
|Europa (West, Noord)| Zweden of Zwitserland |Nee\*|
|Frankrijk (Centraal, Zuid)| Zweden of Zwitserland |Ja|
|Duitsland (Noord, West-Centraal)| Zweden of Zwitserland |Ja|
|India (Centraal, Zuid)|India|Nr.|
|Japan (Oost, West)|Verenigde Staten|Ja|
|Korea (Centraal, Zuid)|Verenigde Staten|Ja|
|Noorwegen (Oost, West)|Zweden of Zwitserland |Ja|
|Zuid-Afrika (Noord, West)|Verenigde Staten|Ja|
|Zwitserland (Noord, West) |Zweden of Zwitserland |Ja|
|Verenigde Arabische Emiraten (Noord, West)|Verenigde Staten|Ja|
|Verenigd Koninkrijk (Zuid, West)|Verenigd Koninkrijk|Nr.|
|Verenigde Staten (Centraal, Oost, Noord-Centraal, Zuid-Centraal, West) |Verenigde Staten|Nee|

\* Voor omgevingen in de Azure-regio's West-Europa en Noord-Europa meldt Business Central zich automatisch aan voor gegevensverplaatsing tussen regio's, maar beheerders kunnen zich op elk gewenst moment afmelden.

> [!NOTE]
> Nadat een Azure OpenAI Service beschikbaar is geworden in uw Business Central-geografie, wordt uw omgeving automatisch overgezet naar het gebruik van de Azure OpenAI Service en is aanmelden niet nodig of zelfs mogelijk.


## <a name="next-steps"></a>Volgende stappen

U meldt zich aan (of af) voor gegevensverplaatsing tussen geografieën vanaf de pagina [Copilot- en AI-mogelijkheden](https://businesscentral.dynamics.com/?page=7775). Ga voor meer informatie naar [Gegevensverplaatsing tussen geografische gebieden toestaan](enable-ai.md#allow-data-movement-across-geographies).
