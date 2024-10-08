---
title: Afschrijvingsmethoden voor vaste activa
description: Meer informatie over de verschillende ingebouwde methoden om vaste activa af te schrijven of in waarde te verminderen.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: 'write down, depreciate, depreciation'
ms.search.form: '5629, 5633'
ms.date: 03/25/2024
ms.custom: bap-template
ms.service: dynamics-365-business-central
---

# <a name="depreciation-methods-for-fixed-assets"></a>Afschrijvingsmethoden voor vaste activa

[!INCLUDE [prod_short](includes/prod_short.md)] ondersteunt acht verschillende afschrijvingsmethoden voor vaste activa:

* Lineair
* Boekwaarde-afschrijving 1 (BW1)
* Boekwaarde-afschrijving 2 (BW2)
* BW1/Lin
* BW2/Lin
* Halfjaarlijkse afspraak
* Handmatig
* Door de gebruiker gedefinieerde afschrijving

## <a name="straight-line-depreciation"></a>Lineaire afschrijving

Bij lineaire afschrijving schrijft u de activumwaarde af met een vast jaarlijks percentage of met een vast jaarlijks bedrag over de afschrijvingsperiode. Als u de lineaire afschrijvingsmethode gebruikt, moet u een van de volgende opties opgeven in het afschrijvingsboek voor vaste activa:  

* De afschrijvingsperiode (jaren of maanden) of een einddatum voor de afschrijving  
* Een vast jaarpercentage  
* Een vast jaarbedrag  
* Afschrijvingsperiode  

### <a name="depreciation-period"></a>Afschrijvingsperiode

Als u de afschrijvingsperiode invoert (aantal afschrijvingsjaren, aantal afschrijvingsmaanden of de einddatum voor de afschrijving), wordt de volgende formule gebruikt om het afschrijvingsbedrag te berekenen:  

* Afschrijvingsbedrag = ((Boekwaarde - Restwaarde) x Aantal afschrijvingsdagen) / Resterende afschrijvingsdagen*  

De resterende afschrijvingsdagen zijn het aantal afschrijvingsdagen min het aantal dagen tussen de begindatum van de afschrijving en de datum van de laatste post voor vaste activa.  

De boekwaarde kan worden verminderd door de geboekte waardevermeerdering, waardevermindering, bedragen voor vrij 1 en vrij 2. Bepalend hiervoor is of het veld **Opnemen in afschr.-berekening** is uitgeschakeld en of het veld **Deel v. boekwaarde** op de pagina **VA-boekingssoortinstellingen** is ingeschakeld. Deze berekening zorgt ervoor dat het vaste activum volledig is afgeschreven op de einddatum van de afschrijving.  

### <a name="fixed-yearly-percentage"></a>Vast jaarpercentage

Als u een vast jaarpercentage invoert, gebruikt [!INCLUDE [prod_short](includes/prod_short.md)] de volgende formule om het afschrijvingsbedrag te berekenen:  

* Afschrijvingsbedrag = (Lineair % x Afschrijvingsbasis x Aantal afschrijvingsdagen) / (100 x 360)*  

### <a name="fixed-yearly-amount"></a>Vast jaarbedrag

Als u een vast jaarbedrag invoert, gebruikt [!INCLUDE [prod_short](includes/prod_short.md)] de volgende formule om het afschrijvingsbedrag te berekenen:  

* Afschrijvingsbedrag = (Vast afschrijvingsbedrag x Aantal afschrijvingsdagen) /360*  

### <a name="example---straight-line-depreciation"></a>Voorbeeld: lineaire afschrijving

De aanschafkosten van een vast activum bedragen LV 100.000. De verwachte levensduur is acht jaar. De batchverwerking **Afschrijving berekenen** wordt elk half jaar uitgevoerd.  

Voor dit voorbeeld ziet de post voor vaste activa er als volgt uit:  

