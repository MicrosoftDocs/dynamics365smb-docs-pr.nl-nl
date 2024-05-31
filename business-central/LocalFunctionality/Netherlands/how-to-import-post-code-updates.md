---
title: 'Postcode-updates importeren [NL]'
description: Het postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel Postcodereeks bijwerken.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 11/23/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="import-post-code-updates-in-the-dutch-version"></a>Postcode-updates importeren in de Nederlandse versie
Elke maand ontvangt u een postcodebestand met alle postcodemutaties in een maand. Dit postcodebestand kan worden geïmporteerd en kan de relevante gegevens in de tabel **Postcodereeks** bijwerken.  

## <a name="to-import-the-update-file"></a>Het updatebestand importeren

1.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Postcode-updates** in en kies vervolgens de gerelateerde koppeling.  
2.  Kies op de pagina **Postcode-updates** de actie **Postcodes-update importeren**.  
3.  Geef het pad en de naam op van het postcode-updatebestand en kies vervolgens de knop **OK**. Als u het bestand niet wilt importeren, kiest u de knop **Annuleren** om de pagina te sluiten.  

Als geen bestand met een volledige set postcodegegevens is geïmporteerd, verschijnt er een bericht.  

Voordat u de postcodes bijwerkt, worden de volgende controles uitgevoerd:  

- Is er al een updatebestand geïmporteerd met een recenter datumveld dan de datum van dit nieuwe updatebestand? Als dat het geval is, wordt het proces gestopt.  

- Is er een lange periode tussen de datum van dit bestand en de waarde in het datumveld van het laatst geïmporteerde bestand? Als dat het geval is, verschijnt er een bericht. U kunt kiezen of u het updatebestand nog steeds wilt importeren.  

Gegevens over de geïmporteerde postcode worden opgeslagen in de tabel Postcode-update logpost.  

## <a name="see-also"></a>Zie ook
[Nederlandse postcodes](dutch-post-codes.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
