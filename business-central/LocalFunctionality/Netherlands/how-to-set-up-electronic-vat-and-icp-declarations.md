---
title: Elektronische btw- en ICP-aangiften [NL]
description: In het volgende onderwerp wordt beschreven hoe u elektronische btw- en ICP-aangiften instelt in de Nederlandse versie.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 06/30/2021
ms.author: edupont
ms.openlocfilehash: ba01b8e2423fb4849aface22d563ba9ce06bc479
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2022
ms.locfileid: "8148917"
---
# <a name="setting-up-electronic-vat-and-icp-declarations-in-the-dutch-version"></a>Elektronische btw- en ICP-aangiften instellen in de Nederlandse versie
Als u elektronische btw- en ICP-aangiften wilt maken en met de belastingdienst wilt communiceren, moet u eerst algemene gegevens over elektronische belastingaangiften instellen. Uw bedrijf moet met de belastingdienst geregistreerd zijn voordat u elektronische aangiften kunt verzenden. 

Als de elektronische aangiften zijn ingesteld, kunt u beginnen btw en ICP naar de belastingdienst te verzenden. Zie voor meer informatie [Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md).  

## <a name="to-set-up-electronic-declarations"></a>Elektronische aangiften instellen  

Zorg er eerst voor dat u de certificaten heeft geüpload die u nodig heeft om met Digipoort te communiceren. Dit wordt gedaan op de pagina **Certificaten**. U heeft een client- en een servicecertificaat nodig. Als ze zijn toegevoegd aan de lijst met certificaten kunt u doorgaan met het opzetten van elektronische aangiften.

1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Elek. aangifte-instellingen** in en kies vervolgens de gerelateerde koppeling.  
2. Vul op de pagina **Elek. aangifte-instellingen** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. Als u het btw-nummer van het bedrijf wilt laten invullen bij de contact-id in de elektronische aangifte, selecteert u **Belastingplichtige** in het veld **BTW-contactpersoonsoort**.
4. Als u elektronische ICP-aangiften voor een dochteronderneming van een fiscale eenheid wilt verzenden, schakelt u het selectievakje **Deel van Fiscale eenheid** in.  

    > [!NOTE]  
    > Als een bedrijf verscheidene bedrijven heeft geregistreerd als dochterondernemingen van een moedermaatschappij, hebben deze de mogelijkheid om de btw-aangifte afzonderlijk te doen of gecombineerd voor één fiscale eenheid. Als u elektronische aangiften voor dochterondernemingen van een moedermaatschappij wilt instellen, moet u een vinkje plaatsen in het veld **Deel van Fiscale eenheid** op de pagina **Elek. aangifte-instellingen**. U kunt dan een elektronische aangifte maken voor slechts één bedrijf.<br /><br />
    Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen. Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst.<br /><br />
    U kunt geen belastinggegevens van ICP-aangiften combineren. ICP-aangiften moeten altijd afzonderlijk worden ingediend.<br /><br />
    Voor elke dochteronderneming kan een elektronische ICP-aangifte worden opgesteld en aan de belastingdienst worden gezonden. Deze elektronische ICP-aangiften moeten het btw-nummer van de dochteronderneming en de waarde van het veld **Nr. fiscale eenheid** van de moedermaatschappij op de pagina **Bedrijfsgegevens** bevatten.

5. Geef in het veld **Directe leverings-URL** de URL op voor de productieversie van de Digipoort Aanlever-service. Zie [https://www.logius.nl/producten/gegevensuitwisseling/digipoort](https://www.logius.nl/producten/gegevensuitwisseling/digipoort) voor meer informatie.  
6. Geef in het veld **Digipoort status-URL** de URL op voor de statusinformatie die komt van de Digipoort Statusinformatie-service. Zie voor meer informatie [Elektronische btw- en ICP-aangiftes](electronic-vat-and-icp-declarations.md).
7. Geef in het veld **Clientcertificaatcode** het clientcertificaat uit de lijst met certificaten op.
8. Geef in het veld **Servicecertificaatcode** het servicecertificaat uit de lijst met certificaten op.

## <a name="see-also"></a>Zie ook  
 [Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md)  
 [Nederlandse lokale functionaliteit](netherlands-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
