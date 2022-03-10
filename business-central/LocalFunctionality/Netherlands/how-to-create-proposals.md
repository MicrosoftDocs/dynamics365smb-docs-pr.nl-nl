---
title: Voorstellen maken
description: Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.
author: SorenGP
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: 6212fd3ec408afde36ce5ede227a6555e41da639
ms.sourcegitcommit: ef80c461713fff1a75998766e7a4ed3a7c6121d0
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/15/2022
ms.locfileid: "8144174"
---
# <a name="create-proposals"></a>Voorstellen maken
Voorstellen kunnen handmatig of automatisch worden gegenereerd op basis van leveranciers- of klantenposten.  

> [!IMPORTANT]  
>  Als u een voorstel maakt, moet u het veld **Rekeninghouder** op de pagina's Bankrekening leverancier en Bankrekening klant gebruiken.  

> [!NOTE]  
>  U kunt op elk moment en op elk niveau, voorafgaand aan de verwerking van een voorstel, de transactiewijze en bankrekening wijzigen. Op het laagste niveau in de desbetreffende leveranciers- of klantenposten.  

## <a name="to-create-proposals-manually"></a>Handmatig voorstellen maken  

1.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Telebank - bankoverzicht** in en kies vervolgens de gerelateerde koppeling.  
2.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
3.  U moet minimaal de velden **Rekeningsoort**, **Rekeningnr.**, **Transactiewijze**, **Bankrekeningnr.** en **Bedrag** invullen.  

4.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.  

## <a name="to-create-proposals-automatically-from-sales"></a>Automatisch voorstellen maken op basis van verkoop  

1. Stel voor de klant die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.
2. Maak een verkoopfactuur of creditnota, vul de klant en relevante items in en boek de factuur.
3. Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten. Standaard worden deze gekopieerd vanuit de klantenkaart.  

4.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Telebank - bankoverzicht** in en kies vervolgens de gerelateerde koppeling.  
5.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
6.  Kies de actie **Posten ophalen**.  

    U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante klantenposten.  

    > [!NOTE]  
    >  Alleen voor posten die een transactiewijze van het rekeningsoort **Klant** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.  

6.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.  

## <a name="to-create-proposals-automatically-from-purchases"></a>Automatisch voorstellen maken op basis van inkoop  

1.  Stel voor de leverancier die de factuur heeft verstuurd een kaart in met de juiste waarden voor de velden **Valutacode**, **Transactiewijze** en **Bankrekening**.  
2.  Maak een inkoopfactuur of creditnota en voer de leverancier en relevante items in.
3. Boek de factuur.
4. Controleer of de velden **Valutacode**, **Transactiewijze** en **Bankrekening** van de factuur/creditnota de juiste waarden bevatten. Standaard worden deze gekopieerd vanuit de leverancierskaart.  
5.  Kies het ![Lampje dat de functie Vertel me opent.](../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Telebank - bankoverzicht** in en kies vervolgens de gerelateerde koppeling.  
6.  Selecteer de betreffende bankrekening en kies vervolgens de actie **Voorstel**.  
7.  Kies de actie **Posten ophalen**.  

    U kunt de batchverwerking Voorstelposten ophalen gebruiken om voorstelregels te genereren op basis van relevante leveranciersposten.  

    > [!NOTE]  
    >  Alleen voor posten die een transactiewijze van het rekeningsoort **Leverancier** hebben en die aan de actieve bankrekening zijn gekoppeld, worden voorstelregels gemaakt.  

6.  Als u de detailregels van het voorstel wilt bekijken of aanpassen, kiest u de actie **Detailinformatie**. U keert weer terug naar het voorstel door de pagina **Voorsteldetailregel** te sluiten.  

## <a name="see-also"></a>Zie ook  
 [Nieuwe klanten registreren](../../sales-how-register-new-customers.md)   
 [Verkopen factureren](../../sales-how-invoice-sales.md)   
 [Inkopen vastleggen](../../purchasing-how-record-purchases.md)   
 [Betalingsrun maken en exporteren](how-to-create-and-export-payment-history.md)


[!INCLUDE[footer-include](../../includes/footer-banner.md)]