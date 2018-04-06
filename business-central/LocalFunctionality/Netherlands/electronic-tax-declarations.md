---
title: Elektronische belastingaangiften
description: Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 01/10/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: 47d69e7a0ed2541b50a78cead35ace20b1714b16
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="electronic-tax-declarations"></a>Elektronische belastingaangiften
Bedrijven moeten hun btw- en ICP-aangiften elektronisch aanleveren aan de belastingdienst.  

## <a name="prepare-for-electronic-declaration"></a>Voorbereiding voor elektronische aangifte  
 Voordat je elektronische aangiften kan versturen naar de belastingdienst moeten eerst de volgende taken zijn uitgevoerd:  

1.  Gebruikerscertificaten aanvragen bij de certificaatautoriteit (CA) en deze importeren in de toepassing. Zie voor meer informatie de [website](http://go.microsoft.com/fwlink/?LinkID=223151) van de Nederlandse belastingdienst.  
2.  Aanmelden voor elektronische aangifte bij de belastingdienst.  
3.  Algemene en persoonlijke gegevens, ontvangen van de belastingdienst, in het venster **Elek. aangifte-instellingen** invoeren.  

Zie voor meer informatie [Elektronische btw- en ICP-aangiftes](electronic-vat-and-icp-declarations.md).  

## <a name="create-and-submit-electronic-declarations"></a>Elektronische aangiftes maken en verzenden  
Als de hierboven vermelde taken zijn afgerond, kan de toepassing btw- en ICP-aangiften maken en verzenden naar de belastingdienst.  

De belastingdienst zal voor elke ontvangen aangifte een responsbericht sturen. Deze responsberichten worden opgehaald van de server bij de belastingdienst en verwerkt in de applicatie.  

## <a name="response-message-from-the-tax-authorities"></a>Responsbericht van de belastingdienst  
De belastingdienst zal een responsbericht sturen om het bedrijf te informeren over de status van de elektronische aangifte(n). Om te beginnen moet u de responsberichten van de belastingdienst in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] importeren. Vervolgens verwerkt u deze responsberichten.  

Het responsbericht moeten aan de gerelateerde elektronische aangifte zijn gekoppeld.

Als de begeleidende elektronische belastingaangifte is gevonden moeten, afhankelijk van de responssoort, verschillende stappen worden uitgevoerd.  

## <a name="acknowledgement-response-message"></a>Bevestiging van responsbericht  
Als er geen fouten zijn gevonden in de elektronische aangifte en de gegevens zijn verwerkt door de belastingdienst, wordt het veld **Status** in de tabel **Elek. aangiftekop** gewijzigd in **Geaccepteerd**.  

## <a name="declaration-for-a-fiscal-entity"></a>Aangifte voor een fiscale eenheid  
Als een bedrijf verscheidene bedrijven heeft geregistreerd als dochterondernemingen van een moedermaatschappij, hebben deze de mogelijkheid om de btw-aangifte afzonderlijk te doen of gecombineerd voor één fiscale eenheid. Ongeacht de keuze, moeten ICP-aangiften altijd afzonderlijk worden ingediend.  

In het programma kunnen geen belastinggegevens van verschillende bedrijven worden gecombineerd tot één btw-aangifte. Als het bedrijf de belastinggegevens wil combineren, moet er een btw-aangifte op papier worden opgesteld voor elke dochteronderneming en moet het totale bedrag voor de moedermaatschappij worden berekend. Daarna moeten deze bedragen handmatig worden ingevoerd op de website van de belastingdienst.  

Voor elke dochteronderneming kan een elektronische ICP-aangifte worden opgesteld en aan de belastingdienst worden gezonden. Deze elektronische ICP-aangiften moeten het btw-nummer van de dochteronderneming en het veld **Nr. fiscale eenheid** van de moedermaatschappij uit de tabel **Bedrijfsgegevens** bevatten.  

Als u elektronische aangiften voor dochterondernemingen van een moedermaatschappij wilt instellen, moet u een vinkje plaatsen in het veld **Deel van Fiscale eenheid** in het venster **Elek. aangifte-instellingen**.  

## <a name="digipoort"></a>Digipoort
In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden. Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes. De rapporten hebben de XBRL-indeling. Zie voor meer informatie [Overzicht van Digipoort](digipoort-overview.md).

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md)  
 [Overzicht van Digipoort](digipoort-overview.md)

