---
title: Gegevens zoeken en filtercriteria invoeren | Microsoft Docs
description: Beschrijft hoe u met filters werkt, zoals het Snelfilter, om de resultaten te verfijnen die u krijgt wanneer u gegevens zoekt.
services: project-madeira
documentationcenter: 
author: jswymer
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: delimit, FlowFilter
ms.date: 03/29/2017
ms.author: solsen
ms.translationtype: HT
ms.sourcegitcommit: 2c13559bb3dc44cdb61697f5135c5b931e34d2a8
ms.openlocfilehash: 11d7ef56e980ba263dba6328b2f2f08b86410242
ms.contentlocale: nl-nl
ms.lasthandoff: 12/14/2017

---
# <a name="searching-filtering-and-sorting-data"></a><span data-ttu-id="c4e33-103">Gegevens zoeken, filteren en sorteren</span><span class="sxs-lookup"><span data-stu-id="c4e33-103">Searching, Filtering, and Sorting Data</span></span>
<span data-ttu-id="c4e33-104">U kunt een paar dingen doen om records in een lijst te vinden, te lokaliseren en te scannen.</span><span class="sxs-lookup"><span data-stu-id="c4e33-104">There are a few things that you can do that will help you find, pinpoint, and scan records in a list.</span></span> <span data-ttu-id="c4e33-105">U kunt de records bijvoorbeeld sorteren, doorzoeken en filteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-105">These include sorting, searching and filtering.</span></span>

<span data-ttu-id="c4e33-106">Wanneer u naar gegevens, zoals klantnamen, adressen of productgroepen wilt zoeken, voert u criteria in.</span><span class="sxs-lookup"><span data-stu-id="c4e33-106">When you want to search for data, such as customer names, addresses, or product groups, you enter criteria.</span></span> <span data-ttu-id="c4e33-107">In zoekcriteria kunt u alle cijfers en letters gebruiken die u normaal in het specifieke veld gebruikt.</span><span class="sxs-lookup"><span data-stu-id="c4e33-107">In search criteria you can use all the numbers and letters that you normally use in the specific field.</span></span> <span data-ttu-id="c4e33-108">Daarnaast kunt u speciale symbolen gebruiken om de resultaten verder te filteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-108">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="c4e33-109">U kunt op twee manieren zoeken: met het snelfilter of kolomfilters.</span><span class="sxs-lookup"><span data-stu-id="c4e33-109">There are two ways to search: using the Quick Filter or column filters.</span></span>

## <a name="sorting"></a><span data-ttu-id="c4e33-110">Sorteervolgorde</span><span class="sxs-lookup"><span data-stu-id="c4e33-110">Sorting</span></span>
<span data-ttu-id="c4e33-111">Met de sorteerfunctie krijgt u snel een overzicht van de gegevens.</span><span class="sxs-lookup"><span data-stu-id="c4e33-111">Sorting makes it easy for you to get a quick overview of your data.</span></span> <span data-ttu-id="c4e33-112">Als u veel klanten hebt, kunt u er bijvoorbeeld voor kiezen hen te sorteren op **Klantnr.**, **Klantboekingsgroep**, **Valutacode**, **Land-/regiocode** of **Btw-nummer** voor het door u gewenste overzicht.</span><span class="sxs-lookup"><span data-stu-id="c4e33-112">If you have many customers, for example, you can choose to sort them by **Customer No.**, **Customer Posting Group**, **Currency Code**, **Country Region Code**, or **Sales Tax Registration No.** to get the overview you need.</span></span>

<span data-ttu-id="c4e33-113">Als u een lijst wilt sorteren, kunt u een kolomkoptekst kiezen om te schakelen tussen op- en aflopend, of de kleine pijl-omlaag in de kolomkop kiezen en vervolgens **Oplopend** of **Aflopend** kiezen.</span><span class="sxs-lookup"><span data-stu-id="c4e33-113">To sort a list, you can either choose a column heading text to toggle between ascending and descending order, or choose the small downs arrow in the column heading, and then choose **Ascending** or **Descending**.</span></span>  