| Datum | VA-boekingssoort | Dagen | Bedrag | Boekwaarde |
| ---- | --------------- | ---- | ------ | ---------- |
| 01/01/20 |Aanschafkosten |(Begindatum afschrijving) |100,000.00 |100,000.00 |
| 06/30/20 |Afschrijvingen |180 |-6.250,00 |93,750.00 |
| 12/31/20 |Afschrijvingen |180 |-6.250,00 |87,500.00 |
| 06/30/21 |Afschrijvingen |180 |-6.250,00 |81,250.00 |
| 31-12-21 |Afschrijvingen |180 |-6.250,00 |75,000.00 |
| ...      |             |    |          |          |
| 30-06-27 |Afschrijvingen |180 |-6.250,00 |6,250.00  |
| 31-12-27 |Afschrijvingen |180 |-6.250,00 |0         |

## <a name="declining-balance-1-depreciation"></a>Boekwaarde-afschrijving 1

Dit is een afschrijvingsmethode waarbij het grootste gedeelte van de kostprijs van een activum wordt verdeeld over de eerste jaren van de gebruiksduur. Als u deze methode gebruikt, moet u een vast jaarpercentage invullen.  

Met de volgende formule worden afschrijvingsbedragen berekend:  

* Afschrijvingsbedrag = (Boekwaarde afschr. % x Aantal afschrijvingsdagen x Afschrijvingsbasis) / (100 x 360)*  

De afschrijvingsbasis wordt berekend als de boekwaarde aan het begin van het jaar. Het aantal afschrijvingsdagen bestaat uit het aantal dagen tussen de boekingsdatum en de laatste afschrijvingsdatum. [!INCLUDE [prod_short](includes/prod_short.md)] berekent de afschrijving ervan uitgaande dat alle afschrijvingen in het fiscale jaar met deze formule worden gedaan.  

De geboekte afschrijving kan posten met verschillende boekingssoorten bevatten (waardevermindering, vrij 1 en vrij 2), die zijn geboekt sinds de begindatum van het lopende boekjaar. Deze boekingssoorten worden opgenomen in het geboekte afschrijvingsbedrag als de velden **Afschrijvingssoort** en **Deel v. boekwaarde** op de pagina **VA-boekingssoortinstellingen** zijn ingeschakeld.  

### <a name="example-1---declining-balance-1-depreciation"></a>Voorbeeld 1: boekwaarde-afschrijving 1

De aanschafkosten van een vast activum bedragen LV 100.000. Het veld **Boekwaarde afschr. %** is 25. De batchverwerking **Afschrijving berekenen** wordt elk half jaar uitgevoerd.  

In de volgende tabel ziet u hoe de posten van een vast activum eruit zien.  

| Datum | VA-boekingssoort | Dagen | Bedrag | Boekwaarde |
| ---- | --------------- | ---- | ------ | ---------- |
| 01/01/20 |Aanschafkosten |(Begindatum afschrijving) |100,000.00 |100,000.00 |
| 06/30/20 |Afschrijvingen |180 |-12.500,00 |87,500.00 |
| 12/31/20 |Afschrijvingen |180 |-12.500,00 |75,000.00 |
| 06/30/21 |Afschrijvingen |180 |-9.375,00 |65,625.00 |
| 12/31/21 |Afschrijvingen |180 |-9.375,00 |56,250.00 |
| 06/30/22 |Afschrijvingen |180 |-7.031,25 |49,218.75 |
| 12/31/22 |Afschrijvingen |180 |-7.031,25 |42,187.50 |
| 06/30/23 |Afschrijvingen |180 |-5.273,44 |36,914.06 |
| 12/31/23 |Afschrijvingen |180 |-5.273,44 |31,640.62 |
| 06/30/24 |Afschrijvingen |180 |-3.955,08 |27,685.54 |
| 31-12-24 |Afschrijvingen |180 |-3.955,08 |23,730.46 |
| ...      |             |    |          |          |

Berekeningsmethode:  

