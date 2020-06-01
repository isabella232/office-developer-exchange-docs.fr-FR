---
title: Référence de service Web de découverte automatique SOAP pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Recherchez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468424"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="ce569-103">Référence de service Web de découverte automatique SOAP pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ce569-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="ce569-104">Recherchez des informations de référence pour le service de découverte automatique SOAP dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce569-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="ce569-105">Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce569-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="ce569-106">Vous pouvez utiliser le service de découverte automatique SOAP pour envoyer des messages entre l’application cliente et le serveur Exchange afin de localiser les paramètres que l’application utilisera pour se connecter à Exchange.</span><span class="sxs-lookup"><span data-stu-id="ce569-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="ce569-107">Contrairement au service de découverte automatique POX, le service de découverte automatique SOAP autorise des demandes de découverte automatique par lot pour de nombreux paramètres d’utilisateurs et un contrôle plus précis sur les paramètres qui sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="ce569-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ce569-108">Pour les clients qui ciblent des versions d’Exchange à partir d’Exchange Server 2010, nous vous recommandons d’utiliser le service de découverte automatique SOAP (au lieu du service de découverte automatique POX).</span><span class="sxs-lookup"><span data-stu-id="ce569-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="ce569-109">Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique POX.</span><span class="sxs-lookup"><span data-stu-id="ce569-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="ce569-110">Nous recommandons aux clients qui utilisent .NET Framework d’utiliser l’API managée EWS car elle contient un client de découverte automatique SOAP fiable et bien testé.</span><span class="sxs-lookup"><span data-stu-id="ce569-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="ce569-111">Pour plus d’informations sur l’API managée EWS, consultez la rubrique [prise en main des applications clientes d’API managée EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="ce569-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="ce569-112">Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur pendant les redirections de demande de découverte automatique SOAP et les paramètres utilisateur qui sont renvoyés dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="ce569-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="ce569-113">La référence d’élément XML contient des résumés de ce que les éléments représentent et une description des hiérarchies d’éléments potentielles qui contiennent l’élément.</span><span class="sxs-lookup"><span data-stu-id="ce569-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="ce569-114">Les Articles de cette section décrivent les instances XML qui sont envoyées entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="ce569-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="ce569-115">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel du serveur qui héberge le service de découverte automatique SOAP.</span><span class="sxs-lookup"><span data-stu-id="ce569-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="ce569-116">Les rubriques relatives à l’opération WSDL de cette section fournissent une vue d’ensemble des opérations effectuées par l’opération et des exemples de demande et de réponse.</span><span class="sxs-lookup"><span data-stu-id="ce569-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="ce569-117">Vous pouvez utiliser les informations de version fournies pour déterminer si les fonctionnalités que vous souhaitez utiliser sont disponibles dans la version du produit que vous exécutez.</span><span class="sxs-lookup"><span data-stu-id="ce569-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="ce569-118">Les exemples fournis dans les rubriques relatives à l’opération vous aident également à comprendre la structure du code XML inclus dans les messages SOAP échangés avec le serveur.</span><span class="sxs-lookup"><span data-stu-id="ce569-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="ce569-119">Cette section fournit également des exemples et des descriptions des messages qui sont utilisés pour récupérer des informations de configuration de découverte automatique à l’aide du service de découverte automatique SOAP.</span><span class="sxs-lookup"><span data-stu-id="ce569-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="ce569-120">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="ce569-120">In this section</span></span>
<span data-ttu-id="ce569-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="ce569-121"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="ce569-122">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce569-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="ce569-123">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce569-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="ce569-124">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce569-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="ce569-125">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ce569-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="ce569-126">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="ce569-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="ce569-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ce569-127">See also</span></span>


- [<span data-ttu-id="ce569-128">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ce569-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="ce569-129">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ce569-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="ce569-130">Utiliser la découverte automatique pour trouver des points de connexion</span><span class="sxs-lookup"><span data-stu-id="ce569-130">Use Autodiscover to find connection points</span></span>](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="ce569-131">Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ce569-131">Get user settings from Exchange by using Autodiscover</span></span>](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="ce569-132">Obtenir des paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="ce569-132">Get domain settings from an Exchange server</span></span>](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="ce569-133">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ce569-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

