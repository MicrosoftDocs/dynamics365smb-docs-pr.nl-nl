---
title: Waarden van klantinstellingen verzamelen | Microsoft Docs
description: U gebruikt de configuratievragenlijst om uw implementatiewerklast te verminderen door het stroomlijnen van de taak voor het instellen van het nieuwe bedrijf. U kunt de configuratievragenlijst genereren in Business Central en vervolgens als een Excel-bestand (.xlsx) of een XML-bestand aan de klant geven.
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: conceptual
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 04/01/2021
ms.author: edupont
ms.openlocfilehash: af8d2bb31b5f76912d69b123803243cfce1445bd
ms.sourcegitcommit: 766e2840fd16efb901d211d7fa64d96766ac99d9
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "5783969"
---
# <a name="gather-customer-setup-values"></a>Waarden van klantinstellingen verzamelen
U gebruikt de configuratievragenlijst om uw implementatiewerklast te verminderen door het stroomlijnen van de taak voor het instellen van het nieuwe bedrijf. U kunt de configuratievragenlijst genereren in [!INCLUDE[prod_short](includes/prod_short.md)] en vervolgens als een Excel-bestand (.xls) of een XML-bestand aan de klant geven.  

U kunt alle standaardwaarden in een vragenlijst aanpassen aan de behoeften van de klant.  

> [!TIP]  
>  Voor meer informatie over het definiëren van instellingen in voorraadplanningvelden zie [Aanbevolen procedures instellen: leveringsplanning](setup-best-practices-supply-planning.md).  

Als uw klant de vragenlijst invult, importeert u het bestand in het nieuwe [!INCLUDE[prod_short](includes/prod_short.md)]-bedrijf van de klant. U en uw klant valideren de antwoorden in de vragenlijst voordat u ze op het bedrijf toepast.

## <a name="to-create-a-configuration-questionnaire"></a>Een configuratievragenlijst maken
U kunt een vragenlijst gebruiken om de reikwijdte en de behoeften van de configuratie te bepalen. U kunt een nieuwe vragenlijst maken of een bestaande vragenlijst wijzigen door het nieuwe vragen of vraaggebieden toe te voegen.  

<!-- A configuration questionnaire has the following structure
* The name of the questionnaire itself
* Question Areas that group questions about a similar subject. For example, you might create a question area that focuses on entering company informtion. Typically, configuration questionnaires have many question groups
* Questions that are closed ended, meaning that the customer must choose an answer, and can choose only one. -->

 U kunt enkel vragenlijsten maken voor tabellen van het type instellen. U kunt bijvoorbeeld het hulpprogramma gebruiken om de volgende pagina's van informatie te voorzien:  

-   Bedrijfsgegevens  
-   VA-instellingen  
-   Grootboekinstellingen  
-   Voorraadinstelling  
-   Assemblage-instelling
-   Productie-instellingen  
-   Inkoopinstellingen  
-   Marketinginstellingen  
-   Service-instellingen  
-   Verkoopinstellingen  
-   Magazijninstellingen  

> [!NOTE]  
>  Als u een complete lijst met instellingstabellen wilt zien, kiest u het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voert u **Instelling** in en kiest u de desbetreffende koppeling. Gebruik migratiefunctionaliteit om de omvang van de migratie van recordgegevens te bepalen. Zie voor meer informatie [Klantgegevens migreren](admin-migrate-customer-data.md).  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Vragenlijst voor configuratie** in en kies de desbetreffende koppeling.  
2. Kies de actie **Nieuw**.   
3. Voer op de pagina **Vragenlijst voor configuratie** in het veld **Code** het volgende in... 
<!--4. In the **Name** field, enter...
5. Choose the **Question Areas** action. .
6. On the **Config. Question Areas** page, in the **Code** field, enter...
  
    > [!Note]  
    > The code is alphanumeric, and must start with a letter of the alphabet.
7. In the Table ID field, choose the table to which to apply the answer to the question. Your selection will determine the fields that are available for the questions, and thereby the answer selections.
  
    > [!Tip]
    > The list of table objects is long. If you know the name of the table, use **Search** in the upper left to find it in the list.