> [!NOTE]  
>   <span data-ttu-id="c4e33-114">Sorteren wordt niet ondersteund bij afbeeldingen, BLOB-velden, FlowFilters en velden die niet deel van een tabel zijn.</span><span class="sxs-lookup"><span data-stu-id="c4e33-114">Sorting is not supported images, BLOB fields, FlowFilters, and fields that do not belong to a table.</span></span>  

## <a name="searching-by-using-the-quick-filter"></a><span data-ttu-id="c4e33-115">Zoeken met het snelfilter</span><span class="sxs-lookup"><span data-stu-id="c4e33-115">Searching by using the Quick Filter</span></span>
<span data-ttu-id="c4e33-116">U kunt filters toevoegen aan alle pagina's met het Snelfilter.</span><span class="sxs-lookup"><span data-stu-id="c4e33-116">You can add filters to all pages by using the Quick Filter.</span></span> <span data-ttu-id="c4e33-117">Het Snelfilter wordt ingeschakeld door het vergrootglaspictogram in de rechterbovenhoek van een pagina te kiezen.</span><span class="sxs-lookup"><span data-stu-id="c4e33-117">The Quick Filter is enabled by choosing the magnifier icon in the top right corner of a page.</span></span> <span data-ttu-id="c4e33-118">Dit type filter wordt gebruikt voor een snelle invoer van criteria.</span><span class="sxs-lookup"><span data-stu-id="c4e33-118">This filtering type is used for a fast entry of criteria.</span></span>

> [!IMPORTANT]  
>   <span data-ttu-id="c4e33-119">Het snelfilter biedt een eenvoudig toegang tot filtergegevens door onbewerkte tekst in te voeren, maar biedt ook veel opties voor zoekcriteria.</span><span class="sxs-lookup"><span data-stu-id="c4e33-119">The Quick Filter provides an easy access to filter data by entering plain text, but does also provide a lot of search criteria options.</span></span> <span data-ttu-id="c4e33-120">Afhankelijk van of u normale tekst of tekst met symbolen invoert, werkt het snelfilter anders.</span><span class="sxs-lookup"><span data-stu-id="c4e33-120">Depending on whether you enter plain text or text including symbols, the Quick Filter behaves differently.</span></span>  

* <span data-ttu-id="c4e33-121">Als u gewone tekst in de zoekcriteria opgeeft, worden de zoekcriteria geïnterpreteerd als een hoofdletterongevoelige zoekactie die bepaalde tekst bevat.</span><span class="sxs-lookup"><span data-stu-id="c4e33-121">If you enter plain text in the search criteria, the search criteria is interpreted as a case insensitive search that contains certain text.</span></span>  
* <span data-ttu-id="c4e33-122">Als u tekst inclusief symbolen in de zoekcriteria opgeeft, worden de zoekcriteria precies zo geïnterpreteerd als u ze hebt ingevoerd en wordt onderscheid gemaakt tussen hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="c4e33-122">If you enter text including symbols in the search criteria, the search criteria is interpreted exactly as you entered it, and the search is case sensitive.</span></span>

