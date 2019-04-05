---
title: 'Ontwerpdetails: Bestelbeleid | Microsoft Docs'
description: In dit onderwerp wordt een overzicht van het beleid voor artikelaanvulling gegeven.
services: project-madeira
documentationcenter: ''
author: SorenGP
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: ''
ms.date: 10/01/2018
ms.author: sgroespe
redirect_url: design-details-handling-reordering-policies
ms.openlocfilehash: 4aaef129da953596632b56716eaff2f0c47736f7
ms.sourcegitcommit: 1bcfaa99ea302e6b84b8361ca02730b135557fc1
ms.translationtype: HT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/08/2019
ms.locfileid: "793958"
---
# <a name="design-details-reordering-policies"></a><span data-ttu-id="469c4-103">Ontwerpdetails: Bestelbeleid</span><span class="sxs-lookup"><span data-stu-id="469c4-103">Design Details: Reordering Policies</span></span>
<span data-ttu-id="469c4-104">Met het bestelbeleid wordt bepaald hoeveel wordt besteld wanneer het artikel moet worden aangevuld.</span><span class="sxs-lookup"><span data-stu-id="469c4-104">Reordering policies define how much to order when the item needs to be replenished.</span></span> <span data-ttu-id="469c4-105">Er zijn vier verschillende soorten bestelbeleid.</span><span class="sxs-lookup"><span data-stu-id="469c4-105">Four different reordering policies exist.</span></span>  

## <a name="fixed-reorder-qty"></a><span data-ttu-id="469c4-106">Vast bestelaantal</span><span class="sxs-lookup"><span data-stu-id="469c4-106">Fixed Reorder Qty.</span></span>
<span data-ttu-id="469c4-107">Het beleid Vast bestelaantal is gerelateerd aan de voorraadplanning van typische C-producten (lage voorraadkosten, laag verouderingsrisico en/of veel artikelen).</span><span class="sxs-lookup"><span data-stu-id="469c4-107">The Fixed Reorder Qty. policy is related to inventory planning of typical C-items (low inventory cost, low risk of obsolescence, and/or many items).</span></span> <span data-ttu-id="469c4-108">Dit beleid wordt gewoonlijk gebruikt in relatie met een bestelpunt met de verwachte vraag tijdens de doorlooptijd van het artikel.</span><span class="sxs-lookup"><span data-stu-id="469c4-108">This policy is usually used in connection with a reorder point reflecting the anticipated demand during the lead time of the item.</span></span>  

### <a name="calculated-per-time-bucket"></a><span data-ttu-id="469c4-109">Berekend per tijdsinterval</span><span class="sxs-lookup"><span data-stu-id="469c4-109">Calculated per Time Bucket</span></span>  
 <span data-ttu-id="469c4-110">Als het planningssysteem ontdekt dat het bestelpunt in een bepaald tijdsinterval (bestelfrequentie) is bereikt of overschreden - boven of op het bestelpunt aan het begin van de periode en onder of op het bestelpunt aan het einde van de periode - wordt voorgesteld een nieuwe voorzieningenorder voor het opgegeven bestelaantal te maken en deze voorwaarts te plannen vanaf de eerste datum na het einde van het tijdsinterval.</span><span class="sxs-lookup"><span data-stu-id="469c4-110">If the planning system detects that the reorder point has been reached or crossed in a given time bucket (reorder cycle) – above or on the reorder point at the start of the period and below or on the reorder point at the end of the period – it will suggest to create a new supply order of the specified reorder quantity and forward schedule it from the first date after the end of the time bucket.</span></span>  

 <span data-ttu-id="469c4-111">Door bestelpunten in combinatie met tijdsintervallen te gebruiken, wordt het aantal voorzieningsvoorstellen verminderd.</span><span class="sxs-lookup"><span data-stu-id="469c4-111">The bucketed reorder point concept reduces the number of supply suggestions.</span></span> <span data-ttu-id="469c4-112">Dit geeft een handmatig proces aan van het frequent door het magazijn lopen om de werkelijke inhoud in de verschillende opslaglocaties te controleren.</span><span class="sxs-lookup"><span data-stu-id="469c4-112">This reflects a manual process of frequently walking through the warehouse to check the actual contents in the various bins.</span></span>  