* Jaar 1: *25% van 100.000 = 25.000 = 12.500 + 12.500*
* Jaar 2: *25% van 75.000 = 18.750 = 9.375 + 9.375*
* Jaar 3: *25% van 56.250 = 14.062,50 = 7.031,25 + 7.031,25*
* ...

De berekening gaat door totdat de boekwaarde gelijk is aan het maximale restbedrag na afschrijving of aan de opgegeven restwaarde.  

### <a name="example-2---declining-balance-1-depreciation"></a>Voorbeeld 2: boekwaarde-afschrijving 1

De boekwaarde van een activum is 100.000 op 31-12-2022. U boekt een afschrijving van 1778 op 2/2/23, wat het verwachte (proportionele) bedrag is van de afschrijving van het jaar na 32 dagen. Als u afschrijving uitvoert op 30-6-2023 stelt [!INCLUDE [prod_short](includes/prod_short.md)] 8.222 voor, omdat er 148 dagen zijn van 2-2-2023 tot 30-6-2023. De verwachte resterende afschrijving voor 30-06-2023 wordt berekend aan de hand van de volgende formule:

* *148/360 x 0,20 x 100.000 = 8222*

### <a name="example-3---declining-balance-1-depreciation"></a>Voorbeeld 3: boekwaarde-afschrijving 1

Als u een bedrag boekt dat niet overeenkomt met de afschrijvingsmethode Boekwaarde-afschrijving 1, bijvoorbeeld 5000, stelt [!INCLUDE [prod_short](includes/prod_short.md)] het restant van het verwachte bedrag voor.

De boekwaarde van een activum is 100.000 op 31-12-2022. U boekt een afschrijving van 5000 op 2-2-2023, wat meer is dan het verwachte (proportionele) bedrag op 2-2-2023 op 32 dagen. Als u afschrijving uitvoert op 30-6-2023, stelt [!INCLUDE [prod_short](includes/prod_short.md)] 8222 voor, omdat er 148 dagen zijn van 2-2-2023 tot 30-6-2023. De verwachte resterende afschrijving voor 30-06-2023 wordt berekend aan de hand van de volgende formule:

* *148/360 x 0,20 x 100.000 = 8222*

### <a name="example-4---declining-balance-1-depreciation"></a>Voorbeeld 4: boekwaarde-afschrijving 1

De boekwaarde van een activum is 100.000 op 31-12-2023. U boekt op 2-2-2023 een afschrijving van 95.000, wat hoger is dan het toegestane afschrijvingsbedrag voor het jaar. Als u afschrijving uitvoert op 30-6-2023, stelt [!INCLUDE [prod_short](includes/prod_short.md)] 5000 voor, omdat er 148 dagen zijn van 2-2-2023 tot 30-6-2023. De verwachte resterende afschrijving voor 30-06-2023 wordt berekend aan de hand van de volgende formule: 

* *148/360 x 0,20 x 100.000 = 8222*

De resterende boekwaarde is echter slechts 5000, dus [!INCLUDE [prod_short](includes/prod_short.md)] zal 5000 voorstellen, omdat een boekwaarde niet negatief kan zijn.

## <a name="declining-balance-2-depreciation"></a>Boekwaarde-afschrijving 2

Met de methoden Boekwaarde-afschrijving 1 en Boekwaarde-afschrijving 2 wordt voor ieder jaar hetzelfde totale afschrijvingsbedrag berekend. Als u de batchverwerking **Afschrijving berekenen** echter meer dan één keer per jaar uitvoert, zorgt de methode Boekwaarde-afschrijving 1 voor gelijke afschrijvingsbedragen per afschrijvingsperiode. De methode Boekwaarde-afschrijving 2 zorgt daarentegen voor afschrijvingsbedragen die bij iedere volgende afschrijvingsperiode lager worden.  

### <a name="example---declining-balance-2-depreciation"></a>Voorbeeld: boekwaarde-afschrijving 2