### <a name="quick-filter-criteria"></a><span data-ttu-id="c4e33-123">Snelfiltercriteria</span><span class="sxs-lookup"><span data-stu-id="c4e33-123">Quick filter criteria</span></span>
<!-- html syntax because symbols conflict with MarkDown syntax -->
<TABLE>
  <TR>
    <TH><span data-ttu-id="c4e33-124">Zoekcriteria</span><span class="sxs-lookup"><span data-stu-id="c4e33-124">Search Criteria</span></span></TH>
    <TH><span data-ttu-id="c4e33-125">Geïnterpreteerd als...</span><span class="sxs-lookup"><span data-stu-id="c4e33-125">Interpreted as...</span></span></TH>
    <TH><span data-ttu-id="c4e33-126">Retourneert...</span><span class="sxs-lookup"><span data-stu-id="c4e33-126">Returns...</span></span></TH>
  </TR>
  <TR>
    <TD><span data-ttu-id="c4e33-127">man</span><span class="sxs-lookup"><span data-stu-id="c4e33-127">man</span></span></TD>
    <TD><span data-ttu-id="c4e33-128">@&#42;man&#42;</span><span class="sxs-lookup"><span data-stu-id="c4e33-128">@&#42;man&#42;</span></span></TD>
    <TD><span data-ttu-id="c4e33-129">Alle records met de tekst <b>man</b> en ongevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="c4e33-129">All records that contain the text <b>man</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="c4e33-130">se</span><span class="sxs-lookup"><span data-stu-id="c4e33-130">se</span></span></TD>
    <TD><span data-ttu-id="c4e33-131">@&#42;zo&#42;</span><span class="sxs-lookup"><span data-stu-id="c4e33-131">@&#42;se&#42;</span></span></TD>
    <TD><span data-ttu-id="c4e33-132">Alle records met de tekst <b>se</b> en ongevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="c4e33-132">All records that contain the text <b>se</b> and case insensitive.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="c4e33-133">Man&#42;</span><span class="sxs-lookup"><span data-stu-id="c4e33-133">Man&#42;</span></span></TD>
    <TD><span data-ttu-id="c4e33-134">Begint met <b>Man</b> en is hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="c4e33-134">Starts with <b>Man</b> and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="c4e33-135">Alle records die beginnen met de tekst <b>Man</b>.</span><span class="sxs-lookup"><span data-stu-id="c4e33-135">All records that start with the text <b>Man</b>.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="c4e33-136">'man'</span><span class="sxs-lookup"><span data-stu-id="c4e33-136">'man'</span></span></TD>
    <TD><span data-ttu-id="c4e33-137">Een exacte tekst en gevoelig voor hoofdletters en kleine letters.</span><span class="sxs-lookup"><span data-stu-id="c4e33-137">An exact text and case sensitive.</span></span></TD>
    <TD><span data-ttu-id="c4e33-138">Alle records die precies overeenkomen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="c4e33-138">All records that match <b>man</b> exactly.</span></span></TD>
  </TR>
  <TR>
    <TD><span data-ttu-id="c4e33-139">@man\*</span><span class="sxs-lookup"><span data-stu-id="c4e33-139">@man\*</span></span> </TD>
    <TD><span data-ttu-id="c4e33-140">Begint met en is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="c4e33-140">Starts with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="c4e33-141">Alle records die beginnen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="c4e33-141">All records that start with <b>man</b>.</span></span></TD>
  </TR>
    <TR>
    <TD><span data-ttu-id="c4e33-142">@&#42;man</span><span class="sxs-lookup"><span data-stu-id="c4e33-142">@&#42;man</span></span></TD>
    <TD><span data-ttu-id="c4e33-143">Eindigt met en is niet hoofdlettergevoelig.</span><span class="sxs-lookup"><span data-stu-id="c4e33-143">Ends with and case insensitive.</span></span></TD>
    <TD><span data-ttu-id="c4e33-144">Alle records die eindigen met <b>man</b>.</span><span class="sxs-lookup"><span data-stu-id="c4e33-144">All records that end with <b>man</b>.</span></span></TD>
  </TR>
</TABLE>