### <a name="creates-only-necessary-supply"></a><span data-ttu-id="469c4-113">Maakt alleen benodigde voorzieningen</span><span class="sxs-lookup"><span data-stu-id="469c4-113">Creates only Necessary Supply</span></span>  
 <span data-ttu-id="469c4-114">Voordat een nieuwe voorzieningenorder wordt voorgesteld om aan een bestelpunt te voldoen, controleert het planningssysteem of al voorziening is besteld voor ontvangst binnen de doorlooptijd van het artikel.</span><span class="sxs-lookup"><span data-stu-id="469c4-114">Before suggesting a new supply order to meet a reorder point, the planning system checks if supply has already been ordered to be received within the item’s lead time.</span></span> <span data-ttu-id="469c4-115">Als een bestaande voorzieningenorder het probleem oplost door de geplande voorraad binnen de looptijd op of boven het bestelpunt te brengen, stelt het systeem geen nieuwe voorzieningenorder voor.</span><span class="sxs-lookup"><span data-stu-id="469c4-115">If an existing supply order will solve the problem by bringing the projected inventory to or above the reorder point within the lead time, the system will not suggest a new supply order.</span></span>  

 <span data-ttu-id="469c4-116">Orders voor voorzieningen die specifiek zijn gemaakt om te voldoen aan een bestelpunt, worden uitgesloten van de normale afstemming van voorzieningen en kunnen op geen enkele manier achteraf worden gewijzigd.</span><span class="sxs-lookup"><span data-stu-id="469c4-116">Supply orders that are created specifically to meet a reorder point is excluded from ordinary supply balancing, and will not in any way be changed afterwards.</span></span> <span data-ttu-id="469c4-117">Dus als een artikel dat het bestelpunt gebruikt, moet worden uitgefaseerd (niet aangevuld), is het raadzaam openstaande orders voor voorzieningen handmatig te controleren of het bestelbeleid te wijzigen in lot-voor-lot, waarbij het systeem overbodige voorzieningen reduceert of annuleert.</span><span class="sxs-lookup"><span data-stu-id="469c4-117">Consequently, if an item using reorder point is to be phased out (not replenished), it is advisable to review outstanding supply orders manually or change the reordering policy to Lot-for-Lot, whereby the system will reduce or cancel superfluous supply.</span></span>  

### <a name="combines-with-order-modifiers"></a><span data-ttu-id="469c4-118">Combineert met orderaanpassingsfuncties</span><span class="sxs-lookup"><span data-stu-id="469c4-118">Combines with Order Modifiers</span></span>  
 <span data-ttu-id="469c4-119">De ordervelden Min. bestelaantal, Max. bestelaantal en Vaste lotgrootte zouden geen grote rol moeten afspelen wanneer het beleid voor vaste bestelaantallen wordt gebruikt.</span><span class="sxs-lookup"><span data-stu-id="469c4-119">The order modifiers, Minimum Order Quantity, Maximum Order Quantity, and Order Multiple, should not play a big role when the fixed reorder quantity policy is used.</span></span> <span data-ttu-id="469c4-120">Het planningssysteem houdt echter toch rekening met deze wijzigingsfactoren en verlaagt het aantal tot het opgegeven maximum orderaantal (en maakt twee of meer voorzieningen om het totale orderaantal te bereiken), verhoogt de order tot het opgegeven maximum aantal of rondt het orderaantal af op een opgegeven orderveelvoud.</span><span class="sxs-lookup"><span data-stu-id="469c4-120">However, the planning system still takes these modifiers into account and will decrease the quantity to the specified maximum order quantity (and create two or more supplies in order to reach the total order quantity), increase the order to the specified minimum order quantity, or round the order quantity up to meet a specified order multiple.</span></span>  