8. In the **Description** field, enter text that indicates the subject of the question group.
9. In the **No.** field, enter a number to define where the question appears in the sequence of questions.
10. In the **Field ID** field, choose the field the the customer's answer will be applied to. You can choose from the fields on the table you chose in the **Table ID** field.
  
    When you choose a field, [!INCLUDE[prod_short](includes/prod_short.md)] provides a suggestion in the **Question** field. You can edit the question if needed.
11. To add more questions to the questionnaire, repeat steps seven through 10.

> [!Tip]
> If at some point you change a question, or add a new one, choose the **Update Questions** action to update the list.

-->

3. Kies de actie **Vraaggebieden**. De pagina **Vragengebieden** wordt geopend.  
4. Kies de actie **Nieuw**. De pagina **Vragengebied voor configuratie** wordt geopend.  
5. Kies in het veld **Tabel-id** de ID van de tabel waarvoor u informatie wilt verzamelen. Het veld **Tabelnaam** wordt automatisch ingevuld.  
6. Kies de actie **Vragen bijwerken**. Elk veld in de tabel wordt toegevoegd aan de vragenlijst met een vraagteken achter het label.

U kunt het label herformuleren om duidelijk te maken hoe de vraag moet worden beantwoord. Indien een veld bijvoorbeeld de naam 'Naam' heeft, kunt u dit bewerken zodat er staat 'Wat is de naam van <data being collected>'. U kunt ook begeleiding bieden in het veld **Referentie**, inclusief een URL naar een pagina die meer informatie bevat.  

U kunt ook vragen verwijderen die u niet wilt opnemen in de vragenlijst.  

> [!NOTE]  
>  Het veld **Antwoordoptie** beschrijft het type en de indeling van het gepaste antwoord van de gegevens. Het veld **Antwoord** bevat door de gebruiker verstrekte informatie.  
>   
>  Indien nodig kunt u ook standaardantwoorden definiëren in het veld **Antwoord**. Deze waarden worden standaard gebruikt voor aangepaste installatie. De persoon die de vragenlijst invult, kan het antwoord echter wijzigen en bijwerken.  

## <a name="to-complete-the-configuration-questionnaire"></a>De configuratievragenlijst voltooien
U gebruikt de configuratievragenlijst om een uitvoerige discussie te structureren en te documenteren over de specifieke behoeften van de klant. Ook kunt u instellingsgegevens verzamelen van de klant voor het configureren van de relevante [!INCLUDE[prod_short](includes/prod_short.md)]- instellingstabellen, zoals het grootboek, voorraad en klanten.  

> [!NOTE]  
>  U kunt ook uw eigen configuratievragenlijst maken die aan uw behoeften voldoet.  

1. Open het bedrijf waarvoor u de vragenlijst wilt voltooien.
2. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Vragenlijst voor configuratie** in en kies de desbetreffende koppeling.  
3. Selecteer de vragenlijst voor het bedrijf en kies de actie **Naar Excel exporteren**, optioneel de actie **Naar XML exporteren**.
4. Laat de klant de configuratievragenlijst invullen door de antwoorden in te voeren in de Excel-werkmap. Er zijn werkbladen voor elk vraaggebied dat is gemaakt voor de vragenlijst.   
5. Sla de Excel-werkmap op als *XML-gegevens*. Kies de actie **Vanuit XML importeren** en selecteer het .xml-bestand met de antwoorden van de klant.
6. Kies de actie **Vragengebieden** om te beginnen met het valideren en toepassen van de antwoorden op de configuratievragenlijst.  

## <a name="to-complete-a-questionnaire-from-the-configuration-worksheet"></a>Een vragenlijst invullen vanuit het configuratiewerkblad  
De volgende procedure biedt een alternatieve manier om toegang te krijgen tot configuratievragenlijsten. Hierbij wordt ervan uitgegaan dat het configuratiepakket dat u hebt opgegeven vragenlijsten bevat.  

1. Open het configuratiewerkblad nadat u een configuratiepakket hebt geïmporteerd.  
2. Kies voor elke tabel waarvoor er een vragengebied is de actie **Vragen**. De vragenlijstpagina wordt geopend.  
3. Beantwoord de vragen en kies vervolgens de actie **Antwoorden toepassen**.  
4. Kies de knop **OK** om de vragenlijst te sluiten.

