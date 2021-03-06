---
title: De status van synchronisatietaken weergeven | Microsoft Docs
description: Leer hoe u de status kunt bekijken na het synchroniseren van gekoppelde records.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: sales, crm, integration, sync, synchronize
ms.date: 04/01/2021
ms.author: bholtorf
ms.openlocfilehash: b87bd1061adbcaae3a5497fa1af020cfaa412593
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5781258"
---
# <a name="view-the-status-of-synchronization-jobs"></a>De status van synchronisatietaken weergeven
[!INCLUDE[prod_short](includes/cc_data_platform_banner.md)]

Gebruik de pagina **Synchronisatiefouten met gekoppelde gegevens** om de status weer te geven van synchronisatietaken die zijn uitgevoerd voor gekoppelde records in een Dataverse- of een [!INCLUDE[crm_md](includes/crm_md.md)]-integratie. Hieronder vallen taken die zijn uitgevoerd vanuit de verwerkingswachtrij en handmatige synchronisatietaken die zijn uitgevoerd op records vanuit de [!INCLUDE[prod_short](includes/prod_short.md)]-client. Het bekijken van hun status is bijvoorbeeld handig bij het oplossen van problemen omdat het u toegang geeft tot details over fouten met betrekking tot gekoppelde records. Meestal worden dit soort fouten veroorzaakt door gebruikersacties, bijvoorbeeld wanneer:  

* Twee personen hebben in beide zakelijke apps een wijziging aangebracht in dezelfde gegevens.
* Iemand heeft gegevens verwijderd in een van de apps, maar niet in beide.

> [!Note]
> De pagina **Synchronisatiefouten met gekoppelde gegevens** toont informatie over taken gerelateerd aan gekoppelde records. Als u alle fouten oplost maar records nog steeds niet synchroniseren, heeft dit mogelijk te maken met een instelling voor de integratie. Doorgaans moet uw beheerder dit soort fouten oplossen.   

<!--

> [!VIDEO https://go.microsoft.com/fwlink/?linkid=2098171]

-->

## <a name="to-view-and-resolve-synchronization-errors-for-coupled-records"></a>Synchronisatiefouten voor gekoppelde records weergeven en oplossen
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Synchronisatiefouten met gekoppelde gegevens** in en kies de desbetreffende koppeling.
2. De pagina **Synchronisatiefouten met gekoppelde gegevens** bevat problemen die zijn opgetreden toen u gekoppelde records synchroniseerde. De volgende tabel bevat acties die u kunt gebruiken om problemen één voor één op te lossen:

|Actie|Omschrijving|
|----|----|
|**Koppeling verwijderen**|Ontkoppelt de records en deze zullen niet langer synchroniseren. Om de synchronisatie te hervatten moet u ze opnieuw koppelen. |
|**Opnieuw** en **Alles opnieuw proberen**|Voor elke record waarin een fout wordt gevonden, wordt de synchronisatie overgeslagen, tenzij u het probleem verhelpt. Met Opnieuw zal de geselecteerde record worden opgenomen in de volgende synchronisatie en met **Alles opnieuw proberen** worden alle records opgenomen.|
|**Synchroniseren**|De app probeert een conflict op te lossen waarbij gegevens zijn gewijzigd in beide zakelijke apps. U kunt kiezen welke gegevens worden gebruikt.|
|**Records herstellen** en **Records verwijderen**|Deze zijn handig wanneer een record in een van de bedrijfsapps is verwijderd. Records verwijderen verwijdert de record of rij in de app waar deze nog steeds bestaat. Met Records herstellen wordt de record of rij opnieuw gemaakt in de bedrijfsapp waarin deze is verwijderd.|

> [!NOTE]
> Om het aantal conflicten dat u moet oplossen te verminderen, kunt u uw integratietabeltoewijzingen zo instellen dat deze acties automatisch worden toegepast. Zie voor meer informatie [Integratietabellen toewijzen](admin-how-to-modify-table-mappings-for-synchronization.md#mapping-integration-tables).

## <a name="to-view-the-synchronization-log-for-a-specific-manually-synchronized-record"></a>Het synchronisatielogboek weergeven voor een specifieke (handmatig gesynchroniseerde) record
1. Open bijvoorbeeld een klant-, artikel- of andere record die gegevens synchroniseert tussen [!INCLUDE[prod_short](includes/prod_short.md)] en Dataverse of [!INCLUDE[crm_md](includes/crm_md.md)].
2. Kies de actie **Synchronisatielogbestand** om het synchronisatielogbestand voor een geselecteerde record weer te geven. Bijvoorbeeld een specifieke klant die u handmatig hebt gesynchroniseerd.

## <a name="see-also"></a>Zie ook  
[Gebruikersaccounts instellen voor integratie met Dynamics 365 Sales](admin-setting-up-integration-with-dynamics-sales.md)  
[Microsoft Dynamics 365 Sales gebruiken vanuit Business Central](marketing-integrate-dynamicscrm.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]