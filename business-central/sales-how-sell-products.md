---
title: Een verkooporder maken en producten verkopen | Microsoft Docs
description: Beschrijft hoe u een verkooporder maakt om uw overeenkomst vast te leggen met een klant om producten onder bepaalde voorwaarden te verkopen of te verhandelen.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: trade
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 19b32e8faa6b9e56505379d1f06fd5ad79466614
ms.sourcegitcommit: f9a190933eadf4608f591e2f1b04c69f1e5c0dc7
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/28/2021
ms.locfileid: "6115512"
---
# <a name="sell-products"></a>Producten verkopen

U maakt een verkoopfactuur of een verkooporder om uw overeenkomst met een klant vast te leggen om bepaalde producten tegen bepaalde leverings- en betalingsvoorwaarden te verkopen.

> [!NOTE]  
> Gebruik verkooporders als uw verkoopproces vereist dat u delen van een orderhoeveelheid kunt verzenden, bijvoorbeeld omdat de volledige hoeveelheid niet in één keer beschikbaar is. Als u verkoopfacturen gebruikt, gaat [!INCLUDE [prod_short](includes/prod_short.md)] ervan uit dat u de volledige hoeveelheid verzendt wanneer u de factuur boekt. Als u artikelen verkoopt door rechtstreeks van uw leverancier bij de klant te leveren, als een doorverzending, moet u ook verkooporders gebruiken. Zie [Doorverzendingen maken](sales-how-drop-shipment.md) voor meer informatie. Wat betreft alle andere aspecten werken verkooporders op dezelfde manier als verkoopfacturen. Zie [Verkopen factureren](sales-how-invoice-sales.md) voor meer informatie.

U kunt met de klant onderhandelen door eerst een verkoopofferte te maken, die u kunt omzetten in een verkooporder wanneer er een overeenkomst is. Zie voor meer informatie [Verkoopoffertes maken](sales-how-make-offers.md).

Nadat de klant de overeenkomst heeft bevestigd, bijvoorbeeld na een offerteproces, kunt u een orderbevestiging verzenden om uw verplichting vast te leggen dat de producten worden geleverd zoals is overeengekomen.

Als u de producten volledig of gedeeltelijk levert, boekt u de verkooporder als verzonden of als verzonden en gefactureerd om het gerelateerde artikel en de klantposten in uw systeem te maken. Wanneer u de verkooporder boekt, kunt u ook het document als een PDF-bijlage via e-mail versturen. U kunt ook de hoofdtekst van de e-mail vooraf invullen met een overzicht van de orde- en betalingsgegevens, zoals een koppeling naar PayPal. Zie [Documenten per e-mail verzenden](ui-how-send-documents-email.md) voor meer informatie.

In ondernemingsomgevingen waar de klant enige tijd na levering betaalt, volgens de betalingsconditie, blijft een geboekte verkoopfactuur open (onbetaald) totdat de afdeling Vorderingen controleert of de betaling is ontvangen en de betaling vereffent met de geboekte verkoopfactuur. Zie voor meer informatie [Betalingen vereffenen met automatische vereffening](receivables-how-reconcile-payments-auto-application.md).

In ondernemingsomgevingen waar de klant direct betaalt, bijvoorbeeld met PayPal of contant, wordt de betaling direct geregistreerd wanneer u de verkooporder als gefactureerd boekt, dat wil zeggen, de geboekte verkoopfactuur wordt gesloten als volledig vereffend. U selecteert de relevante methode in het veld **Betalingswijze** in de verkooporder. Zie onder stap 8. Voor elektronische betalingen, zoals PayPal, moet u ook het veld **Betalingsservice** invullen. Zie [Klantbetalingen via betalingsservices inschakelen](sales-how-enable-payment-service-extensions.md) voor meer informatie.

U kunt zelfs direct betaalde orders voor niet-geregistreerde klanten maken door eerst een kaart voor een contant betalende klant te maken, waarnaar u verwijst op de verkooporder. Raadpleeg voor meer informatie [Contant betalende klanten instellen](finance-how-to-set-up-cash-customers.md).

