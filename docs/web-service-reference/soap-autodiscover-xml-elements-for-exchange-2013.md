---
title: Éléments du fichier XML Autodiscover SOAP pour Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Trouvez des informations de référence d’élément XML pour le service web de découverte automatique SOAP dans Exchange.
ms.openlocfilehash: 7201ef33060691df70b63d06b2045e1120b0610f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829517"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="1b7bc-103">Éléments du fichier XML Autodiscover SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="1b7bc-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="1b7bc-104">Trouvez des informations de référence d’élément XML pour le service web de découverte automatique SOAP dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="1b7bc-105">La documentation de cette section est basée sur les instances d’élément XML de découverte automatique SOAP qui sont envoyés entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="1b7bc-106">Cette documentation d’instance XML est basée sur les fichiers qui sont trouvent dans le répertoire virtuel qui héberge le service de découverte automatique SOAP WSDL et le schéma.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="1b7bc-107">Les utilisateurs authentifiés peuvent parcourir les fichiers WSDL et le schéma à l’aide d’une URL qui est similaire à une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="1b7bc-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="1b7bc-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — l’emplacement du fichier WSDL.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-108">http://\<yourclientaccessserver\>.com/autodiscover/services.wsdl or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="1b7bc-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd ou http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — l’emplacement du schéma des messages.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-109">http://\<yourclientaccessserver\>.com/autodiscover/messages.xsd or http://autodiscover.\<yourclientaccessserver\>.com/autodiscover/messages.xsd — The location of the messages schema.</span></span>
    
<span data-ttu-id="1b7bc-110">L’emplacement des fichiers de schéma et SOAP Autodiscover WSDL varie en fonction de l’installation d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="1b7bc-111">Le fichier de schéma messages.xsd décrit les éléments XML qui peuvent être envoyés dans un en-tête SOAP de découverte automatique et le corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="1b7bc-112">Ce fichier fournit un guide général de la structure XML qui peut être pour une interaction de message de demande-réponse donnée.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="1b7bc-113">La structure XML réelle échangées entre le client et le serveur est basée sur les options et le contexte dans lequel il est utilisé.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="1b7bc-114">Les fichiers de schéma définissent ce que XML est possible.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="1b7bc-115">La plage de code XML qui est transmis sur le réseau est basé sur l’opération est appelé, les informations demandées et les paramètres côté serveur.</span><span class="sxs-lookup"><span data-stu-id="1b7bc-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="1b7bc-116">Sections associées</span><span class="sxs-lookup"><span data-stu-id="1b7bc-116">Related sections</span></span>
<span data-ttu-id="1b7bc-117"><a name="bk_RelatedSections"> </a></span><span class="sxs-lookup"><span data-stu-id="1b7bc-117"></span></span>

- [<span data-ttu-id="1b7bc-118">SOAP de référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-118">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="1b7bc-119">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-119">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
    
- [<span data-ttu-id="1b7bc-120">Référence au service web messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-120">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="1b7bc-121">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1b7bc-121">See also</span></span>

- [<span data-ttu-id="1b7bc-122">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="1b7bc-123">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="1b7bc-124">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1b7bc-124">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    