### <a name="combines-with-calendars"></a><span data-ttu-id="469c4-121">Combineert met agenda's</span><span class="sxs-lookup"><span data-stu-id="469c4-121">Combines with Calendars</span></span>  
 <span data-ttu-id="469c4-122">Voordat het planningssysteem een nieuwe voorzieningenorder voorstelt, wordt gecontroleerd of de order is gepland voor een niet-werkdag, volgens agenda's die zijn gedefinieerd in het veld **Basisagendacode** op de pagina's **Bedrijfsgegevens** en **Vestiging**.</span><span class="sxs-lookup"><span data-stu-id="469c4-122">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.</span></span>  

 <span data-ttu-id="469c4-123">Als de verwachte datum een vrije dag is, verplaatst het planningssysteem de order voorwaarts naar de dichtstbijzijnde werkdatum.</span><span class="sxs-lookup"><span data-stu-id="469c4-123">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="469c4-124">Dit kan resulteren in een order die voldoet een bestelpunt maar aan een bepaalde vraag niet voldoet.</span><span class="sxs-lookup"><span data-stu-id="469c4-124">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="469c4-125">Voor dergelijke vraag in onbalans maakt het systeem een extra voorziening.</span><span class="sxs-lookup"><span data-stu-id="469c4-125">For such unbalanced demand, the planning system creates an extra supply.</span></span>  

### <a name="should-not-be-used-with-forecast"></a><span data-ttu-id="469c4-126">Moet niet worden gebruikt met prognose</span><span class="sxs-lookup"><span data-stu-id="469c4-126">Should Not be Used with Forecast</span></span>  
 <span data-ttu-id="469c4-127">Omdat de verwachte vraag al is uitgedrukt in het bestelpuntniveau, is het niet nodig een prognose in de planning van een artikel op te nemen met behulp van een bestelpunt.</span><span class="sxs-lookup"><span data-stu-id="469c4-127">Because the anticipated demand is already expressed in the reorder point level it is not necessary to include a forecast in the planning of an item using a reorder point.</span></span> <span data-ttu-id="469c4-128">Als het belangrijk is dat de planning op een prognose wordt gebaseerd, gebruikt u het lot-voor-lot beleid.</span><span class="sxs-lookup"><span data-stu-id="469c4-128">If it is relevant to base the plan on a forecast, use the lot-for-lot policy.</span></span>  

### <a name="must-not-be-used-with-reservations"></a><span data-ttu-id="469c4-129">Mag niet met reserveringen worden gebruikt</span><span class="sxs-lookup"><span data-stu-id="469c4-129">Must Not be Used with Reservations</span></span>  
 <span data-ttu-id="469c4-130">Als de gebruiker een aantal heeft gereserveerd, bijvoorbeeld een aantal in voorraad, voor een of andere toekomstige vraag, wordt de basis van de planning verstoord.</span><span class="sxs-lookup"><span data-stu-id="469c4-130">If the user has reserved a quantity, for instance a quantity in inventory, for some distant demand, the planning foundation will be disturbed.</span></span> <span data-ttu-id="469c4-131">Zelfs als de geplande voorraad met betrekking tot het bestelpunt aanvaardbaar is, zijn de hoeveelheden mogelijk niet beschikbaar.</span><span class="sxs-lookup"><span data-stu-id="469c4-131">Even if the projected inventory level is acceptable in relation to the reorder point, the quantities might not be available.</span></span> <span data-ttu-id="469c4-132">Het systeem probeert dit mogelijk te compenseren door uitzonderingsorders aan te maken. Het wordt echter aangeraden het veld Reserveren in te stellen op Nooit voor artikelen die worden gepland met behulp van een bestelpunt.</span><span class="sxs-lookup"><span data-stu-id="469c4-132">The system may try to compensate for that by creating exception orders; however, it is recommended that the Reserve field is set to Never on items that are planned using a reorder point.</span></span>

## <a name="maximum-qty"></a><span data-ttu-id="469c4-133">Maximum aantal</span><span class="sxs-lookup"><span data-stu-id="469c4-133">Maximum Qty.</span></span>
<span data-ttu-id="469c4-134">Het beleid Maximum aantal is een manier om voorraad bij te houden met behulp van een bestelpunt.</span><span class="sxs-lookup"><span data-stu-id="469c4-134">The Maximum Quantity policy is a way to maintain inventory using a reorder point.</span></span>  