De aanschafkosten van een vast activum bedragen LV 100.000. Het veld **Boekwaarde afschr. %** is 25. De batchverwerking **Afschrijving berekenen** wordt elk half jaar uitgevoerd. De VA-posten zien er als volgt uit:  

| Datum     | VA-boekingssoort  | Dagen                       | Bedrag    | Boekwaarde |
| -------- | ---------------- | -------------------------  | --------- | ---------- |
| 01/01/20 |Aanschafkosten |(Begindatum afschrijving)|100,000.00 |100,000.00 |
| 06/30/20 |Afschrijvingen      |180                         |-13.397,46 | 86,602.54 |
| 12/31/20 |Afschrijvingen      |180                         |-11.602,54 | 75,000.00 |
| 06/30/21 |Afschrijvingen      |180                         |-10.048,09 | 64,951.91 |
| 31-12-21 |Afschrijvingen      |180                         |-8.701,91  | 56,250.00 |
| ...      |                  |                            |           |           |

Berekeningsmethode:  

* *BW* = Boekwaarde  
* *AD* = Aantal afschrijvingsdagen  
* *BAP* = Boekwaarde-afschrijvingspercentage  
* *P* = *DBP*/100  
* *D* = *ND*/360  

De formule voor het berekenen van de afschrijvingsbedragen luidt als volgt:  

* *AB* = *BW* x (1 – (1 –P)<sup>D</sup>)

De afschrijvingswaarden zijn:  

| Datum     | Berekening                                                |
| -------- | -----------                                                |
| 06/30/20 |AB = 100.000,00 x (1 -(1 - 0,25)<sup>0,5</sup>) = 13.397,46 |
| 12/31/20 |AB = 86.602,54 x (1 - (1 - 0,25)<sup>0,5</sup>) = 11.602,54 |
| 06/30/21 |AB = 75.000,00 x (1 - (1 - 0,25)<sup>0,5</sup>) = 10.048,09 |
| 31-12-21 |AB = 64.951,91 x (1 - (1 - 0,25)<sup>0,5</sup>) = 8.701,91  |
| ...      |                                                            |

## <a name="db1sl-depreciation"></a>BW1/Lineaire afschrijving

BW1/Lin is de afkorting voor deze combinatie van boekwaarde-afschrijving 1 en Lineair. De berekening wordt voortgezet totdat de boekwaarde gelijk is aan het maximale restbedrag na afschrijving of aan de opgegeven restwaarde.  

De batchverwerking **Afschrijving berekenen** berekent een lineair bedrag en een boekwaarde-afschrijvingsbedrag, maar alleen het hoogste bedrag van de twee wordt naar het dagboek overgebracht.  

U kunt de boekwaarde-afschrijving met meerdere percentages berekenen.  

Als u deze methode gebruikt, moet u de verwachte gebruiksduur en een boekwaarde-afschrijvingspercentage invullen op de pagina **VA-afschrijvingsboeken**.  

> [!NOTE]
> Als u een van de afschrijvingsmethoden met boekwaarde-afschrijving gebruikt en u de afschrijving over meerdere jaren wilt uitvoeren, moet u de afschrijving voor elk jaar afzonderlijk uitvoeren. Als u de afschrijving uitvoert voor de hele periode vanaf de aanschafdatum tot het einde van het laatste boekjaar of de laatste boekhoudperiode, zijn de resultaten waarschijnlijk onjuist. U kunt het bijvoorbeeld meerdere jaren uitvoeren als u verouderde gegevens hebt geïmporteerd en u de werkelijke aanschafdatums voor uw activa gebruikt en geaccumuleerde afschrijving wilt inhalen. Voor methoden met boekwaarde-afschrijving berekent [!INCLUDE [prod_short](includes/prod_short.md)] de toegestane afschrijving per jaar, te beginnen met de geregistreerde boekwaarde voor elk jaar. Het kan niet in één stap een afschrijving over meerdere jaren uitvoeren.
>
> In het rapport **Vast activum - Gesch. waarde** kunnen afschrijvingen over perioden van meerdere jaren worden geprojecteerd, wat verwarrend kan zijn in vergelijking met de resultaten die u krijgt als u afschrijvingen over meerdere jaren uitvoert met behulp van een van de methoden met boekwaarde-afschrijving. 

