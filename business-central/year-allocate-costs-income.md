---
title: Overzicht van taken om kosten en inkomsten toe te wijzen | Microsoft Docs
description: Beschrijft de taken om een post in een dagboek te verdelen over verschillende rekeningen wanneer u het dagboek boekt.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 8fec3a7c079058e73cda2b6f8940e3778b405bac
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5775037"
---
# <a name="allocate-costs-and-income"></a>Kosten en inkomsten toewijzen
U kunt een post in een dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt. De verdeling kan plaatsvinden op basis van drie verschillende methoden.

* Aantal
* Percentage (%)
* Bedrag

De toewijzingsfuncties kunnen worden gebruikt met periodieke dagboeken en in VA-dagboeken.
<!--You can also distribute the cost or revenue of a line to an intercompany partner when you post a sales or purchase document. When you post the document, a line will be posted in your general journal, and a corresponding line will be created in the intercompany outbox.-->

In de volgende procedures wordt beschreven hoe voorbereidingen moeten worden getroffen om kosten in een periodiek dagboek te verdelen door verdeelsleutels te definiëren. Wanneer verdeelsleutels worden gedefinieerd, voltooit en boekt u het dagboek zoals elk ander periodiek dagboek. Zie [Werken met diversendagboeken](ui-work-general-journals.md) voor meer informatie.

## <a name="to-set-up-allocation-keys"></a>Verdeelsleutels instellen
U kunt een post in een periodiek dagboek verdelen over verschillende rekeningen wanneer u het dagboek boekt. De verdeling kan plaatsvinden op basis van aantal, percentage of bedrag.
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Periodiek dagboek** in en kies de desbetreffende koppeling.
2. Kies het veld **Batchnaam** om de pagina **Fin. dagboekbatches** te openen.
3. U kunt verdeelsleutels in een bestaande batch in de lijst wijzigen of u kunt een nieuwe batch met verdeelsleutels maken.
   * Als u een nieuwe batch wilt maken, kiest u de actie **Nieuw** en gaat u naar de volgende stap.
   * Als u de verdeelsleutels van een bestaand dagboek wilt wijzigen, selecteert u het dagboek en gaat u naar stap 7.    
4. Voer in het veld **Naam** een naam voor de batch in, bijvoorbeeld Schoonmaak. Voer in het veld **Omschrijving** een omschrijving in, bijvoorbeeld Dagboek schoonmaakkosten.
5. Wanneer u klaar bent, sluit u de pagina. Er wordt een nieuw, leeg periodiek dagboek geopend.
6. Vul de velden op de regel in.
7. Kies de actie **Verdeelsleutels**.
8. Voeg voor elke verdeelsleutel een regel toe. U moet ofwel het veld **Verdeelsleutel %**, of **Verdeelsleutelaantal**, of **Bedrag** invullen. U moet ook het veld **Rekeningnr.** invullen. Als u de transactie wilt toewijzen aan verschillende globale dimensies, moet u ook de globale dimensievelden invullen.
9. Als u een percentage op de regel invoert, wordt het bedrag in het veld **Bedrag** automatisch berekend. Deze bedragen hebben het tegengestelde teken van het totale bedrag in het veld **Bedrag** in het periodieke dagboek.
10. Kies **OK** na het invoeren van de verdeelsleutelregels om terug te keren naar de pagina **Periodiek dagboek**. Het veld **Verdeeld bedrag (LV)** wordt ingevuld en de inhoud komt overeen met het veld **Bedrag**.
11. Boek het dagboek.

## <a name="to-change-an-allocation-key-that-has-already-been-set-up"></a>Een reeds ingestelde verdeelsleutel wijzigen
1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Periodiek dagboek** in en kies de desbetreffende koppeling.
2. Selecteer op de pagina **Periodiek dagboek** het dagboek met de verdeling.
3. Kies de regel met de verdeelsleutel en kies vervolgens **Verdeelsleutels**.
4. Pas de relevante velden aan en kies vervolgens de knop **OK**.

## <a name="see-also"></a>Zie ook
[Afsluitingsjaren en -perioden](year-close-years-periods.md)  
[Werken met diversendagboeken](ui-work-general-journals.md)    
[Documenten en dagboeken boeken](ui-post-documents-journals.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]