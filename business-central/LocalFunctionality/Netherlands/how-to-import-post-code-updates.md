---
title: Postcode-updates importeren
description: Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel Postcodereeks bijwerken.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2020
ms.author: edupont
ms.openlocfilehash: f2273b898e4c0485ec707bd04d41d3a359df4e4b
ms.sourcegitcommit: a80afd4e5075018716efad76d82a54e158f1392d
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2020
ms.locfileid: "3778544"
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