<span data-ttu-id="469c4-135">Alles over het beleid voor een vast bestelaantal geldt ook voor dit beleid.</span><span class="sxs-lookup"><span data-stu-id="469c4-135">Everything regarding the Fixed Reorder Qty. policy also applies to this policy.</span></span> <span data-ttu-id="469c4-136">Het enige verschil is de hoeveelheid van de voorgestelde voorziening.</span><span class="sxs-lookup"><span data-stu-id="469c4-136">The only difference is the quantity of the suggested supply.</span></span> <span data-ttu-id="469c4-137">Wanneer het beleid voor maximaal aantal wordt gebruikt, wordt het bestelaantal dynamisch bepaald op basis van het geplande voorraadniveau en verschilt daarom gewoonlijk per order.</span><span class="sxs-lookup"><span data-stu-id="469c4-137">When using the maximum quantity policy, the reorder quantity will be defined dynamically based on the projected inventory level and will therefore usually differ from order to order.</span></span>  

### <a name="calculated-per-time-bucket"></a><span data-ttu-id="469c4-138">Berekend per tijdsinterval</span><span class="sxs-lookup"><span data-stu-id="469c4-138">Calculated per Time Bucket</span></span>  
<span data-ttu-id="469c4-139">Het bestelaantal wordt bepaald op het moment (het einde van het tijdsinterval) dat het planningssysteem detecteert dat het bestelpunt is overschreden.</span><span class="sxs-lookup"><span data-stu-id="469c4-139">The reorder quantity is determined at the point of time (the end of a time bucket) when the planning system detects that the reorder point has been crossed.</span></span> <span data-ttu-id="469c4-140">Op dit moment meet het systeem het verschil tussen het huidige geplande voorraadniveau en de opgegeven maximale voorraad.</span><span class="sxs-lookup"><span data-stu-id="469c4-140">At this time, the system measures the gap from the current projected inventory level up to the specified maximum inventory.</span></span> <span data-ttu-id="469c4-141">Dit vormt het aantal dat opnieuw moet worden besteld.</span><span class="sxs-lookup"><span data-stu-id="469c4-141">This constitutes the quantity that should be reordered.</span></span> <span data-ttu-id="469c4-142">Het systeem controleert vervolgens of de voorziening al elders is besteld voor ontvangst binnen de doorlooptijd. Als dit het geval is, wordt het aantal van de nieuwe voorzieningenorder verminderd met de reeds bestelde aantallen.</span><span class="sxs-lookup"><span data-stu-id="469c4-142">The system then checks if supply has already been ordered elsewhere to be received within the lead time and, if so, reduces the quantity of the new supply order by already ordered quantities.</span></span>  

<span data-ttu-id="469c4-143">Het systeem zorgt dat de geplande voorraad ten minste het bestelpuntniveau bereikt, voor het geval dat de gebruiker is vergeten een maximaal voorraadaantal op te geven.</span><span class="sxs-lookup"><span data-stu-id="469c4-143">The system will ensure that the projected inventory at least reaches the reorder point level – in case the user has forgotten to specify a maximum inventory quantity.</span></span>  

### <a name="combines-with-order-modifiers"></a><span data-ttu-id="469c4-144">Combineert met orderaanpassingsfuncties</span><span class="sxs-lookup"><span data-stu-id="469c4-144">Combines with Order Modifiers</span></span>  
<span data-ttu-id="469c4-145">Afhankelijk van de instellingen kan het het beste zijn om het maximale aantal-beleid te combineren met orderwijzigingen om een minimaal orderaantal te garanderen of af te ronden op een geheel aantal inkoopeenheden, of te splitsen in meerdere lots zoals bepaald door het maximale orderaantal.</span><span class="sxs-lookup"><span data-stu-id="469c4-145">Depending on the setup, it may be best to combine the Maximum Quantity policy with order modifiers to ensure a minimum order quantity or round it to an integer number of purchase units of measure, or split it into more lots as defined by the maximum order quantity.</span></span>  