U kunt een geboekte verkoopfactuur die het resultaat is van een verkooporder gemakkelijk corrigeren of annuleren voordat deze wordt betaald. Dit is handig als u een typfout wilt corrigeren of als de klant om een wijziging in het begin van het orderproces verzoekt. Zie voor meer informatie [Onbetaalde verkoopfacturen corrigeren of annuleren](sales-how-correct-cancel-sales-invoice.md). Als de geboekte verkoopfactuur is betaald, moet u een verkoopcreditnota maken om de verkoop tegen te boeken. Zie [Verkoopretouren of annuleringen verwerken](sales-how-process-sales-returns-cancellations.md) voor meer informatie.

De artikelkaart kan van het type **Voorraad**, **Service** en **Niet-voorraad** zijn om op te geven of het artikel een fysieke voorraadeenheid, een eenheid voor arbeidskosten of een fysieke eenheid die niet in voorraad wordt gehouden, is. Zie voor meer informatie [Nieuwe artikelen registreren](inventory-how-register-new-items.md). Het verkooporderproces is hetzelfde voor alle drie de artikeltypen.

U kunt klantvelden op de verkooporder op twee manieren invullen afhankelijk van de vraag of de klant reeds is geregistreerd. Zie stap 2 in de volgende procedure.

## <a name="to-create-a-sales-order"></a>Een verkooporder maken

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Verkooporders** in en kies de gerelateerde koppeling.
2. Voer in het veld **Klant** de naam in van een bestaande klant.

    Overige velden op de pagina **Verkooporder** worden nu ingevuld met de standaardinformatie over de geselecteerde klant.  

    [!INCLUDE [sales-create-customer](includes/sales-create-customer.md)]  

    Verschillende velden op de verkooporder worden nu ingevuld met gegevens die u hebt opgegeven op de nieuwe klantenkaart.
3. Vul desgewenst de overige velden op de pagina **Verkooporder** in. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

    > [!NOTE]  
    > Als u toestaat dat de klant direct betaalt, bijvoorbeeld met creditcard of PayPal, vult u het veld **Betalingswijze** in. De betaling wordt vervolgens geregistreerd zodra u de verkooporder als gefactureerd boekt. Als u CONTANT selecteert, wordt de betaling geregistreerd in een opgegeven tegenrekening.

    U kunt nu de verkooporderregels invullen met voorraadartikelen of services die u aan de klant wilt verkopen.

    Als u terugkerende verkoopregels voor de klant hebt ingesteld, zoals een maandelijkse aanvullingsorder, kunt u deze regels invoegen op de order door de actie **Terugkerende verkoopregels ophalen** te kiezen.
4. Selecteer op het sneltabblad **Regels** in het veld **Soort** het type product, kosten of transactie die u wilt boeken voor de klant met deze verkoopregel.

5. Kies in het veld **Nr.** het nummer in van een voorraadartikel of service.

    Laat het veld **Nr.** leeg in de volgende gevallen:

    * Als de regel voor een opmerking is. Schrijf de opmerking in het veld **Omschrijving**.
    * Als de regel voor een catalogusartikel is. Kies de actie **Catalogusartikelen selecteren**. Zie voor meer informatie [Werken met catalogusartikelen](inventory-how-work-nonstock-items.md).
6. Geef in het veld **Aantal** op hoeveel artikelen u wilt verkopen.

    > [!NOTE]  
    > Voor artikelen van de soort *Resource* of *Service* is de hoeveelheid een tijdseenheid, bijvoorbeeld uren, zoals aangegeven in het veld **Eenheidscode** op de regel. Zie [Artikeleenheden instellen](inventory-how-setup-units-of-measure.md) voor meer informatie.

    Het veld **Regelbedrag** wordt bijgewerkt met de waarde in het veld **Eenheidsprijs**, vermenigvuldigd met de waarde in het veld **Aantal**.

    De prijs en de regelbedragen worden weergegeven met of zonder btw afhankelijk van wat u hebt geselecteerd in het veld **Prijzen inclusief btw** op de klantenkaart.