### <a name="example---db1-sl-depreciation"></a>Voorbeeld: boekwaarde 1/Lineaire afschrijving

De aanschafkosten van een vast activum bedragen LV 100.000. Op de pagina **VA-afschrijvingsboeken** bevat het veld **Boekwaarde afschr. %** 25, en het veld **Aantal afschr.-jaren** **8**. De batchverwerking **Afschrijving berekenen** wordt elk half jaar uitgevoerd.  

De VA-posten zien er als volgt uit:  

| Datum | VA-boekingssoort | Dagen | Bedrag | Boekwaarde |
| --- | --- | --- | --- | --- |
| 01/01/20 |Aanschafkosten |(Begindatum afschrijving) |100,000.00 |100,000.00 |
| 06/30/20 |Afschrijvingen |180 |-12.500,00 |87,500.00 |
| 12/31/20 |Afschrijvingen |180 |-12.500,00 |75,000.00 |
| 06/30/21 |Afschrijvingen |180 |-9.375,00 |65,625.00 |
| 12/31/21 |Afschrijvingen |180 |-9.375,00 |56,250.00 |
| 06/30/22 |Afschrijvingen |180 |-7.031,25 |49,218.75 |
| 12/31/22 |Afschrijvingen |180 |-7.031,25 |42,187.50 |
| 06/30/23 |Afschrijvingen |180 |-5.273,44 |36,914.06 |
| 12/31/23 |Afschrijvingen |180 |-5.273,44 |31,640.62 |
| 06/30/24 |Afschrijvingen |180 |-3.955,08 |27,685.54 |
| 12/31/24 |Afschrijvingen |180 |-3.955,08 |23,730.46 |
| 06/30/25 |Afschrijvingen |180 |-3.955,08 |19.775,38 Lin |
| 12/31/25 |Afschrijvingen |180 |-3.955,08 |15.820,30 Lin |
| 06/30/26 |Afschrijvingen |180 |-3.955,08 |11.865,22 Lin |
| 12/31/26 |Afschrijvingen |180 |-3.955,07 |7.910,15 Lin |
| 06/30/27 |Afschrijvingen |180 |-3.955,08 |3.955,07 Lin |
| 12/31/27 |Afschrijvingen |180 |-3.955,07 |0,00 Lin |

`SL` achter de boekwaarde betekent dat de lineaire afschrijvingsmethode is gebruikt.  

Berekeningsmethode:  

* Jaar 1 (2020):  

    *Boekwaarde-afschrijvingsbedrag: 25% van 100.000 = 25.000 = 12.500 + 12.500*  

    *Lineair afschrijvingsbedrag = 100.000/8 = 12.500 + 6.250 + 6.250*  

    Het boekwaarde-afschrijvingsbedrag wordt gebruikt omdat dit het hoogste bedrag is.  
* ...
* Jaar 5 (2025):  

    *Boekwaarde-afschrijvingsbedrag: 25% van 23,730.46 = 4,943.85 = 2,471.92 + 2,471.92*  

    *Lineair afschrijvingsbedrag = 23,730.46/3 = 7,910.15 + 3,995.07 + 3,995.08*  

    Het lineaire afschrijvingsbedrag wordt gebruikt, omdat dit het hoogste bedrag is.  

## <a name="half-year-convention-depreciation"></a>Afschrijving volgens halfjaarlijkse afspraak

De methode van halfjaarlijkse afspraak wordt alleen toegepast als u de schakeloptie **Halfjaarlijkse afspraak gebruiken** voor het vaste activum op de pagina **Vast activum** inschakelt.  