> [!NOTE]  
>   <span data-ttu-id="c4e33-145">U kunt geen jokerteken gebruiken bij het filteren op opsommingsvelden, zoals het veld **Status** op verkooporders.</span><span class="sxs-lookup"><span data-stu-id="c4e33-145">You cannot use a wildcard when filtering on enumeration fields, such as the **Status** field on sales orders.</span></span> <span data-ttu-id="c4e33-146">Om een filter voor deze veldsoort in te voeren, kunt u de numerieke waarde als een filterparameter invoeren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-146">To enter a filter for this type of field, you can enter the numeric value as a filtering parameter.</span></span> <span data-ttu-id="c4e33-147">Bijvoorbeeld: gebruik in het veld **Status** op een verkooporder met de waarden **Open**, **Vrijgegeven**, **Wacht op goedkeuring** en **Wacht op vooruitbetaling** de waarden **0**, **1**, **2** en **3** om voor deze opties te filteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-147">For example, in the **Status** field on a sales order that has the values **Open**, **Released**, **Pending Approval**, and **Pending Prepayment**, use the values **0**, **1**, **2**, and **3** to filter for these options.</span></span> 

## <a name="searching-by-using-column-filters"></a><span data-ttu-id="c4e33-148">Zoeken met kolomfilters</span><span class="sxs-lookup"><span data-stu-id="c4e33-148">Searching by using column Filters</span></span>
<span data-ttu-id="c4e33-149">U kunt een filter toevoegen aan een of meer kolommen in een lijst.</span><span class="sxs-lookup"><span data-stu-id="c4e33-149">You can add a filter on one or more columns in a list.</span></span> <span data-ttu-id="c4e33-150">Kolomfilters bieden een meer flexibele en geavanceerde methode dan het snelfilter.</span><span class="sxs-lookup"><span data-stu-id="c4e33-150">Filtering on columns is more flexible and enhanced than the Quick Filter.</span></span> 

### <a name="to-add-a-filter-on-a-column"></a><span data-ttu-id="c4e33-151">Een filter toevoegen aan een kolom</span><span class="sxs-lookup"><span data-stu-id="c4e33-151">To add a filter on a column</span></span>
1.  <span data-ttu-id="c4e33-152">Voordat u een filter toevoegt, klikt u op het pictogram ![Als overzicht weergeven](media/ui_show_as_list_icon.png "pijl-links Als overzicht weergeven") om de weergave te wijzigen.</span><span class="sxs-lookup"><span data-stu-id="c4e33-152">Before you add a filter, choose ![Show as list](media/ui_show_as_list_icon.png "Show as list arrow left") icon to change to the list view.</span></span>
2. <span data-ttu-id="c4e33-153">Kies de pijl-omlaag in de kolomkop en kies **Filter**.</span><span class="sxs-lookup"><span data-stu-id="c4e33-153">Choose the downwards arrow in the column heading, and then choose **Filter**.</span></span>
3. <span data-ttu-id="c4e33-154">Ga op een van de volgende manieren te werk:</span><span class="sxs-lookup"><span data-stu-id="c4e33-154">Do one of the following:</span></span> 
  -  <span data-ttu-id="c4e33-155">Kies *...* naast het vak om een waarde in de lijst te selecteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-155">Choose *...* next to the box to select a value from a list.</span></span>
  -  <span data-ttu-id="c4e33-156">Voer filtercriteria in het vak in.</span><span class="sxs-lookup"><span data-stu-id="c4e33-156">Enter filter criteria in the box.</span></span> <span data-ttu-id="c4e33-157">Zie het volgende gedeelte voor details.</span><span class="sxs-lookup"><span data-stu-id="c4e33-157">See the next section for details.</span></span>
4. <span data-ttu-id="c4e33-158">Kies de knop **OK**.</span><span class="sxs-lookup"><span data-stu-id="c4e33-158">Choose the **OK** button.</span></span>

## <a name="filter-criteria-and-symbols"></a><span data-ttu-id="c4e33-159">Filtercriteria en -symbolen</span><span class="sxs-lookup"><span data-stu-id="c4e33-159">Filter criteria and symbols</span></span>
<span data-ttu-id="c4e33-160">U kunt bij de invoer van criteria alle cijfers en letters gebruiken die u normaal ook kunt gebruiken.</span><span class="sxs-lookup"><span data-stu-id="c4e33-160">When you enter criteria, you can use all the numbers and letters that you can normally use in the field.</span></span> <span data-ttu-id="c4e33-161">Daarnaast kunt u speciale symbolen gebruiken om de resultaten verder te filteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-161">In addition, you can use special symbols to further filter the results.</span></span> <span data-ttu-id="c4e33-162">De volgende tabellen bevatten de tekens die in filters kunnen worden gebruikt.</span><span class="sxs-lookup"><span data-stu-id="c4e33-162">The following tables show the symbols which can be used in filters.</span></span>  
  
