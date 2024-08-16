---
title: Plaats de jaarafsluiting
description: Beschrijft hoe u het dagboek opent dat u hebt opgegeven in de batchverwerking Afsluiten WenV-rekening en vervolgens de jaareinde-ultimopost controleert en boekt.
author: brentholtorf
ms.topic: conceptual
ms.search.keywords: 'year closing, close accounting period, close fiscal year, bank account detailed trial balance'
ms.search.form: 100
ms.date: 08/05/2024
ms.author: bholtorf
ms.service: dynamics-365-business-central
ms.reviewer: bholtorf
---

# <a name="post-the-year-end-closing-entry"></a>Plaats de jaarafsluiting

Nadat u de batchverwerking **Afsluiten WenV-rekening** hebt gebruikt om de jaareinde-ultimopost of -posten te boeken, moet u het dagboek openen dat u in de batchverwerking hebt opgegeven en vervolgens de posten herzien en boeken.  

> [!TIP]
> Afhankelijk van de werkprocessen van uw organisatie, kunt u ervoor kiezen om boekhoudkundige perioden en boekjaren wel of niet af te sluiten in [!INCLUDE [prod_short](includes/prod_short.md)]. Bij de volgende procedure wordt ervan uitgegaan dat u het boekjaar hebt afgesloten met de optie *Boekhoudperioden*, een jaarafsluitingspost hebt gegenereerd met behulp van de batchverwerking **Resultatenrekeningen sluiten** en nu klaar bent om de jaarafsluitingspost te boeken samen met de uitstellende vermogensrekeningboekingen. Uw organisatie kan ervoor kiezen om anders te werken, zoals het boeken van de jaarafsluitingspost als onderdeel van het afsluiten van het boekjaar.

## <a name="to-post-the-year-end-closing-entry"></a>De jaareinde-ultimopost boeken

1. Kies het pictogram ![Lampje dat de functie Vertel me opent.](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Financiële dagboeken** in en kies vervolgens de gerelateerde koppeling.
2. Selecteer op de pagina  **Algemene dagboeken**  in het veld  **Batchnaam**  de batch die de sluitende posten bevat.
3. Controleer de posten.
4. Kies de actie **Boeken** om het dagboek te boeken.

> [!NOTE]  
> Als een fout wordt gedetecteerd, wordt een foutbericht weergegeven. Als de boeking is geslaagd, worden de geboekte posten uit het dagboek gehaald. Nadat de boeking is voltooid, wordt een post geboekt in elke resultatenrekening zodat het saldo nul wordt en het jaarresultaat wordt overgebracht naar de balans.

## <a name="see-also"></a>Zie ook

[Sluiten Boekhoudperioden](year-close-account-periods.md)    
[Boeken sluiten](year-close-books.md)    
[Sluiten Winst- en verliesrekening](year-close-income-statement.md)    
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]