U kunt deze afschrijvingsmethode met de volgende afschrijvingsmethoden gebruiken:  

* Lineair  
* Boekwaarde 1  
* BW1/Lin  

Als u de methode van halfjaarlijkse afspraak toepast, heeft een vast activum een afschrijving van zes maanden in het eerste boekjaar, ongeacht de inhoud van het veld **Begindatum afschrijving**.  

> [!NOTE]  
> De verwachte levensduur van een vast activum na het eerste boekjaar, bedraagt altijd een half jaar bij de halfjaarlijkse afspraak. Om de halfjaarlijkse afspraak dus juist toe te passen, moet het veld **Einddatum afschr.** op de pagina **VA-afschrijvingsboek** altijd een datum bevatten die precies zes maanden voor de laatste datum van het boekjaar ligt waarin het vaste activum volledig wordt afgeschreven.  

### <a name="example---half-year-convention-depreciation"></a>Voorbeeld - afschrijving volgens halfjaarlijkse afspraak

De aanschafkosten van een vast activum bedragen LV 100.000. De **Begindatum afschr.** is 03-01-20. De verwachte levensduur is vijf jaar, dus de **Einddatum afschr.** moet 06-30-25 zijn. De batchverwerking **Afschrijving berekenen** wordt jaarlijks uitgevoerd. Dit voorbeeld is gebaseerd op een agendaboekjaar.  

De VA-posten zien er als volgt uit:  

| Datum | VA-boekingssoort | Dagen | Bedrag | Boekwaarde |
| --- | --- | --- | --- | --- |
| 03/01/20 |Aanschafkosten |(Begindatum afschrijving) |100,000.00 |100,000.00 |
| 12/31/20 |Afschrijvingen |270 |-10.000,00 |90,000.00 |
| 12/31/21 |Afschrijvingen |360 |-20.000,00 |70,000.00 |
| 12/31/22 |Afschrijvingen |360 |-20.000,00 |50,000.00 |
| 12/31/23 |Afschrijvingen |360 |-20.000,00 |30,000.00 |
| 12/31/24 |Afschrijvingen |360 |-20.000,00 |10,000.00 |
| 31-12-25 |Afschrijvingen |180 |-10.000,00 |  0.00 |

## <a name="example---db1sl-depreciation-using-half-year-convention"></a>Voorbeeld: boekwaarde 1/lineaire afschrijving met gebruik van halfjaarlijkse afspraak

De aanschafkosten van een vast activum bedragen LV 100.000. De **Begindatum afschr.** is 11-01-20. De verwachte levensduur is vijf jaar, dus de **Einddatum afschr.** moet 06-30-25 zijn. Het veld **Boekwaarde afschr.** op de pagina **Boekwaarde afschr. %** bevat 40. De batchverwerking **Afschrijving berekenen** wordt jaarlijks uitgevoerd. Dit voorbeeld is gebaseerd op een agendaboekjaar.  

De VA-posten zien er als volgt uit:  

| Datum | VA-boekingssoort | Dagen | Bedrag | Boekwaarde |
| --- | --- | --- | --- | --- |
| 11/01/20 |Aanschafkosten |(Begindatum afschrijving) |100,000.00 |100,000.00 |
| 12/31/20 |Afschrijvingen |60 |-20.000,00 |80,000.00 |
| 12/31/21 |Afschrijvingen |360 |-32.000,00 |48,000.00 |
| 12/31/22 |Afschrijvingen |360 |-19.200,00 |28,800.00 |
| 12/31/23 |Afschrijvingen |360 |-11.520,00 |17,280.00 |
| 12/31/24 |Afschrijvingen |360 |-11.520,00 |5.760,00 Lin |
| 12/31/25 |Afschrijvingen |180 |-5.760,00 |0,00 Lin |

`SL` achter de boekwaarde betekent dat de lineaire afschrijvingsmethode is gebruikt.  

Berekeningsmethode:  

