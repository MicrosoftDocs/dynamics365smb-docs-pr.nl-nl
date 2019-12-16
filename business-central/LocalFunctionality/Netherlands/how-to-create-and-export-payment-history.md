---
title: Betalingsrun maken en exporteren
description: Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken. Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2019
ms.author: sgroespe
ms.openlocfilehash: 7f1960a7aac9d63585073ef02551e4292abae20c
ms.sourcegitcommit: cfc92eefa8b06fb426482f54e393f0e6e222f712
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/03/2019
ms.locfileid: "2881355"
---
# <a name="create-and-export-payment-history"></a>Betalingsrun maken en exporteren
Nadat u een voorstel hebt gemaakt en eventuele wijzigingen hebt aangebracht, kunt u het voorstel verwerken om een betaalrun te maken. Voorstellen kunnen handmatig worden gegenereerd of automatisch op basis van een leveranciers- of klantenpost. Zie [Voorstellen maken](how-to-create-proposals.md) voor meer informatie.  

 Voor het exporteren van betaalruns worden de volgende protocollen ondersteund:  

- BTL91 $)  
- BBV  
- PAYMUL  

## <a name="to-create-a-payment-history-for-a-proposal"></a>Een betaalrun voor een voorstel maken  

1.  Kies het pictogram ![Pagina of rapport zoeken](../../media/ui-search/search_small.png "Pictogram Pagina of rapport zoeken"), voer **Telebank - bankoverzicht** in en kies de desbetreffende koppeling.  

    Als u het voorstel wilt afdrukken voordat u het verwerkt, kiest u de knop **Afdrukken**.  

2.  Als u het voorstel wilt verwerken, kiest u de actie **Verwerken**.  
3.  Als u de betaalrun wilt bekijken, sluit u de pagina **Telebankierenvoorstel**. Zorg dat dezelfde bankrekening op de pagina **Telebankieren - bankoverzicht** is geselecteerd en kies vervolgens de actie **Betaalrun**.  

De pagina **Betaalrunlijst** verschijnt met de betaalrun die u zojuist hebt gemaakt.  

## <a name="to-export-a-payment-history"></a>Een betaalrun exporteren  

- Kies op de pagina **Betaalrunlijst** de actie **Exporteren**.  

    > [!NOTE]  
    >  Er wordt een tekstbestand gemaakt. Dit bestand bevat het pad en de bestandsnaam zoals die in het veld **Standaardbestandsnamen** van het exportprotocol zijn gedefinieerd.  

## <a name="see-also"></a>Zie ook  
 [Voorstellen maken](how-to-create-proposals.md)
