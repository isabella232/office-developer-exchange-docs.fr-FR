---
title: Éléments XML EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Rechercher des informations de référence pour les données XML EWS éléments dans Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756238"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="b54ab-103">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="b54ab-104">Rechercher des informations de référence pour les données XML EWS éléments dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="b54ab-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="b54ab-105">Exchange Web Services (EWS) est un service web basé sur SOAP, ce qui signifie que les messages de demande et de réponse qui sont envoyés entre le client et le serveur sont composent des éléments XML.</span><span class="sxs-lookup"><span data-stu-id="b54ab-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="b54ab-106">La documentation de cette section est basée sur les instances XML qui sont envoyés entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="b54ab-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="b54ab-107">Les instances XML sont définies dans les fichiers WSDL et le schéma qui sont trouvent dans le répertoire virtuel qui héberge EWS.</span><span class="sxs-lookup"><span data-stu-id="b54ab-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="b54ab-108">Si vous êtes un utilisateur authentifié, vous accédez aux fichiers WSDL et le schéma à l’aide de l’URL suivantes, où \<yourclientaccessserver\> est le nom de votre serveur d’accès au Client :</span><span class="sxs-lookup"><span data-stu-id="b54ab-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="b54ab-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — l’emplacement du fichier WSDL.</span><span class="sxs-lookup"><span data-stu-id="b54ab-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="b54ab-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — l’emplacement du schéma des messages.</span><span class="sxs-lookup"><span data-stu-id="b54ab-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="b54ab-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — l’emplacement du schéma de types.</span><span class="sxs-lookup"><span data-stu-id="b54ab-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="b54ab-112">Les fichiers de schéma qui décrivent les éléments XML EWS fournissent une feuille de route générale de la structure XML est possible, pour les interactions de message de réponse à la demande.</span><span class="sxs-lookup"><span data-stu-id="b54ab-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="b54ab-113">La structure XML réelle qui est envoyée entre client et serveur varie en fonction de l’opération qui est appelée, les informations demandées et les paramètres côté serveur.</span><span class="sxs-lookup"><span data-stu-id="b54ab-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="b54ab-114">Le fichier WSDL EWS, services.wsdl, n’est pas entièrement conforme à la norme WSDL, car il n’inclut pas une définition de service WSDL.</span><span class="sxs-lookup"><span data-stu-id="b54ab-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="b54ab-115">C’est pourquoi EWS n’est pas conçu pour être hébergé sur un ordinateur disposant d’une adresse prédéfinie.</span><span class="sxs-lookup"><span data-stu-id="b54ab-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="b54ab-116">Vous pouvez utiliser le service de découverte automatique pour obtenir l’adresse de point de terminaison EWS.</span><span class="sxs-lookup"><span data-stu-id="b54ab-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="b54ab-117">Certains générateurs de modèle objet côté client analyser le fichier WSDL et peuvent rencontrer une condition d’erreur car le fichier WSDL ne contient pas d’une définition de service WSDL.</span><span class="sxs-lookup"><span data-stu-id="b54ab-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="b54ab-118">Si votre générateur de modèle d’objet rencontre une erreur, vous pouvez insérer un espace réservé définition WSDL du service.</span><span class="sxs-lookup"><span data-stu-id="b54ab-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="b54ab-119">Si vous utilisez le .NET Framework pour développer votre application, nous vous recommandons d’utiliser l' [API managée EWS](http://aka.ms/ews-managed-api-readme), plutôt que d’un générateur de modèle d’objet.</span><span class="sxs-lookup"><span data-stu-id="b54ab-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="b54ab-120">L’API managée EWS fournit un modèle d’objet à utiliser pour gérer la sérialisation et la désérialisation XML EWS.</span><span class="sxs-lookup"><span data-stu-id="b54ab-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="b54ab-121">Pour plus d’informations, voir [prendre en main des applications clientes API managées](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b54ab-121">For more information, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="b54ab-122">Le fichier de schéma messages.xsd contient les définitions d’élément pour les éléments de niveau supérieur dans le corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="b54ab-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="b54ab-123">À l’exception des codes de réponse d’erreur, la plupart des définitions de messages.xsd sont spécifique à une opération.</span><span class="sxs-lookup"><span data-stu-id="b54ab-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="b54ab-124">Le schéma types.xsd contient les définitions pour les en-têtes SOAP et toutes les définitions de courants qui sont partagées entre les opérations.</span><span class="sxs-lookup"><span data-stu-id="b54ab-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b54ab-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b54ab-125">See also</span></span>

- [<span data-ttu-id="b54ab-126">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="b54ab-127">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="b54ab-128">Explorer l'API managée EWS, EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="b54ab-129">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="b54ab-130">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="b54ab-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