> [!IMPORTANT]  
>  <span data-ttu-id="c4e33-163">Het kan voorkomen dat veldwaarden deze symbolen bevatten en u hierop wilt filteren.</span><span class="sxs-lookup"><span data-stu-id="c4e33-163">There may be instances where field values contain these symbols and you want to filter on them.</span></span> <span data-ttu-id="c4e33-164">Hiervoor moet u de filterexpressie opnemen die het symbool tussen aanhalingstekens (“) bevat.</span><span class="sxs-lookup"><span data-stu-id="c4e33-164">To do this, you must include the filter expression that contains the symbol in quotation marks ('').</span></span> <span data-ttu-id="c4e33-165">Als u wilt filteren op records die beginnen met de tekst *S&R*, is de filterexpressie bijvoorbeeld **'S&R\*'**.</span><span class="sxs-lookup"><span data-stu-id="c4e33-165">For example, if you want to filter on records that start with the text *S&R*, the filter expression is **'S&R\*'**.</span></span>  
  
### <a name="-interval"></a><span data-ttu-id="c4e33-166">(..) Interval</span><span class="sxs-lookup"><span data-stu-id="c4e33-166">(..) Interval</span></span>  
  
|<span data-ttu-id="c4e33-167">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-167">Sample Expression</span></span>|<span data-ttu-id="c4e33-168">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-168">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-169">1.100..2.100</span><span class="sxs-lookup"><span data-stu-id="c4e33-169">1100..2100</span></span>|<span data-ttu-id="c4e33-170">Nummers 1100 t/m 2100</span><span class="sxs-lookup"><span data-stu-id="c4e33-170">Numbers 1100 through 2100</span></span>|  
|<span data-ttu-id="c4e33-171">..2.500</span><span class="sxs-lookup"><span data-stu-id="c4e33-171">..2500</span></span>|<span data-ttu-id="c4e33-172">Tot en met 2500</span><span class="sxs-lookup"><span data-stu-id="c4e33-172">Up to and including 2500</span></span>|  
|<span data-ttu-id="c4e33-173">..31 12 00</span><span class="sxs-lookup"><span data-stu-id="c4e33-173">..12 31 00</span></span>|<span data-ttu-id="c4e33-174">Datums tot en met 31.12.00</span><span class="sxs-lookup"><span data-stu-id="c4e33-174">Dates up to and including 12 31 00</span></span>|  
|<span data-ttu-id="c4e33-175">P8..</span><span class="sxs-lookup"><span data-stu-id="c4e33-175">P8..</span></span>|<span data-ttu-id="c4e33-176">Gegevens voor boekhoudperiode 8 en verder</span><span class="sxs-lookup"><span data-stu-id="c4e33-176">Information for accounting period 8 and thereafter</span></span>|  
|<span data-ttu-id="c4e33-177">..23</span><span class="sxs-lookup"><span data-stu-id="c4e33-177">..23</span></span>|<span data-ttu-id="c4e33-178">Van begindatum tot 23 lopende maand, lopend jaar 23:59:59</span><span class="sxs-lookup"><span data-stu-id="c4e33-178">From the beginning date until 23-current month-current year 23:59:59</span></span>|  
|<span data-ttu-id="c4e33-179">23..</span><span class="sxs-lookup"><span data-stu-id="c4e33-179">23..</span></span>|<span data-ttu-id="c4e33-180">Van 23 lopende maand, lopend jaar 00:00:00 tot eindtijd</span><span class="sxs-lookup"><span data-stu-id="c4e33-180">From 23-current month-current year 0:00:00 until the end of time</span></span>|  
|<span data-ttu-id="c4e33-181">22..23</span><span class="sxs-lookup"><span data-stu-id="c4e33-181">22..23</span></span>|<span data-ttu-id="c4e33-182">Van 22 lopende maand, lopend jaar 0:00:00 tot 23 lopende maand, lopend jaar 23:59:59</span><span class="sxs-lookup"><span data-stu-id="c4e33-182">From 22-current month-current year 0:00:00 until 23-current month-current year 23:59:59</span></span>|  
  