## <a name="to-validate-the-configuration-questionnaire"></a>De configuratievragenlijst valideren
Het is belangrijk dat u de configuratievragenlijst valideert voordat u deze toepast op de [!INCLUDE[prod_short](includes/prod_short.md)]-indeling. Het is ook een manier om te zorgen dat de opmaak blijft behouden tijdens het importeren vanuit Excel.  

Een veelvoorkomende validatietaak is te controleren dat geen tekenreeksen worden ingevoerd in datumvelden. Dit proces is nodig omdat de indeling van het antwoord op de vragenlijst niet automatisch wordt gevalideerd wanneer u de functie **Antwoorden toepassen** uitvoert.  

> [!NOTE]  
>  Validatie van de configuratievragenlijst is in het algemeen een handmatig proces. Er zijn echter controles op regionale indelingsinconsistenties. Bovendien treden er fouten op als de structuur van uw [!INCLUDE[prod_short](includes/prod_short.md)]-database niet overeenkomt met de structuur van de migratiedatabase.  

1. Selecteer op de pagina **Vragenlijst voor configuratie** de desbetreffende vragenlijst en kies de actie **Vragengebieden**.  
2. Open het betreffende vragengebied.  
3. Controleer voor elke vraag of de waarde in het veld **Antwoord** overeenkomt met de opmaak van het veld **Antwoordoptie**. Controleer bijvoorbeeld of het adres van een bedrijf in tekstindeling is.  
4. Als u fouten vindt, kunt u problemen oplossen en correcties aanbrengen in Excel door de vragenlijst te exporteren en opnieuw te importeren. U kunt fouten ook rechtstreeks in [!INCLUDE[prod_short](includes/prod_short.md)] corrigeren terwijl u de antwoorden bekijkt op de pagina **Vragengebied voor configuratie**.  
5. Herhaal deze stappen voor elk vragengebied.  

Wanneer u de validatie hebt voltooid, zijn de gegevens gereed om te worden toegepast op de database.  

## <a name="to-apply-answers-from-the-configuration-questionnaire"></a>Antwoorden uit de configuratievragenlijst toepassen
Nadat u informatie uit een configuratievragenlijst hebt geïmporteerd en gevalideerd, kunt u de installatiegegevens overbrengen naar of toepassen op de bijbehorende tabellen in de [!INCLUDE[prod_short](includes/prod_short.md)]-database.  

1. Kies het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voer **Vragenlijst voor configuratie** in en kies de desbetreffende koppeling. De pagina **Vragenlijst voor configuratie** wordt geopend.  
2. Selecteer een configuratievragenlijst in de lijst en kies vervolgens de actie **Lijst bewerken**.  
3. U kunt antwoorden op twee manieren toepassen.  

- Als u de hele vragenlijst wilt toepassen, kiest u de actie **Antwoorden toepassen**.  
- Als u antwoorden alleen voor een specifiek **Vragengebied** wilt toepassen, kiest u de actie **Vraaggebieden**, selecteert u een **Vragengebied** in de lijst en kiest u de actie **Antwoorden toepassen**.  

### <a name="to-verify-that-answers-have-been-applied-successfully"></a>Controleren dat antwoorden met succes zijn toegepast  
1. Controleer de installatiepagina's op de verschillende functionele gebieden van [!INCLUDE[prod_short](includes/prod_short.md)]. Als u de pagina wilt vinden, kiest u het pictogram ![Lampje dat de functie Vertel me opent](media/ui-search/search_small.png "Vertel me wat u wilt doen"), voert u de naam van de instellingenpagina in en kiest u de desbetreffende koppeling.  
2. Controleer of de velden zijn gevuld met de juiste gegevens uit de verschillende vragengebieden in de configuratievragenlijst.  

De installatie is nu geconfigureerd met de zakelijke gegevens en regels van de klant.

## <a name="see-also"></a>Zie ook  
[Een bedrijf instellen met RapidStart Services](admin-set-up-a-company-with-rapidstart.md)  
[Beheer](admin-setup-and-administration.md)


[!INCLUDE[footer-include](includes/footer-banner.md)]