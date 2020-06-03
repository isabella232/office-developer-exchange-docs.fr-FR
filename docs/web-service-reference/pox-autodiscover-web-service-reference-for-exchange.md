---
title: Référence du service Web de découverte automatique POX pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465652"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="83027-103">Référence du service Web de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="83027-104">Recherchez des informations de référence pour le service de découverte automatique POX dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="83027-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="83027-105">Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="83027-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="83027-106">Vous pouvez utiliser le service de découverte automatique « simple Old XML » (POX) pour envoyer des messages constitués uniquement de charges utiles XML, sans enveloppe SOAP englobante, afin de localiser les paramètres qu’une application cliente doit disposer afin de se connecter à Exchange.</span><span class="sxs-lookup"><span data-stu-id="83027-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="83027-107">Pour les clients qui ciblent des versions d’Exchange à partir d’Exchange Server 2010, nous vous recommandons d’utiliser le service de découverte automatique SOAP au lieu du service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="83027-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="83027-108">Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="83027-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="83027-109">Nous recommandons aux clients qui utilisent .NET Framework d’utiliser l’API managée EWS car elle contient un client de découverte automatique robuste et bien testé.</span><span class="sxs-lookup"><span data-stu-id="83027-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="83027-110">Pour plus d’informations sur l’API managée EWS, consultez la rubrique [prise en main des applications clientes d’API managée EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="83027-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="83027-111">Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur pendant les redirections de demande de découverte automatique de la VARIOle et les paramètres utilisateur qui sont renvoyés dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="83027-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="83027-112">La référence d’élément XML contient des résumés de ce que les éléments représentent et une description des hiérarchies d’éléments potentielles qui utilisent l’élément.</span><span class="sxs-lookup"><span data-stu-id="83027-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="83027-113">Cette documentation couvre les instances XML qui sont envoyées entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="83027-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="83027-114">Le service de découverte automatique POX ne dispose pas d’un schéma explicite.</span><span class="sxs-lookup"><span data-stu-id="83027-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="83027-115">Les Articles de cette section fournissent des exemples et des descriptions des messages qui sont utilisés pour récupérer des informations de configuration de découverte automatique à l’aide du service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="83027-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="83027-116">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="83027-116">In this section</span></span>
<span data-ttu-id="83027-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="83027-117"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="83027-118">Demande de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="83027-119">Réponse de découverte automatique POX pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="83027-120">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="83027-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="83027-121">See also</span></span>

- [<span data-ttu-id="83027-122">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="83027-123">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="83027-124">Référence de service Web de découverte automatique SOAP pour Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="83027-125">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="83027-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