### <a name="124-eitheror"></a><span data-ttu-id="c4e33-183">(&#124;) Of/of</span><span class="sxs-lookup"><span data-stu-id="c4e33-183">(&#124;) Either/or</span></span>  
  
|<span data-ttu-id="c4e33-184">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-184">Sample Expression</span></span>|<span data-ttu-id="c4e33-185">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-185">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-186">1200&#124;1300</span><span class="sxs-lookup"><span data-stu-id="c4e33-186">1200&#124;1300</span></span>|<span data-ttu-id="c4e33-187">Nummers met 1200 of 1300</span><span class="sxs-lookup"><span data-stu-id="c4e33-187">Numbers with 1200 or 1300</span></span>|  
  
### <a name="-not-equal-to"></a><span data-ttu-id="c4e33-188">(<>) Niet gelijk aan</span><span class="sxs-lookup"><span data-stu-id="c4e33-188">(<>) Not equal to</span></span>  
  
|<span data-ttu-id="c4e33-189">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-189">Sample Expression</span></span>|<span data-ttu-id="c4e33-190">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-190">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-191"><>0</span><span class="sxs-lookup"><span data-stu-id="c4e33-191"><>0</span></span>|<span data-ttu-id="c4e33-192">Alle nummers behalve 0</span><span class="sxs-lookup"><span data-stu-id="c4e33-192">All numbers except 0</span></span><br /><br /> <span data-ttu-id="c4e33-193">Met de SQL Server-optie kunt u dit teken combineren met jokertekens.</span><span class="sxs-lookup"><span data-stu-id="c4e33-193">The SQL Server Option allows you to combine this symbol with a wild card expression.</span></span> <span data-ttu-id="c4e33-194"><>A\* betekent bijvoorbeeld 'Niet gelijk aan tekst die begint met A'.</span><span class="sxs-lookup"><span data-stu-id="c4e33-194">For example, <>A\* meaning not equal to any text that starts with A.</span></span>|  
  
### <a name="-greater-than"></a><span data-ttu-id="c4e33-195">(>) Groter dan</span><span class="sxs-lookup"><span data-stu-id="c4e33-195">(>) Greater than</span></span>  
  
|<span data-ttu-id="c4e33-196">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-196">Sample Expression</span></span>|<span data-ttu-id="c4e33-197">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-197">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-198">>1.200</span><span class="sxs-lookup"><span data-stu-id="c4e33-198">>1200</span></span>|<span data-ttu-id="c4e33-199">Nummers groter dan 1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-199">Numbers greater than 1200</span></span>|  
  
### <a name="-greater-than-or-equal-to"></a><span data-ttu-id="c4e33-200">(>=) Groter dan of gelijk aan</span><span class="sxs-lookup"><span data-stu-id="c4e33-200">(>=) Greater than or equal to</span></span>  
  
|<span data-ttu-id="c4e33-201">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-201">Sample Expression</span></span>|<span data-ttu-id="c4e33-202">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-202">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-203">>=1.200</span><span class="sxs-lookup"><span data-stu-id="c4e33-203">>=1200</span></span>|<span data-ttu-id="c4e33-204">Nummers groter dan of gelijk aan 1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-204">Numbers greater than or equal to 1200</span></span>|  
  
### <a name="-less-than"></a><span data-ttu-id="c4e33-205">(<) Kleiner dan</span><span class="sxs-lookup"><span data-stu-id="c4e33-205">(<) Less than</span></span>  
  
