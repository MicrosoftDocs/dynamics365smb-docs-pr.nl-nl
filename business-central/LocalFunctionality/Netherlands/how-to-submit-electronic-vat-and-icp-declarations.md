---
title: Elektronische btw- en ICP-aangiften verzenden
description: Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden. Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd in het venster Elek. aangifte-instellingen.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 07/01/2017
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: d7fb34e1c9428a64c71ff47be8bcff174649c00d
ms.openlocfilehash: b482632cece8eb26f61b28bf3754ab6c15c3cda1
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="submit-electronic-vat-and-icp-declarations"></a>Elektronische btw- en ICP-aangiften verzenden
Met de eXtensible Business Reporting Language (XBRL) Reporter kunt u de aangifte van Intracommunautaire Leveringen (ICP) of de btw-aangifte in de vereiste XML-indeling verzenden. Wanneer dit wordt verzonden, wordt het bestand verstuurd naar de belastingdienst zoals is gedefinieerd in het venster Elek. aangifte-instellingen.  

De XBRL Reporter zorgt ervoor dat alle rekeningnummers die worden geïmporteerd van [!INCLUDE[d365fin](../../includes/d365fin_md.md)], aan de XBRL-elementen in een rapport worden toegewezen. De XBRL Reporter geeft ook een lijst weer met fouten wegens niet-toegewezen elementen of rekeningen.  

Als u elektronische btw- en ICP-aangiften naar de belastingdienst wilt sturen, voert u respectievelijk de batchverwerking **Elektronische btw-aangifte versturen** en **Elektronische ICP-aangifte versturen** uit. Voordat de batchverwerking de elektronische aangifte naar de belastingdienst verzendt, wordt deze eerst ondertekend, gecomprimeerd en gecodeerd.  

## <a name="to-submit-an-electronic-vat-or-icp-declaration"></a>Een elektronische btw- of ICP-aangifte verzenden  

1.  Kies het pictogram ![Zoeken naar pagina of rapport](../../media/ui-search/search_small.png "pictogram Zoeken naar pagina of rapport"), voer **Elektronische aangiften** in en kies de gerelateerde koppeling.  
2.  Selecteer de elektronische aangifte die u wilt verzenden en kies de actie **Bewerken**.  

    > [!NOTE]  
    >  U kunt alleen een elektronische aangifte verzenden die de status **Gemaakt** heeft. Voor meer informatie over de status van de elektronische aangifte, zie het veld Status.  

3.  Kies de actie **Elektronische aangifte versturen**.  
4.  Vul de velden in zoals beschreven in de volgende tabel.  

    |Veld|Description|  
    |---------------------------------|---------------------------------------|  
    |**PIN**|Het unieke identificatienummer van het bedrijf.<br /><br /> U kunt alleen een waarde invoeren in dit veld als u het veld **Tekenmethode** op **PIN** hebt ingesteld in het venster **Elek. aangifte-instellingen**.|  
    |**Wachtwoord gebruikerscertificaat**|Het wachtwoord dat gebruikt wordt om de gebruikerscertificaten te versleutelen.<br /><br /> U kunt alleen een waarde invoeren in dit veld als u het veld **Tekenmethode** op **PKI** hebt ingesteld in het venster **Elek. aangifte-instellingen**.|  

5.  Kies de knop **OK**.  

De elektronische aangifte wordt verstuurd naar de belastingdienst.  

## <a name="see-also"></a>Zie ook  
[Lijsten met XBRL maken](../../bi-create-reports-with-xbrl.md)

