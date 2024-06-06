---
title: Verplichte beschrijvingen in grootboekpost
description: Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld.
author: brentholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: null
ms.date: 12/08/2023
ms.author: bholtorf
ms.service: dynamics-365-business-central
---
# <a name="required-descriptions-in-g-l-entry"></a>Verplichte beschrijvingen in grootboekpost

Bij het invoeren van memoriaalregels in een formulier wordt het omschrijvingsveld automatisch ingevuld. Deze omschrijving wordt ook opgeslagen in de grootboekpost na het boeken van het dagboek. Voor een goede auditprocedure is een meer gedetailleerde omschrijving wenselijk wanneer u een dagboekregel van de soort Grootboekrekening boekt.  

Om een gebruiker te dwingen een meer gedetailleerde omschrijving in te voeren, is het mogelijk te kiezen of het systeem automatisch de omschrijving van de grootboekrekening moet invullen of het veld leeg laten. Als het veld **Standaardbeschrijv. in dagboek weglaten** op de pagina **Grootboekrekening** is aangevinkt, wordt het veld **Omschrijving** voor die grootboekrekening niet ingevuld wanneer dit wordt geselecteerd in een algemene dagboekregel.  

Wanneer de dagboekregels worden geboekt, wordt door het systeem gecontroleerd of alle velden **Omschrijving** zijn ingevuld. Als er een blanco omschrijving is, wordt een foutmelding gegeven.  

> [!NOTE]  
> Het leeg laten van het omschrijvingsveld en controleren of alle omschrijvingsvelden zijn ingevuld vóór het boeken, wordt alleen gedaan in de memoriaalpagina's op verscheidene plaatsen in de module en op de pagina's van Kas, Bank, Giro.  

## <a name="see-also"></a>Zie ook

[Klantbetalingen handmatig vereffenen](../../receivables-how-apply-sales-transactions-manually.md)  
[Een auditfile voor de belastingdienst maken](how-to-create-an-audit-file-for-the-tax-authority.md)  
[Het grootboek en COA begrijpen](../../finance-general-ledger.md)  


[!INCLUDE[footer-include](../../includes/footer-banner.md)]