### <a name="combines-with-calendars"></a><span data-ttu-id="469c4-146">Combineert met agenda's</span><span class="sxs-lookup"><span data-stu-id="469c4-146">Combines with Calendars</span></span>  
<span data-ttu-id="469c4-147">Voordat het planningssysteem een nieuwe voorzieningenorder voorstelt, wordt gecontroleerd of de order is gepland voor een niet-werkdag, volgens agenda's die zijn gedefinieerd in het veld **Basisagendacode** op de pagina's **Bedrijfsgegevens** en **Vestiging**.</span><span class="sxs-lookup"><span data-stu-id="469c4-147">Before suggesting a new supply order to meet a reorder point, the planning system checks if the order is scheduled for a non-working day, according to any calendars that are  defined in the **Base Calendar Code** field in the **Company Information** and **Location Card** pages.</span></span>  

<span data-ttu-id="469c4-148">Als de verwachte datum een vrije dag is, verplaatst het planningssysteem de order voorwaarts naar de dichtstbijzijnde werkdatum.</span><span class="sxs-lookup"><span data-stu-id="469c4-148">If the scheduled date is a non-working day, the planning system moves the order forward to the nearest working date.</span></span> <span data-ttu-id="469c4-149">Dit kan resulteren in een order die voldoet een bestelpunt maar aan een bepaalde vraag niet voldoet.</span><span class="sxs-lookup"><span data-stu-id="469c4-149">This may result in an order that meets a reorder point but does not meet some specific demand.</span></span> <span data-ttu-id="469c4-150">Voor dergelijke vraag in onbalans maakt het systeem een extra voorziening.</span><span class="sxs-lookup"><span data-stu-id="469c4-150">For such unbalanced demand, the planning system creates an extra supply.</span></span>

## <a name="order"></a><span data-ttu-id="469c4-151">Volgorde</span><span class="sxs-lookup"><span data-stu-id="469c4-151">Order</span></span>
<span data-ttu-id="469c4-152">In een op-order-produceren omgeving wordt een artikel ingekocht of geproduceerd om uitsluitend aan een specifieke vraag te voldoen.</span><span class="sxs-lookup"><span data-stu-id="469c4-152">In a make-to-order environment, an item is purchased or produced to exclusively cover a specific demand.</span></span> <span data-ttu-id="469c4-153">Meestal heeft dit betrekking op A-producten en de motivatie om het bestelbeleid Order te kiezen, kan zijn dat de vraag niet frequent is, dat de doorlooptijd onbeduidend is of dat de vereiste kenmerken verschillen.</span><span class="sxs-lookup"><span data-stu-id="469c4-153">Typically it relates to A-items, and the motivation for choosing the order reordering policy can be that the demand is infrequent, the lead-time is insignificant, or the required attributes vary.</span></span>  

<span data-ttu-id="469c4-154">Het programma maakt een order-naar-order-koppeling die fungeert als voorlopige verbinding tussen de voorziening, een voorzieningenorder of voorraad, en de vraag waaraan het zal voldoen.</span><span class="sxs-lookup"><span data-stu-id="469c4-154">The program creates an order-to-order link, which acts as a preliminary connection between the supply, a supply order or inventory, and the demand that it is going to fulfill.</span></span>  

<span data-ttu-id="469c4-155">Afgezien van het gebruik van het bestelbeleid kan de order-aan-order koppeling tijdens planning op de volgende manieren worden toegepast:</span><span class="sxs-lookup"><span data-stu-id="469c4-155">Apart from using the Order policy, the order-to-order link can be applied during planning in the following ways:</span></span>  

* <span data-ttu-id="469c4-156">Wanneer het productiebeleid Op order produceren wordt gebruikt om productieorders met meerdere niveaus of projecttype te maken (waarbij benodigde onderdelen op dezelfde productieorder worden geproduceerd).</span><span class="sxs-lookup"><span data-stu-id="469c4-156">When using the Make-to-Order manufacturing policy to create multi-level or project type production orders (producing needed components on the same production order).</span></span>  
* <span data-ttu-id="469c4-157">Wanneer de functie Verkooporderplanning wordt gebruikt om een productieorder te maken van een verkooporder.</span><span class="sxs-lookup"><span data-stu-id="469c4-157">When using the Sales Order Planning feature to create a production order from a sales order.</span></span>  