|<span data-ttu-id="c4e33-206">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-206">Sample Expression</span></span>|<span data-ttu-id="c4e33-207">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-207">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-208"><1.200</span><span class="sxs-lookup"><span data-stu-id="c4e33-208"><1200</span></span>|<span data-ttu-id="c4e33-209">Nummers kleiner dan 1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-209">Numbers less than 1200</span></span>|  
  
### <a name="-less-than-or-equal-to"></a><span data-ttu-id="c4e33-210">(<=) Kleiner dan of gelijk aan</span><span class="sxs-lookup"><span data-stu-id="c4e33-210">(<=) Less than or equal to</span></span>  
  
|<span data-ttu-id="c4e33-211">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-211">Sample Expression</span></span>|<span data-ttu-id="c4e33-212">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-212">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-213"><=1.200</span><span class="sxs-lookup"><span data-stu-id="c4e33-213"><=1200</span></span>|<span data-ttu-id="c4e33-214">Nummers kleiner dan of gelijk aan 1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-214">Numbers less than or equal to 1200</span></span>|  
  
### <a name="-and"></a><span data-ttu-id="c4e33-215">(&) En</span><span class="sxs-lookup"><span data-stu-id="c4e33-215">(&) And</span></span>  
  
|<span data-ttu-id="c4e33-216">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-216">Sample Expression</span></span>|<span data-ttu-id="c4e33-217">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-217">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-218">>200&<1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-218">>200&<1200</span></span>|<span data-ttu-id="c4e33-219">Getallen groter dan 200 en kleiner dan 1200</span><span class="sxs-lookup"><span data-stu-id="c4e33-219">Numbers greater than 200 and less than 1200</span></span>|  
  
### <a name="-an-exact-character-match"></a><span data-ttu-id="c4e33-220">('') Een exacte tekenovereenkomst</span><span class="sxs-lookup"><span data-stu-id="c4e33-220">('') An exact character match</span></span>  
  
|<span data-ttu-id="c4e33-221">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-221">Sample Expression</span></span>|<span data-ttu-id="c4e33-222">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-222">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-223">'man'</span><span class="sxs-lookup"><span data-stu-id="c4e33-223">'man'</span></span>|<span data-ttu-id="c4e33-224">Tekst die exact overeenkomt met man en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="c4e33-224">Text that matches man exactly and is case sensitive.</span></span>|  
  
### <a name="-case-insensitive"></a><span data-ttu-id="c4e33-225">(@) Niet hoofdlettergevoelig</span><span class="sxs-lookup"><span data-stu-id="c4e33-225">(@) Case insensitive</span></span>  
  
|<span data-ttu-id="c4e33-226">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-226">Sample Expression</span></span>|<span data-ttu-id="c4e33-227">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-227">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-228">@man\*</span><span class="sxs-lookup"><span data-stu-id="c4e33-228">@man\*</span></span>|<span data-ttu-id="c4e33-229">Tekst die begint met man en niet hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="c4e33-229">Text that starts with man and is case insensitive.</span></span>|  
  
### <a name="-an-indefinite-number-of-unknown-characters"></a><span data-ttu-id="c4e33-230">(\*) Een onbeperkt aantal onbekende tekens</span><span class="sxs-lookup"><span data-stu-id="c4e33-230">(\*) An indefinite number of unknown characters</span></span>  
  
