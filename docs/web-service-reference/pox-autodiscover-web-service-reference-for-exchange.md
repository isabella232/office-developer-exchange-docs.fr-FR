---
title: Référence de service web variole découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Trouvez des informations de référence pour le service de découverte automatique variole dans Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="7ac7a-103">Référence de service web variole découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="7ac7a-104">Trouvez des informations de référence pour le service de découverte automatique variole dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="7ac7a-105">Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="7ac7a-106">Vous pouvez utiliser « XML brut anciens » service de découverte automatique (POX) pour envoyer des messages qui contiennent uniquement les charges XML, sans les enveloppes SOAP englobants, afin de localiser les paramètres dont une application cliente doit se connecter à Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7ac7a-107">Pour les clients qui ciblent les versions d’Exchange commençant par Exchange Server 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP au lieu du service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="7ac7a-108">Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="7ac7a-109">Il est recommandé que les clients qui utilisent le .NET Framework utilisent l’API managée EWS, car il contient un client de découverte automatique variole robuste et bien testé.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="7ac7a-110">Pour plus d’informations sur l’API managée EWS, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="7ac7a-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="7ac7a-111">Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur au cours des redirections de demande de découverte automatique POX et les paramètres utilisateur sont retournés dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="7ac7a-112">Référence à l’élément XML contient les résumés de ce qui représentent les éléments et une description des hiérarchies d’élément potentiels qui utilisent l’élément.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="7ac7a-113">Cette documentation traite les instances XML qui sont envoyés entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="7ac7a-114">Le service de découverte automatique variole ne dispose pas d’un schéma explicite.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="7ac7a-115">Les articles de cette section fournissent des exemples et une description des messages qui sont utilisées pour extraire des informations de configuration de découverte automatique en utilisant le service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="7ac7a-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="7ac7a-116">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="7ac7a-116">In this section</span></span>
<span data-ttu-id="7ac7a-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="7ac7a-117"></span></span>

- [<span data-ttu-id="7ac7a-118">Demande de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="7ac7a-119">Réponse de découverte automatique variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="7ac7a-120">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="7ac7a-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7ac7a-121">See also</span></span>

- [<span data-ttu-id="7ac7a-122">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="7ac7a-123">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="7ac7a-124">SOAP de référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="7ac7a-125">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7ac7a-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

