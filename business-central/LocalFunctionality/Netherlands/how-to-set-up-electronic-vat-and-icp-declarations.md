---
title: 'Elektronische btw- en ICP-aangiften [NL]'
description: Dit artikel beschrijft hoe u elektronische btw- en ICP-aangiften instelt in de Nederlandse versie.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: altotovi
ms.service: dynamics365-business-central
ms.topic: how-to
ms.date: 12/01/2022
ms.custom: bap-template
---

# <a name="setting-up-electronic-vat-and-icp-declarations-in-the-dutch-version"></a><a name="setting-up-electronic-vat-and-icp-declarations-in-the-dutch-version"></a>Elektronische btw- en ICP-aangiften instellen in de Nederlandse versie

Als u elektronische btw- en ICP-aangiften wilt maken en met de belastingdienst wilt communiceren, moet u eerst algemene gegevens over elektronische belastingaangiften instellen. Uw bedrijf moet met de belastingdienst geregistreerd zijn voordat u elektronische aangiften kunt verzenden.

Als de elektronische aangiften zijn ingesteld, kunt u beginnen btw en ICP naar de belastingdienst te verzenden. Zie voor meer informatie [Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md).  

## <a name="to-set-up-electronic-declarations"></a><a name="to-set-up-electronic-declarations"></a>Elektronische aangiften instellen

Zorg ervoor dat u de certificaten hebt geüpload die nodig zijn om met Digipoort te communiceren. Gebruik de pagina **Certificaten** om een client- en een servicecertificaat te uploaden. Als ze zijn toegevoegd aan de lijst met certificaten kunt u doorgaan met het opzetten van elektronische aangiften.

1. Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Elek. aangifte-instellingen** in en kies vervolgens de gerelateerde koppeling.  
2. Vul op de pagina **Elek. aangifte-instellingen** indien nodig de velden in. [!INCLUDE[tooltip-inline-tip](../../includes/tooltip-inline-tip_md.md)]
3. Als u het btw-nummer van het bedrijf wilt laten invullen bij de contact-id in de elektronische aangifte, selecteert u **Belastingplichtige** in het veld **BTW-contactpersoonsoort**.
4. Als u elektronische ICP-aangiften voor een dochteronderneming van een fiscale eenheid wilt verzenden, schakelt u het selectievakje **Deel van Fiscale eenheid** in.  

    > [!NOTE]  
    > Als een bedrijf verscheidene bedrijven heeft geregistreerd als dochterondernemingen van een moedermaatschappij, hebben deze de mogelijkheid om de btw-aangifte afzonderlijk te doen of gecombineerd voor één fiscale eenheid. Als u elektronische aangiften voor dochterondernemingen van een moedermaatschappij wilt instellen, moet u een vinkje plaatsen in het veld **Deel van Fiscale eenheid** op de pagina **Elek. aangifte-instellingen**. U kunt dan een elektronische aangifte maken voor slechts één bedrijf.<br /><br />
    Als u de btw-gegevens van alle dochterondernemingen van een moedermaatschappij wilt combineren, moet u een btw-aangifte op papier opstellen voor elke dochteronderneming en handmatig de totaalbedragen voor de moedermaatschappij berekenen. Deze totaalbedragen van de moedermaatschappij moeten worden ingevoerd op de website van de belastingdienst.<br /><br />
    U kunt geen belastinggegevens van ICP-aangiften combineren. ICP-aangiften moeten altijd afzonderlijk worden ingediend.<br /><br />
    Voor elke dochteronderneming kan een elektronische ICP-aangifte worden opgesteld en aan de belastingdienst worden gezonden. Deze elektronische ICP-aangiften moeten het btw-nummer van de dochteronderneming en de waarde van het veld **Nr. fiscale eenheid** van de moedermaatschappij op de pagina **Bedrijfsgegevens** bevatten.

5. Stel op het sneltabblad **Digipoort** de volgende configuraties in:
   - Geef in het veld **Directe leverings-URL** de URL op voor de productieversie van de Digipoort Aanlever-service. Meer informatie op [https://www.logius.nl/producten/gegevensuitwisseling/digipoort](https://www.logius.nl/producten/gegevensuitwisseling/digipoort).  
   - Geef in het veld **Digipoort status-URL** de URL op voor de statusinformatie die komt van de Digipoort Statusinformatie-service. Ga voor meer informatie naar [Elektronische btw- en ICP-aangiften](electronic-vat-and-icp-declarations.md).
   - Selecteer **Certificaatinstellingen gebruiken** om op te geven dat de certificaatcodes die in de volgende stap zijn opgegeven, moeten worden gebruikt om gegevens over te dragen naar de informatieservice.
   - Geef in het veld **Code van clientcertificaat** het clientcertificaat op.
   - Geef in het veld **Code van servicecertificaat** het servicecertificaat op.

6. Om eindpunten in te stellen voegt u de eindpunt-URL's toe op het sneltabblad **Eindpunten**.

    > [!NOTE]  
    > De ingestelde eindpunten worden geïmplementeerd in 21.1-tenants. Alle waarden zijn echter leeg, maar de Digipoort-oplossing werkt nog steeds door hardgecodeerde waarden te nemen als er geen waarden in de instellingen zijn. In release 21.2 [!INCLUDE [prod_short](../../includes/prod_short.md)] wordt er automatisch een upgrade uitgevoerd.

## <a name="see-also"></a><a name="see-also"></a>Zie ook

[Elektronische btw- en ICP-aangiften verzenden](electronic-vat-and-icp-declarations.md)  
[Nederlandse lokale functionaliteit](netherlands-local-functionality.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
