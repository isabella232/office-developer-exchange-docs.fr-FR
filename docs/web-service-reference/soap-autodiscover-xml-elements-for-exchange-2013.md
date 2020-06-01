---
title: Éléments XML de découverte automatique SOAP pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Recherchez des informations de référence sur les éléments XML pour le service Web de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465183"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="0fe35-103">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0fe35-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="0fe35-104">Recherchez des informations de référence sur les éléments XML pour le service Web de découverte automatique SOAP dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fe35-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="0fe35-105">La documentation de cette section est basée sur les instances d’éléments XML de découverte automatique SOAP qui sont envoyées entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="0fe35-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="0fe35-106">La documentation de cette instance XML est basée sur les fichiers WSDL et de schéma qui se trouvent dans le répertoire virtuel qui héberge le service de découverte automatique SOAP.</span><span class="sxs-lookup"><span data-stu-id="0fe35-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="0fe35-107">Les utilisateurs authentifiés peuvent accéder aux fichiers WSDL et de schéma à l’aide d’une URL semblable à l’une des suivantes :</span><span class="sxs-lookup"><span data-stu-id="0fe35-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="0fe35-108">Emplacement du fichier WSDL : `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="0fe35-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="0fe35-109">Emplacement du schéma des messages : `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` ou`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="0fe35-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="0fe35-110">L’emplacement des fichiers de schéma et WSDL de découverte automatique SOAP varie en fonction de l’installation d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="0fe35-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="0fe35-111">Le fichier de schéma messages. xsd décrit les éléments XML qui peuvent être envoyés dans un en-tête SOAP de découverte automatique et un corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="0fe35-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="0fe35-112">Ce fichier fournit une feuille de route générale sur ce que peut être la structure XML pour une interaction de message demande-réponse donnée.</span><span class="sxs-lookup"><span data-stu-id="0fe35-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="0fe35-113">La structure XML réelle qui est envoyée entre le client et le serveur est basée sur les options et le contexte dans lequel elle est utilisée.</span><span class="sxs-lookup"><span data-stu-id="0fe35-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="0fe35-114">Les fichiers de schéma définissent les données XML possibles.</span><span class="sxs-lookup"><span data-stu-id="0fe35-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="0fe35-115">La plage réelle de code XML envoyé sur le réseau est basée sur l’opération appelée, les informations demandées et les paramètres côté serveur.</span><span class="sxs-lookup"><span data-stu-id="0fe35-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="0fe35-116">Sections connexes</span><span class="sxs-lookup"><span data-stu-id="0fe35-116">Related sections</span></span>

- [<span data-ttu-id="0fe35-117">Référence de service Web de découverte automatique SOAP pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="0fe35-118">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="0fe35-119">Référence du service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="0fe35-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0fe35-120">See also</span></span>

- [<span data-ttu-id="0fe35-121">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="0fe35-122">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="0fe35-123">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0fe35-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

