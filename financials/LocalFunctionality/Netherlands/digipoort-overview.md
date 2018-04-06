---
title: Overzicht van Digipoort
description: In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen. Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden.
services: project-madeira
documentationcenter: 
author: SorenGP
ms.service: dynamics365-financials
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: 
ms.date: 017/10/2018
ms.author: sgroespe
ms.translationtype: HT
ms.sourcegitcommit: b34f276a764f0e828fbc1f015429df9852242a4c
ms.openlocfilehash: aecef53418e4730b763da18093a8326851e822c9
ms.contentlocale: nl-nl
ms.lasthandoff: 03/22/2018

---
# <a name="digipoort-overview"></a><span data-ttu-id="655bf-104">Overzicht van Digipoort</span><span class="sxs-lookup"><span data-stu-id="655bf-104">Digipoort Overview</span></span>
<span data-ttu-id="655bf-105">In Nederland gebruikt u Digipoort om periodieke elektronische aangiften te maken voor btw-aangiften en ICP-rapporten in EU-verkooplijstverzendingen.</span><span class="sxs-lookup"><span data-stu-id="655bf-105">In the Netherlands, you use Digipoort to make periodic electronic filings for VAT declarations and ICP reports in EU sales list submissions.</span></span> <span data-ttu-id="655bf-106">Digipoort is het elektronische postkantoor dat door de Nederlandse overheid voor bedrijven wordt geboden.</span><span class="sxs-lookup"><span data-stu-id="655bf-106">Digipoort is the electronic post office provided by the Dutch government for companies.</span></span> <span data-ttu-id="655bf-107">Het bevat de gemeenschappelijke infrastructuur voor de communicatie van gegevens tussen bedrijven en de overheid, inclusief btw-aangiftes.</span><span class="sxs-lookup"><span data-stu-id="655bf-107">It provides the common infrastructure for the communication of information between companies and the government, including VAT declarations.</span></span> <span data-ttu-id="655bf-108">De rapporten hebben de XBRL-indeling.</span><span class="sxs-lookup"><span data-stu-id="655bf-108">The reports are in XBRL format.</span></span>  

<span data-ttu-id="655bf-109">Het installatieprogramma van [!INCLUDE[d365fin](../../includes/d365fin_md.md)] installeert de .dll op de volgende locatie: c:Program Files (x86)Microsoft Dynamics NAV<version>RoleTailored ClientAdd-insMicrosoft.Dynamics.NL.Digipoortservice.dll.</span><span class="sxs-lookup"><span data-stu-id="655bf-109">[!INCLUDE[d365fin](../../includes/d365fin_md.md)] installer installs the .dll to the following location: c:Program Files (x86)Microsoft Dynamics NAV<version>RoleTailored ClientAdd-insMicrosoft.Dynamics.NL.Digipoortservice.dll.</span></span>  

<span data-ttu-id="655bf-110">Het Digipoort-kanaal vervangt de BAPI-methode voor het doen van verzendingen.</span><span class="sxs-lookup"><span data-stu-id="655bf-110">The Digipoort channel replaces the BAPI method for making submissions.</span></span>  

## <a name="certificate-storage"></a><span data-ttu-id="655bf-111">Certificaatopslag</span><span class="sxs-lookup"><span data-stu-id="655bf-111">Certificate Storage</span></span>  
<span data-ttu-id="655bf-112">Als u via Digipoort elektronisch wilt communiceren met de Nederlandse overheid, hebt u twee certificaten nodig (PKIoverheid).</span><span class="sxs-lookup"><span data-stu-id="655bf-112">In order to communicate electronically using Digipoort with the Dutch government, you will need two certificates (PKIoverheid).</span></span> <span data-ttu-id="655bf-113">U hebt een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse belastingdienst.</span><span class="sxs-lookup"><span data-stu-id="655bf-113">You will need a private certificate for the company as well as a public certificate from the website of the Dutch tax authorities.</span></span> <span data-ttu-id="655bf-114">een privécertificaat voor het bedrijf nodig en een openbaar certificaat van de website van de Nederlandse autoriteiten.</span><span class="sxs-lookup"><span data-stu-id="655bf-114">need a private certificate for the company as well as a public certificate from the Dutch authorities.</span></span> <span data-ttu-id="655bf-115">U kunt meer specifieke informatie van de website van de Nederlandse belastingdienst krijgen.</span><span class="sxs-lookup"><span data-stu-id="655bf-115">You can get more specific information from the website of the Dutch tax authority.</span></span> <span data-ttu-id="655bf-116">Zie voor meer informatie de website van de Nederlandse belastingdienst [Logius](https://aansluiten.procesinfrastructuur.nl/site/en/).</span><span class="sxs-lookup"><span data-stu-id="655bf-116">For more information, see the Dutch Tax Administration website [Logius](https://aansluiten.procesinfrastructuur.nl/site/en/).</span></span>  

<span data-ttu-id="655bf-117">U moet de certificaten importeren die u in het certificaatarchief van Windows hebt ontvangen.</span><span class="sxs-lookup"><span data-stu-id="655bf-117">You will have to import the certificates that you receive into the Windows Certificate store.</span></span> <span data-ttu-id="655bf-118">Dit is een wijziging van eerdere versies, waarin u certificaten in [!INCLUDE[d365fin](../../includes/d365fin_md.md)] ontving.</span><span class="sxs-lookup"><span data-stu-id="655bf-118">This is a change from prior releases, in which you stored your certificates in [!INCLUDE[d365fin](../../includes/d365fin_md.md)].</span></span>  

## <a name="see-also"></a><span data-ttu-id="655bf-119">Zie ook</span><span class="sxs-lookup"><span data-stu-id="655bf-119">See Also</span></span>  
[<span data-ttu-id="655bf-120">Certificaten instellen voor gebruik met Digipoort</span><span class="sxs-lookup"><span data-stu-id="655bf-120">Set Up Certificates for use with Digipoort</span></span>](how-to-set-up-certificates-for-use-with-digipoort.md)

