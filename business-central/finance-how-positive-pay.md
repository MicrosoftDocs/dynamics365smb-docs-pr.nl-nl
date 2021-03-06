---
title: Positive Pay-bestanden exporteren| Microsoft Docs
description: U kunt zorgen dat uw bank alleen gevalideerde cheques en bedragen verrekent door een Positive Pay-bestand te exporteren dat gegevens over leveranciers en betalingen bevat.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: check, clearing
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 7d4789f2ef9db38afdb67893d8ac242288c0aae2
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5773977"
---
# <a name="export-a-positive-pay-file"></a>Een Positive Pay-bestand exporteren
Om ervoor te zorgen dat uw bank alleen gevalideerde cheques en bedragen verrekent, kunt u een Positive Pay-bestand exporteren dat leveranciersgegevens, het chequenummer en het betalingsbedrag bevat, die u naar de bank verzendt wanneer u betalingen verwerkt.

[!INCLUDE[prod_short](includes/prod_short.md)] is vooraf geconfigureerd om Positive Pay-bestanden te ondersteunen voor Bank of America en City Bank.

## <a name="to-set-up-a-bank-account-for-positive-pay"></a>Een bankrekening voor Positive Pay instellen
1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.
2. Open de kaart voor de bank waarvoor u Positive Pay wilt gebruiken.
3. Voer in het veld **Positive Pay-exportcode** POSPAYBANK in.
4. Sluit de pagina.

## <a name="to-export-a-positive-pay-file"></a>Een Positive Pay-bestand exporteren
1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.
2. Selecteer de bankrekening waarvoor u een Positive Pay-bestand wilt exporteren.
3. Kies de actie **Positive Pay exporteren**.

    De pagina **Positive Pay exporteren** wordt geopend met betalingen die voor de bankrekening zijn uitgevoerd sinds de laatste uploaddatum, zoals weergegeven in het veld **Laatste uploaddatum** en het veld **Laatste uploadtijd**.
4. In het veld **Afkapdatum voor uploaden** geeft u een datum op waarvóór betalingen niet worden opgenomen in het geëxporteerde bestand.
5. Kies de actie **Exporteren**.
6. Kies op de pagina **Bestand exporteren** de knop **Opslaan** en sla vervolgens het bestand op een geschikte locatie op.
7. Upload het bestand naar uw elektronische banksite.
8. Noteer of kopieer het bevestigingsnummer dat wordt weergegeven wanneer de bestandsupload is gelukt.

Geëxporteerde Positive Pay-records weergeven

1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.
2. Selecteer de bankrekening waarvoor u Positive Pay-exportrecords wilt weergeven.
3. Kies de actie **Positive Pay-posten**.

    Op de pagina **Positive Pay-posten** kunt u alle Positive Pay-exportrecords voor de bankrekening zien.
4. Voer in het veld **Bevestigingsnummer** voor elke exportrecord het bevestigingsnummer in dat u ontvangt als de bestandsupload naar de bank is gelukt.
5. Als u de relateerde betalingsregels wilt weergeven, kiest u de actie **Details van Positive Pay-post**.

Positive Pay-bestanden opnieuw exporteren

1. Kies het pictogram ![Gloeilamp om de Vertel mij-functie te openen](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Bankrekeningen** in en kies de desbetreffende koppeling.
2. Selecteer de bankrekening waarvoor u Positive Pay-bestanden opnieuw wilt exporteren.
3. Kies de actie **Positive Pay-posten**.
4. Selecteer de regel van het Positive Pay-exportbestand dat u opnieuw wilt exporteren.
5. Kies op de pagina **Positive Pay-posten** de actie **Positive Pay opnieuw exporteren naar bestand**.

## <a name="see-also"></a>Zie ook
[Financiën](finance.md)  
[Financiën instellen](finance-setup-finance.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]