* Jaar 1:  

    *Boekwaarde-afschrijvingsbedrag = Volledig jaarbedrag = 40% van 100.000 = 40.000.* Voor een half jaar is dit dus 40.000/2 = 20.000  

    *Lineair bedrag = Volledig jaarbedrag = 100.000/5 = 20.000.* Voor een half jaar is dit dus 20.000 / 2 = 10.000  

    Het boekwaarde-afschrijvingsbedrag wordt gebruikt omdat dit het hoogste bedrag is.  
* ...
* Jaar 5 (2024):  

    *Boekwaarde-afschrijvingsbedrag = 40% van 17.280,00 = 6.912,00*  

    *Lineair bedrag = 28.800/1,5 = 11.520,00*  

    Het lineaire afschrijvingsbedrag wordt gebruikt, omdat dit het hoogste bedrag is.  

## <a name="duplicate-entries-to-other-depreciation-books"></a>Posten dupliceren naar andere afschrijvingsboeken

Als er drie afschrijvingsboeken zijn, B1, B2 en B3, en u wilt posten uit B1 naar B2 en B3 dupliceren, schakelt u de schakeloptie **Deel van duplicatielijst** in op de kaarten voor de afschrijvingsboeken B2 en B3. Deze instelling kan bijvoorbeeld handig zijn in de volgende situaties:

* Afschrijvingsboek B1 is geïntegreerd met het grootboek en maakt gebruik van het grootboekjournaal voor vaste activa.
* Afschrijvingsboeken B2 en B3 zijn geïntegreerd met het grootboek en maken gebruik van het grootboekjournaal voor vaste activa.  

Als u een post boekt in B1 in het financieel dagboek voor vaste activa en de schakeloptie **Deel van duplicatielijst** inschakelt, dupliceert [!INCLUDE [prod_short](includes/prod_short.md)] de post naar B2 en B3 in het dagboek voor vaste activa wanneer u de post boekt.  

> [!NOTE]  
> U kunt niet in hetzelfde dagboek en dezelfde dagboekbatch dupliceren als waar u vanuit dupliceert. Als u posten in het financieel dagboek voor vaste activa boekt, kunt u deze met behulp van een andere batch dupliceren in het dagboek voor vaste activa of in het financieel dagboek voor vaste activa.  

> [!NOTE]  
> U kunt niet dezelfde nummerreeks gebruiken in het financieel dagboek voor vaste activa en het dagboek voor vaste activa. Wanneer u posten in het VA-financieel dagboek boekt, moet u het veld **Documentnr.** leeg laten. Als u een getal in het veld invoert, wordt het getal gedupliceerd in het VA-dagboek. U moet het documentnummer handmatig wijzigen voordat u het dagboek kunt boeken.  

## <a name="manual-depreciation"></a>Handmatige afschrijving

Gebruik deze handmatige methode voor activa waarop niet wordt afgeschreven, bijvoorbeeld grond. U moet afschrijving invoeren in het VA-financiële dagboek. Uit de batchverwerking **Afschrijving berekenen** worden de vaste activa weggelaten die handmatig worden afgeschreven.

## <a name="user-defined-depreciation"></a>Door de gebruiker gedefinieerde afschrijving

Als de ingebouwde afschrijvingsmethoden niet aan uw behoeften voldoen, kunt u uw eigen afschrijvingsmethode definiëren met behulp van afschrijvingstabellen. Voor informatie over het toepassen van een door de gebruiker gedefinieerde afschrijvingsmethode gaat u naar [Door de gebruiker gedefinieerde afschrijvingsmethode instellen](fa-how-setup-user-defined-depreciation-method.md).

## <a name="see-also"></a>Zie ook

[Overzicht van vaste activa](fa-manage.md)  
[Vaste activa instellen](fa-setup.md)  
[Financiën](finance.md)  
[Voorbereid zijn om zaken te doen](ui-get-ready-business.md)  
[Werken met [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