<span data-ttu-id="469c4-158">Zelfs als een productiebedrijf zichzelf beschouwt als een op-order-produceren omgeving, kan het het best zijn een lot-voor-lot bestelbeleid te gebruiken als de artikelen standaard zijn, zonder variatie in kenmerken.</span><span class="sxs-lookup"><span data-stu-id="469c4-158">Even if a manufacturing company considers itself as a make-to-order environment, it might be best to use a Lot-for-Lot reordering policy if the items are pure standard without variation in attributes.</span></span> <span data-ttu-id="469c4-159">Hierdoor gebruikt het systeem niet-geplande voorraad en worden verkooporders alleen gecumuleerd met dezelfde verzenddatum of binnen een bepaalde periode.</span><span class="sxs-lookup"><span data-stu-id="469c4-159">As a result, the system will use unplanned inventory and only accumulates sales orders with the same shipment date or within a defined time bucket.</span></span>  

### <a name="order-to-order-links-and-past-due-dates"></a><span data-ttu-id="469c4-160">Order-naar-order koppelingen en overschreden vervaldatums</span><span class="sxs-lookup"><span data-stu-id="469c4-160">Order-to-Order Links and Past Due Dates</span></span>  
<span data-ttu-id="469c4-161">In tegenstelling tot de meeste combinaties van voorziening en vraag, worden gekoppelde orders met vervaldatums voor de begindatum van de planning, volledig door het systeem gepland.</span><span class="sxs-lookup"><span data-stu-id="469c4-161">Unlike most supply-demand sets, linked orders with due dates before the planning starting date are fully planned for by the system.</span></span> <span data-ttu-id="469c4-162">De bedrijfsreden voor deze uitzondering is dat specifieke vraag-voorzieningcombinaties moeten worden gesynchroniseerd tot aan uitvoering.</span><span class="sxs-lookup"><span data-stu-id="469c4-162">The business reason for this exception is that specific demand-supply sets must be synchronized through to execution.</span></span> <span data-ttu-id="469c4-163">Zie voor meer informatie over de bevroren zone die de meeste vraag/voorziening toepast [Ontwerpdetails: Werken met orders voor de geplande begindatum](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span><span class="sxs-lookup"><span data-stu-id="469c4-163">For more information about the frozen zone that applies to most demand-supply types, see [Design Details: Dealing with Orders Before the Planning Starting Date](design-details-dealing-with-orders-before-the-planning-starting-date.md).</span></span>

## <a name="lot-for-lot"></a><span data-ttu-id="469c4-164">Lot-for-Lot</span><span class="sxs-lookup"><span data-stu-id="469c4-164">Lot-for-Lot</span></span>
<span data-ttu-id="469c4-165">Het lot-for-lot-beleid is het meest flexibel omdat het systeem alleen reageert op werkelijke vraag, én rekening houdt met verwachte vraag uit prognoses en raamcontracten en vervolgens het orderaantal op basis van de vraag vereffent.</span><span class="sxs-lookup"><span data-stu-id="469c4-165">The lot-for-lot policy is the most flexible because the system only reacts on actual demand, plus it acts on anticipated demand from forecast and blanket orders and then settles the order quantity based on the demand.</span></span> <span data-ttu-id="469c4-166">Het lot-for-lot-beleid is bedoeld voor A- en B-artikelen waar voorraad kan worden geaccepteerd maar vermeden moet worden.</span><span class="sxs-lookup"><span data-stu-id="469c4-166">The lot-for-lot policy is aimed at A- and B-items where inventory can be accepted but should be avoided.</span></span>  

<span data-ttu-id="469c4-167">In sommige opzichten lijkt het lot-voor-lot beleid op het orderbeleid, maar het hanteert een algemene aanpak van artikelen; het kan aantallen in voorraad accepteren en het bundelt vraag en corresponderend aanbod in tijdsintervallen die door de gebruiker worden gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="469c4-167">In some ways, the lot-for-lot policy looks like the Order policy, but it has a generic approach to items; it can accept quantities in inventory, and it bundles demand and corresponding supply in time buckets defined by the user.</span></span>  

<span data-ttu-id="469c4-168">Het tijdsinterval wordt gedefinieerd in het veld **Tijdsinterval**.</span><span class="sxs-lookup"><span data-stu-id="469c4-168">The time bucket is defined in the **Time Bucket** field.</span></span> <span data-ttu-id="469c4-169">Er wordt gewerkt met een minimumtijdsinterval van één dag, aangezien dit de kleinste tijdseenheid voor vraag- en voorzieningsgebeurtenissen in het systeem is (hoewel in de praktijk de tijdseenheid voor productieorders en materiaalbehoeften zelfs seconden kan zijn).</span><span class="sxs-lookup"><span data-stu-id="469c4-169">The system works with a minimum time bucket of one day, since this is the smallest time unit of measure on demand and supply events in the system (although, in practice, the time unit of measure on production orders and component needs can be seconds).</span></span>  

<span data-ttu-id="469c4-170">Met het tijdsinterval worden ook limieten ingesteld wanneer een bestaande voorzieningenorder opnieuw moet worden gepland om te voldoen aan een bepaalde vraag.</span><span class="sxs-lookup"><span data-stu-id="469c4-170">The time bucket also sets limits on when an existing supply order should be rescheduled to meet a given demand.</span></span> <span data-ttu-id="469c4-171">Als het aanbod binnen het tijdsinterval ligt, wordt het opnieuw in of uit gepland om aan de vraag te voldoen.</span><span class="sxs-lookup"><span data-stu-id="469c4-171">If the supply lies within the time bucket, it will be rescheduled in or out to meet the demand.</span></span> <span data-ttu-id="469c4-172">Als de voorziening eerder ligt, ontstaat onnodige opeenhoping van voorraad en moet worden geannuleerd.</span><span class="sxs-lookup"><span data-stu-id="469c4-172">Otherwise, if it lies earlier, it will cause unnecessary build-up of inventory and should be canceled.</span></span> <span data-ttu-id="469c4-173">Als het later ligt, wordt in plaats daarvan een nieuwe order gemaakt.</span><span class="sxs-lookup"><span data-stu-id="469c4-173">If it lies later, a new supply order will be created instead.</span></span>  

<span data-ttu-id="469c4-174">Met dit beleid is het ook mogelijk om een veiligheidsvoorraad te definiëren om mogelijke schommelingen in voorzieningen op te vangen of te voldoen aan plotselinge vraag.</span><span class="sxs-lookup"><span data-stu-id="469c4-174">With this policy, it is also possible to define a safety stock in order to compensate for possible fluctuations in supply, or to meet sudden demand.</span></span>  

<span data-ttu-id="469c4-175">Omdat het aantal van de voorzieningenorder op de werkelijke vraag is gebaseerd, kan het zinnig zijn de orderwijzigingen te gebruiken: rond het orderaantal naar boven af om aan een opgegeven orderveelvoud (of inkoopeenheid) te voldoen, vergroot de order tot een opgegeven minimaal orderaantal of verlaag het aantal tot het opgegeven maximale aantal (en maak zo twee of meer voorzieningen om het totaal benodigde aantal te bereiken).</span><span class="sxs-lookup"><span data-stu-id="469c4-175">Because the supply order quantity is based on the actual demand it can make sense to use the order modifiers: round the order quantity up to meet a specified order multiple (or purchase unit of measure), increase the order to a specified minimum order quantity, or decrease the quantity to the specified maximum quantity (and thus create two or more supplies to reach the total needed quantity).</span></span>

## <a name="see-also"></a><span data-ttu-id="469c4-176">Zie ook</span><span class="sxs-lookup"><span data-stu-id="469c4-176">See Also</span></span>  
<span data-ttu-id="469c4-177">[Ontwerpdetails: Planningsparameters](design-details-planning-parameters.md) </span><span class="sxs-lookup"><span data-stu-id="469c4-177">[Design Details: Planning Parameters](design-details-planning-parameters.md) </span></span>  
<span data-ttu-id="469c4-178">[Ontwerpdetails: Bestelbeleid verwerken](design-details-handling-reordering-policies.md) </span><span class="sxs-lookup"><span data-stu-id="469c4-178">[Design Details: Handling Reordering Policies](design-details-handling-reordering-policies.md) </span></span>  
[<span data-ttu-id="469c4-179">Ontwerpdetails: Voorraadplanning</span><span class="sxs-lookup"><span data-stu-id="469c4-179">Design Details: Supply Planning</span></span>](design-details-supply-planning.md)