|<span data-ttu-id="c4e33-231">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-231">Sample Expression</span></span>|<span data-ttu-id="c4e33-232">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-232">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-233">*Co*</span><span class="sxs-lookup"><span data-stu-id="c4e33-233">*Co*</span></span>|<span data-ttu-id="c4e33-234">Tekst die “Co“ bevat en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="c4e33-234">Text that contains "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="c4e33-235">\*Be</span><span class="sxs-lookup"><span data-stu-id="c4e33-235">\*Co</span></span>|<span data-ttu-id="c4e33-236">Tekst die eindigt met “Co“ en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="c4e33-236">Text that ends with "Co" and is case sensitive.</span></span>|  
|<span data-ttu-id="c4e33-237">Be\*</span><span class="sxs-lookup"><span data-stu-id="c4e33-237">Co\*</span></span>|<span data-ttu-id="c4e33-238">Tekst die begint met “Co“ en hoofdlettergevoelig is.</span><span class="sxs-lookup"><span data-stu-id="c4e33-238">Text that begins with "Co" and is case sensitive.</span></span>|  
  
### <a name="-one-unknown-character"></a><span data-ttu-id="c4e33-239">(?) Een onbekend teken</span><span class="sxs-lookup"><span data-stu-id="c4e33-239">(?) One unknown character</span></span>  
  
|<span data-ttu-id="c4e33-240">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-240">Sample Expression</span></span>|<span data-ttu-id="c4e33-241">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-241">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-242">Jans?n</span><span class="sxs-lookup"><span data-stu-id="c4e33-242">Hans?n</span></span>|<span data-ttu-id="c4e33-243">Tekst zoals Jansen of Jansma</span><span class="sxs-lookup"><span data-stu-id="c4e33-243">Text such as Hansen or Hanson</span></span>|  
  
### <a name="combined-format-expressions"></a><span data-ttu-id="c4e33-244">Gecombineerde notatiesoorten</span><span class="sxs-lookup"><span data-stu-id="c4e33-244">Combined format expressions</span></span>  
  
|<span data-ttu-id="c4e33-245">Voorbeeld</span><span class="sxs-lookup"><span data-stu-id="c4e33-245">Sample Expression</span></span>|<span data-ttu-id="c4e33-246">Weergegeven records</span><span class="sxs-lookup"><span data-stu-id="c4e33-246">Records Displayed</span></span>|  
|-----------------------|-----------------------|  
|<span data-ttu-id="c4e33-247">5999&#124;8100..8490</span><span class="sxs-lookup"><span data-stu-id="c4e33-247">5999&#124;8100..8490</span></span>|<span data-ttu-id="c4e33-248">Alle records met het nummer 5999 of een nummer uit het interval 8100 tot en met 8490.</span><span class="sxs-lookup"><span data-stu-id="c4e33-248">Include any records with the number 5999 or a number from the interval 8100 through 8490.</span></span>|  
|<span data-ttu-id="c4e33-249">..1299&#124;1400..</span><span class="sxs-lookup"><span data-stu-id="c4e33-249">..1299&#124;1400..</span></span>|<span data-ttu-id="c4e33-250">Records met een nummer kleiner dan of gelijk aan 1299 of gelijk aan 1400 en hoger. Met andere woorden: alle nummers behalve 1300 tot en met 1399.</span><span class="sxs-lookup"><span data-stu-id="c4e33-250">Include records with a number less than or equal to 1299 or a number equal to 1400 or greater (all numbers except 1300 through 1399).</span></span>|  
|<span data-ttu-id="c4e33-251">>50&<100</span><span class="sxs-lookup"><span data-stu-id="c4e33-251">>50&<100</span></span>|<span data-ttu-id="c4e33-252">Records met een nummer groter dan 50 en kleiner dan 100, ofwel nummer 51 tot en met 99.</span><span class="sxs-lookup"><span data-stu-id="c4e33-252">Include records with numbers that are greater than 50 and less than 100 (numbers 51 through 99).</span></span>|  
 
## <a name="see-also"></a><span data-ttu-id="c4e33-253">Zie ook</span><span class="sxs-lookup"><span data-stu-id="c4e33-253">See Also</span></span>
<span data-ttu-id="c4e33-254">[Werken met [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span><span class="sxs-lookup"><span data-stu-id="c4e33-254">[Working with [!INCLUDE[d365fin](includes/d365fin_md.md)]](ui-work-product.md)</span></span>

