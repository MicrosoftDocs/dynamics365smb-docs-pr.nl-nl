---
author: brentholtorf
ms.topic: include
ms.date: 03/06/2023
ms.author: bholtorf
---

> [!NOTE]
> Bedrijven in alle landen/regio's kunnen profiteren van de mogelijkheid om grootboekposten te controleren voordat ze worden geboekt. In een toekomstige release zullen we de land/regio-specifieke functie afschaffen en vervangen door een functie die beschikbaar is in alle land/regio-versies. Nadat de functie is beëindigd, kunt u deze gebruiken om toegang te krijgen tot eerdere beoordelingen, maar niet om nieuwe beoordelingen te doen. We archiveren uw gegevens volgens de lokale vereisten. Ga voor meer informatie over de beëindiging naar [Verouderde functies in de basis-app](/dynamics365/business-central/dev-itpro/upgrade/deprecated-features-w1). Ga voor meer informatie over de vervangingsfunctie naar [Bedragen op grootboekrekeningen controleren](../../../finance-review-accounts.md).

Door tijdelijke grootboekposten te vereffenen kunnen bedrijven werken met tijdelijke rekeningen en transferrekeningen in het grootboek. Tijdelijke en transferrekeningen worden gebruikt om tijdelijke posten op te slaan die op verdere verwerking in het grootboek wachten.  

U kunt tijdelijke rekeningen gebruiken voor:  

- Geldtransfers van de ene naar de andere bankrekening.  
- Financiële transactietransfers van het ene systeem naar het andere, waarbij een deel van de gegevens tijdelijk op het oorspronkelijke systeem staat.  
- Transacties waarvoor u een verkoopfactuur hebt verzonden naar een klant maar nog niet de bijbehorende inkoopfactuur van de leverancier hebt ontvangen.  

Nadat de posten zijn verwerkt, kunt u de functie **Posten vereffenen** gebruiken om de geboekte posten en het boekingsrekeningsoort bij te werken.  

U kunt de vereffening van de vereffende grootboekposten ongedaan maken en vervolgens de gesloten posten openen om wijzigingen aan te brengen.  

## <a name="to-apply-general-ledger-entries" />Grootboekposten vereffenen

1. Kies het ![Lampje dat de functie Vertel me opent.](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.  
3. Kies op de pagina **Grootboekposten** de actie **Posten vereffenen**.  

    Alle openstaande posten voor de grootboekrekening worden weergegeven op de pagina **Grootboekposten vereffenen**.  

    > [!NOTE]  
    > Standaard wordt het veld **Posten opnemen** ingesteld op **Open**. U kunt de waarde van het veld **Posten opnemen** wijzigen in **Alle** of **Afgesloten**. U kunt alleen grootboekposten vereffenen die **open** zijn.  

4. Selecteer de betreffende grootboekpost en kies de actie **Vereffenings-id instellen**.  

    Het veld **Vereffenings-id** wordt bijgewerkt met de gebruikers-id. Het restbedrag wordt weergegeven op de pagina **Saldo** op de pagina **Grootboekposten vereffenen**.  

    > [!IMPORTANT]  
    > U kunt alleen meerdere boekingen toepassen als alle posten die worden toegepast, volledig kunnen worden gesloten.  

5. Kies de actie **Vereffening boeken**.  

    U kunt de vereffening boeken zelfs wanneer het saldobedrag gelijk is aan 0. Wanneer wordt geboekt, wordt het veld **Restbedrag** als volgt beïnvloed:  

    - Als het veld **Saldo** gelijk is aan 0, wordt het veld **Restbedrag** bij alle grootboekposten op 0 gezet.  

    - Als het veld **Saldo** niet gelijk is aan 0, wordt het bedrag in het veld **Saldo** overgebracht naar het veld **Restbedrag** van de grootboekpost die was geselecteerd toen u de vereffening boekte.  

    - Voor alle overige grootboekposten wordt het veld **Restbedrag** op 0 gezet en worden de velden **Open**, **Afgesloten door volgnr.**, **Afgesloten met bedrag** en **Afgesloten op** bijgewerkt.  

    > [!NOTE]  
    > Wanneer wordt geboekt, worden de grootboekposten die het veld **Vereffenings-id** bijwerken, verwijderd.  

6. Kies de knop **OK**.  

## <a name="to-view-the-applied-general-ledger-entries" />De vereffende grootboekposten weergeven

1. Kies het ![Lampje dat de functie Vertel me opent.](../../../media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.  
3. Selecteer de betreffende grootboekpost en kies de actie **Vereffende posten**.  

    U kunt alle vereffende grootboekposten weergeven.  

4. Kies de knop **Ok**.  

## <a name="to-unapply-general-ledger-entries" />De vereffening van grootboekposten ongedaan maken

1. Kies het pictogram :::image type="icon" source="../../../media/ui-search/search_small.png" border="false":::, voer **Grootboekjournalen** in en kies vervolgens de gerelateerde koppeling.  
2. Selecteer een grootboekjournaal en kies vervolgens de actie **Grootboek**.  
3. Selecteer de grootboekpost waarvan u de vereffening ongedaan wilt maken en kies vervolgens de actie **Vereffening ongedaan maken**.  

    De vereffening van de vereffende grootboekposten wordt ongedaan gemaakt.  

    > [!NOTE]  
    > Als een post is vereffend met meer dan één vereffeningspost, moet u de vereffening van de laatste vereffeningspost het eerst ongedaan maken. Standaard wordt de laatste post weergegeven.  

4. Kies de knop **OK**.  
