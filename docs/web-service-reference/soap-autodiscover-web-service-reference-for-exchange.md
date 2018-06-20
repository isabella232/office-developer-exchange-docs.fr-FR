---
title: SOAP de référence de service web de découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Trouvez des informations de référence pour le service de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="b444f-103">SOAP de référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b444f-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="b444f-104">Trouvez des informations de référence pour le service de découverte automatique SOAP dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b444f-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="b444f-105">Le service de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="b444f-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="b444f-106">Vous pouvez utiliser le service de découverte automatique SOAP pour envoyer des messages entre l’application cliente et le serveur Exchange pour rechercher les paramètres de que l’application utilise pour se connecter à Exchange.</span><span class="sxs-lookup"><span data-stu-id="b444f-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="b444f-107">Contrairement au service de découverte automatique variole, le service de découverte automatique SOAP permet pour les demandes de découverte automatique par lots pour les paramètres de nombreux utilisateurs et un contrôle plus précis sur les paramètres sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="b444f-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b444f-108">Pour les clients qui ciblent les versions d’Exchange commençant par Exchange Server 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP (plutôt que le service de découverte automatique variole).</span><span class="sxs-lookup"><span data-stu-id="b444f-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="b444f-109">Les clients qui ciblent Exchange 2007 doivent utiliser le service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="b444f-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="b444f-110">Il est recommandé que les clients qui utilisent le .NET Framework utilisent l’API managée EWS, car il contient un client SOAP Autodiscover robuste et bien testé.</span><span class="sxs-lookup"><span data-stu-id="b444f-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="b444f-111">Pour plus d’informations sur l’API managée EWS, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b444f-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="b444f-112">Cette section fournit des informations sur les éléments XML qui sont envoyés entre le client et le serveur au cours des redirections de demande SOAP Autodiscover et les paramètres utilisateur sont retournés dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="b444f-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="b444f-113">Référence à l’élément XML contient les résumés de ce qui représentent les éléments et une description des hiérarchies potentiels d’élément qui contient l’élément.</span><span class="sxs-lookup"><span data-stu-id="b444f-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="b444f-114">Les articles de cette section décrivent les instances XML qui sont envoyés entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="b444f-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="b444f-115">Vous trouverez le schéma qui décrit les éléments suivants dans le répertoire virtuel du serveur qui héberge le service de découverte automatique SOAP.</span><span class="sxs-lookup"><span data-stu-id="b444f-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="b444f-116">L’opération WSDL rubriques de cette section fournissent qu'une vue d’ensemble de l’opération qui est et des exemples de requête et de réponse opération.</span><span class="sxs-lookup"><span data-stu-id="b444f-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="b444f-117">Vous pouvez utiliser les informations de version fournies pour déterminer si les fonctionnalités que vous souhaitez utiliser sont disponibles dans la version du produit que vous exécutez.</span><span class="sxs-lookup"><span data-stu-id="b444f-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="b444f-118">Les exemples dans les rubriques opération également vous aident à comprendre la structure du code XML qui est inclus dans les messages SOAP qui sont envoyés vers ou à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="b444f-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="b444f-119">Cette section fournit des exemples et une description des messages qui sont utilisées pour extraire des informations de configuration de découverte automatique en utilisant le service de découverte automatique SOAP.</span><span class="sxs-lookup"><span data-stu-id="b444f-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="b444f-120">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="b444f-120">In this section</span></span>
<span data-ttu-id="b444f-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="b444f-121"></span></span>

- [<span data-ttu-id="b444f-122">Opération GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b444f-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="b444f-123">Opération GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b444f-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="b444f-124">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b444f-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="b444f-125">Opération GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="b444f-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="b444f-126">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b444f-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="b444f-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b444f-127">See also</span></span>


- [<span data-ttu-id="b444f-128">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b444f-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="b444f-129">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b444f-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="b444f-130">Utiliser la découverte automatique pour rechercher les points de connexion</span><span class="sxs-lookup"><span data-stu-id="b444f-130">Use Autodiscover to find connection points</span></span>](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="b444f-131">Obtenir les paramètres de l’utilisateur Exchange à l’aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="b444f-131">Get user settings from Exchange by using Autodiscover</span></span>](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="b444f-132">Obtenir les paramètres de domaine à partir d’un serveur Exchange</span><span class="sxs-lookup"><span data-stu-id="b444f-132">Get domain settings from an Exchange server</span></span>](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="b444f-133">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b444f-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