7. In het veld **Regelkorting %** voert u een percentage in als u de klant een korting op het product wilt verlenen. De waarde in het veld **Regelbedrag** wordt dienovereenkomstig bijgewerkt.

    Als u speciale artikelprijzen hebt ingesteld op het sneltabblad **Verkoopprijzen en verkoopregelkortingen** op de klantenkaart of de artikelkaart, worden de prijs en het bedrag op de offerteregel automatisch bijgewerkt als aan de overeengekomen prijscriteria is voldaan. Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).
8. Als u een opmerking over de offerteregel wilt toevoegen die de klant op de afgedrukte verkoopofferte kan zien, schrijft u een tekst in het veld **Omschrijving** op een lege regel.  
9. Herhaal stap 4 t/m 8 voor elk artikel dat u aan de klant wilt verkopen.

    De totalenvelden onder de regels worden automatisch bijgewerkt wanneer u regels maakt of wijzigt om de bedragen weer te geven die naar de grootboeken worden geboekt.

    > [!NOTE]
    > In zeer zeldzame gevallen kunnen de geboekte bedragen afwijken van wat wordt weergegeven in de totalenvelden. Dit is meestal het gevolg van afrondingsberekeningen met betrekking tot btw of omzetbelasting.
    >
    > Om de bedragen te controleren die daadwerkelijk worden geboekt, kunt u de pagina **Statistieken** gebruiken, die rekening houdt met de afrondingsberekeningen. Als u de actie **Vrijgeven** kiest, worden de totalenvelden ook bijgewerkt met afrondingsberekeningen.  

10. Voer desgewenst in het veld **Kortingsbedrag op factuur** een bedrag in dat moet worden afgetrokken van de waarde in het veld **Totaal incl. btw**.

    Als u factuurkortingen voor de klant hebt opgegeven, wordt het opgegeven percentage automatisch ingevoegd in het veld **Factuurkorting %** als aan de voorwaarden wordt voldaan, en het gerelateerde bedrag wordt ingevoegd in het veld **Factuurkortingsbedrag excl. btw** . Zie voor meer informatie [Afspraken over prijzen, kortingen en betalingen van verkopen vastleggen](sales-how-record-sales-price-discount-payment-agreements.md).
11. Als u slechts een deel van het orderaantal wilt verzenden, voert u dat aantal in het veld **Te verzenden aantal** in. De waarde wordt gekopieerd naar **Te factureren aantal**.
12. Als u slechts een deel van het verzonden aantal wilt factureren, voert u dat aantal in het veld **Te factureren aantal** in. Het aantal moet lager zijn dan de waarde in het veld **Te verzenden aantal**.  
13. Wanneer de verkooporderregels zijn ingevuld, kiest u de actie **Boeken en verzenden**.

Het dialoogvenster **Boeken en verzenden bevestigen** geeft de manier aan waarop de klant de documenten wil ontvangen. U kunt de verzendmethode wijzigen door de opzoekknop voor het veld **Document verzenden naar** te kiezen. Zie [Verzendprofielen voor documenten instellen](sales-how-setup-document-send-profiles.md) voor meer informatie.

Het gerelateerde artikel en de gerelateerde klantposten worden nu gemaakt in het systeem en de verkooporder is uitvoer als een PDF-document. Als de verkooporder volledig is geboekt, wordt deze verwijderd uit de lijst met verkooporders en vervangen door nieuwe documenten in de lijst met geboekte verkoopfacturen en de lijst met van geboekte verkoopverzendingen.  

## <a name="external-document-number"></a>Externe documentnummer

[!INCLUDE [ext-doc-no-sales](includes/ext-doc-no-sales.md)]

## <a name="see-also"></a>Zie ook

[Verkoop](sales-manage-sales.md)  
[Verkopen instellen](sales-setup-sales.md)  
[De picklijst afdrukken](sales-how-print-picking-list.md)  
[Voorraad](inventory-manage-inventory.md)  
[Documenten per e-mail verzenden](ui-how-send-documents-email.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]