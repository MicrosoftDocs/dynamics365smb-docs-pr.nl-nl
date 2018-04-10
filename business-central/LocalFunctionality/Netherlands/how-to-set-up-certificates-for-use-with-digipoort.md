---
title: Certificaten instellen voor gebruik met Digipoort
description: Informatie over Digipoort-certificaten.
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
ms.sourcegitcommit: e7dcdc0935a8793ae226dfc2f9709b5b8f487a62
ms.openlocfilehash: 21f22fe25003b3255f429551e699143300535e37
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---

# <a name="set-up-certificates-for-use-with-digipoort"></a><span data-ttu-id="50381-103">Certificaten instellen voor gebruik met Digipoort</span><span class="sxs-lookup"><span data-stu-id="50381-103">Set Up Certificates for use with Digipoort</span></span>
<span data-ttu-id="50381-104">In de volgende procedure wordt ervan uitgegaan dat u de certificaten van de overheid hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="50381-104">The following procedure assumes that you have obtained the certificates from the government.</span></span> <span data-ttu-id="50381-105">Als dat niet zo is, voert u de volgende stappen uit om de certificaten te krijgen.</span><span class="sxs-lookup"><span data-stu-id="50381-105">If you have not, take the following steps to obtain the certificates.</span></span>  

- <span data-ttu-id="50381-106">Verkrijg een PKIoverheid-certificaat voor het bedrijf als u er nog geen hebt.</span><span class="sxs-lookup"><span data-stu-id="50381-106">Obtain a PKIoverheid certificate for the company if you do not have one already.</span></span> <span data-ttu-id="50381-107">Een lijst met certificaatproviders vindt u hier: [http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps](http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps).</span><span class="sxs-lookup"><span data-stu-id="50381-107">A list of certificate providers can be found here: [http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps](http://www.logius.nl/producten/toegang/pkioverheid/aansluiten/toegetreden-csps).</span></span>  

- <span data-ttu-id="50381-108">Verkrijg een **Digipoort Service-certificaat**, dat kan worden verkregen van de website van de Nederlandse belastingdienst: [https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl).</span><span class="sxs-lookup"><span data-stu-id="50381-108">Obtain a **Digipoort Service certificate**, which can be obtained at the Dutch Tax Administration website: [https://aansluiten.procesinfrastructuur.nl](https://aansluiten.procesinfrastructuur.nl).</span></span>  

- <span data-ttu-id="50381-109">Registreer een gebruiker van Digipoort, wat u hier kunt doen: [https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw](https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw).</span><span class="sxs-lookup"><span data-stu-id="50381-109">Register a user of Digipoort, which can be done here: [https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw](https://aansluiten.procesinfrastructuur.nl/site/registratie/nieuw).</span></span>  

<span data-ttu-id="50381-110">Nadat u zich registreert en aanmeldt bij de officiële site, kunt u de Digipoort-servercertificaten van deze website downloaden: [https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten](https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten).</span><span class="sxs-lookup"><span data-stu-id="50381-110">After you register and log on to the official site, you can download the digiport server certificates from this site: [https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten](https://aansluiten.procesinfrastructuur.nl/site/documentatie/certificaten).</span></span>  

<span data-ttu-id="50381-111">Vervolgens moet u de certificaten installeren.</span><span class="sxs-lookup"><span data-stu-id="50381-111">Next, you have to install the certificates.</span></span> <span data-ttu-id="50381-112">De certificaten moeten op de server worden geïnstalleerd.</span><span class="sxs-lookup"><span data-stu-id="50381-112">The certificates have to be installed on the server.</span></span> <span data-ttu-id="50381-113">Later gebruikt u de algemene naam (CN) van de certificaten in [!INCLUDE[d365fin](../../includes/d365fin_md.md)].</span><span class="sxs-lookup"><span data-stu-id="50381-113">Later, you will use the common name (CN) of the certificates in [!INCLUDE[d365fin](../../includes/d365fin_md.md)].</span></span>  

> [!NOTE]  
>  <span data-ttu-id="50381-114">In de Digipoort-implementatie installeert u certificaten op de server.</span><span class="sxs-lookup"><span data-stu-id="50381-114">In the Digipoort implementation you install certificates on the server.</span></span> <span data-ttu-id="50381-115">Gebruikers die moeten kunnen communiceren met de belastingdienst via Digipoort, hebben toegang nodig tot de persoonlijke sleutel van het persoonlijke certificaat op de server.</span><span class="sxs-lookup"><span data-stu-id="50381-115">Users who need to be able to communicate with tax authorities via Digipoort will need access to the private key of the personal certificate on the server.</span></span>  

## <a name="to-install-the-certificates"></a><span data-ttu-id="50381-116">De certificaten installeren</span><span class="sxs-lookup"><span data-stu-id="50381-116">To install the certificates</span></span>  

1.  <span data-ttu-id="50381-117">Open de **Windows-certificaatconsole** om de certificaten te importeren die u van de overheid hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="50381-117">Open the **Windows Certificate Console** to import the certificates that you have obtained from the government.</span></span> <span data-ttu-id="50381-118">Zie voor meer informatie [De certificaatconsole gebruiken](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx).</span><span class="sxs-lookup"><span data-stu-id="50381-118">For more information, see [Use the Certificates Console](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx).</span></span>  
2.  <span data-ttu-id="50381-119">Importeer de twee certificaten.</span><span class="sxs-lookup"><span data-stu-id="50381-119">Import the two certificates.</span></span> <span data-ttu-id="50381-120">Zie voor meer informatie [Een certificaat importeren](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx#To_import_certificates).</span><span class="sxs-lookup"><span data-stu-id="50381-120">For more information, [To import a certificate](http://social.technet.microsoft.com/wiki/contents/articles/2167.how-to-use-the-certificates-console.aspx#To_import_certificates).</span></span>  

    <span data-ttu-id="50381-121">**Persoonlijk certificaat**</span><span class="sxs-lookup"><span data-stu-id="50381-121">**Personal Certificate**</span></span>  

    1.  <span data-ttu-id="50381-122">Kies in de sectie **Persoonlijk** de actie **Importeren**.</span><span class="sxs-lookup"><span data-stu-id="50381-122">In the **Personal** section, choose the **Import** action.</span></span> <span data-ttu-id="50381-123">Zorg dat u de juiste machtigingen instelt voor de persoonlijke sleutel.</span><span class="sxs-lookup"><span data-stu-id="50381-123">Make sure to set proper permissions to the private key.</span></span>  
    2.  <span data-ttu-id="50381-124">Voer de **wizard Certificaat importeren** uit.</span><span class="sxs-lookup"><span data-stu-id="50381-124">Complete the **Certificate Import Wizard**.</span></span>  

    <span data-ttu-id="50381-125">**Servicecertificaat**</span><span class="sxs-lookup"><span data-stu-id="50381-125">**Service Certificate**</span></span>  

    1.  <span data-ttu-id="50381-126">Kies in de sectie **Vertrouwde uitgevers** de actie **Importeren**</span><span class="sxs-lookup"><span data-stu-id="50381-126">In the **Trusted Publishers** section, choose the **Import** action</span></span>  
    2.  <span data-ttu-id="50381-127">Voer de **wizard Certificaat importeren** uit.</span><span class="sxs-lookup"><span data-stu-id="50381-127">Complete the **Certificate Import Wizard**.</span></span>  

3.  <span data-ttu-id="50381-128">Verleen leesmachtigingen aan het certificaat voor de gebruiker die de verzending doet.</span><span class="sxs-lookup"><span data-stu-id="50381-128">Grant read permissions to the certificate for the user who is doing the submission.</span></span>  

    <span data-ttu-id="50381-129">Klik met de rechtermuisknop, kies de actie **Alle taken** en kies vervolgens de actie **Persoonlijke sleutels beheren**.</span><span class="sxs-lookup"><span data-stu-id="50381-129">Right-click the certificate, choose the **All Tasks** action, and then choose the **Manage Private Keys** action.</span></span> <span data-ttu-id="50381-130">Selecteer de gebruiker en schakel in het vak **Machtigingen** het selectievakje **Lezen toestaan** in.</span><span class="sxs-lookup"><span data-stu-id="50381-130">Select the user and in the **Permissions** box, select the **Allow Read** check box.</span></span>  

4.  <span data-ttu-id="50381-131">Sluit het venster **Console**.</span><span class="sxs-lookup"><span data-stu-id="50381-131">Close the **Console** window.</span></span>  

## <a name="see-also"></a><span data-ttu-id="50381-132">Zie ook</span><span class="sxs-lookup"><span data-stu-id="50381-132">See Also</span></span>  
 [<span data-ttu-id="50381-133">Overzicht van Digipoort</span><span class="sxs-lookup"><span data-stu-id="50381-133">Digipoort Overview</span></span>](digipoort-overview.md)

