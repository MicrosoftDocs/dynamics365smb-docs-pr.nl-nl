---
title: Postcode-updates importeren
description: Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel Postcodereeks bijwerken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: d45c9b51e3206998d78a9bf307d681379c8789ae
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5780120"
---
# <a name="import-post-code-updates"></a>Updates van postcodes importeren
Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken.  

## <a name="to-import-the-update-file"></a>Het updatebestand importeren  

1.  Kies het pictogram ![Lampje dat de functie Vertel me opent](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Postcode-updates** in en kies de gerelateerde koppeling.  
2.  Kies op de pagina **Postcode-updates** de actie **Postcodes-update importeren**.  
3.  Geef het pad en de naam op van het postcode-updatebestand en kies vervolgens de knop **OK**. Als u het bestand niet wilt importeren, kiest u de knop **Annuleren** om de pagina te sluiten.  

Als geen bestand met een volledige set postcodegegevens is geïmporteerd, verschijnt er een bericht.  

Voordat de postcodes worden bijgewerkt, worden de volgende controles uitgevoerd:  

- Is er al een updatebestand geïmporteerd met een recenter datumveld dan de datum van dit nieuwe updatebestand? Als dat het geval is, wordt het proces gestopt.  

- Is er een lange periode tussen de datum van dit bestand en de waarde in het datumveld van het laatst geïmporteerde bestand? Als dat het geval is, verschijnt er een bericht. U kunt kiezen of u het updatebestand nog steeds wilt importeren.  

Gegevens over de geïmporteerde postcode worden opgeslagen in de tabel Postcode-update logpost.  

## <a name="see-also"></a>Zie ook  
[Nederlandse postcodes](dutch-post-codes.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]