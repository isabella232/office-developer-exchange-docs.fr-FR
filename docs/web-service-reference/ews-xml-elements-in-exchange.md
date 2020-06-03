---
title: Éléments XML de EWS dans Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Recherchez des informations de référence pour les éléments XML EWS dans Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526115"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="15e1a-103">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="15e1a-104">Recherchez des informations de référence pour les éléments XML EWS dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="15e1a-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="15e1a-105">Les services Web Exchange (EWS) sont un service Web basé sur SOAP, ce qui signifie que les messages de demande et de réponse échangés entre le client et le serveur sont constitués d’éléments XML.</span><span class="sxs-lookup"><span data-stu-id="15e1a-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="15e1a-106">La documentation de cette section est basée sur les instances XML qui sont envoyées entre le client et le serveur.</span><span class="sxs-lookup"><span data-stu-id="15e1a-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="15e1a-107">Les instances XML sont définies dans les fichiers WSDL et de schéma qui se trouvent dans le répertoire virtuel qui héberge EWS.</span><span class="sxs-lookup"><span data-stu-id="15e1a-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="15e1a-108">Si vous êtes un utilisateur authentifié, vous pouvez accéder aux fichiers WSDL et de schéma à l’aide des URL suivantes, où \<yourclientaccessserver\> est le nom de votre serveur d’accès au client :</span><span class="sxs-lookup"><span data-stu-id="15e1a-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="15e1a-109">http:// \<yourclientaccessserver\> . com/EWS/services. wsdl : emplacement du fichier WSDL.</span><span class="sxs-lookup"><span data-stu-id="15e1a-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="15e1a-110">http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — l’emplacement du schéma des messages.</span><span class="sxs-lookup"><span data-stu-id="15e1a-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="15e1a-111">http:// \<yourclientaccessserver\> . com/EWS/types. xsd — l’emplacement du schéma de types.</span><span class="sxs-lookup"><span data-stu-id="15e1a-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="15e1a-112">Les fichiers de schéma qui décrivent les éléments XML EWS fournissent une feuille de route générale de la structure XML qui est possible pour les interactions entre les messages demande-réponse.</span><span class="sxs-lookup"><span data-stu-id="15e1a-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="15e1a-113">La structure XML réelle qui est envoyée entre le client et le serveur varie en fonction de l’opération qui est appelée, des informations demandées et des paramètres côté serveur.</span><span class="sxs-lookup"><span data-stu-id="15e1a-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="15e1a-114">Le fichier WSDL EWS, services. wsdl, n’est pas entièrement conforme à la norme WSDL, car il n’inclut pas de définition de service WSDL.</span><span class="sxs-lookup"><span data-stu-id="15e1a-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="15e1a-115">En effet, EWS n’est pas conçu pour être hébergé sur un ordinateur disposant d’une adresse prédéfinie.</span><span class="sxs-lookup"><span data-stu-id="15e1a-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="15e1a-116">Vous pouvez utiliser le service de découverte automatique pour obtenir l’adresse du point de terminaison EWS.</span><span class="sxs-lookup"><span data-stu-id="15e1a-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="15e1a-117">Certains générateurs de modèle objet côté client analysent le WSDL et peuvent rencontrer une condition d’erreur car le fichier WSDL ne contient pas de définition de service WSDL.</span><span class="sxs-lookup"><span data-stu-id="15e1a-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="15e1a-118">Si votre générateur de modèle objet rencontre une erreur, vous pouvez insérer une définition de service WSDL d’espace réservé.</span><span class="sxs-lookup"><span data-stu-id="15e1a-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="15e1a-119">Si vous utilisez .NET Framework pour développer votre application, nous vous recommandons d’utiliser l' [API managée EWS](http://aka.ms/ews-managed-api-readme), plutôt qu’un générateur de modèle objet.</span><span class="sxs-lookup"><span data-stu-id="15e1a-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="15e1a-120">L’API managée EWS fournit un modèle objet facile à utiliser pour gérer la sérialisation et la désérialisation du XML EWS.</span><span class="sxs-lookup"><span data-stu-id="15e1a-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="15e1a-121">Pour plus d’informations, consultez la rubrique [prise en main des applications clientes d’API managée EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="15e1a-121">For more information, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="15e1a-122">Le fichier de schéma messages. xsd contient les définitions d’élément pour les éléments de niveau supérieur dans le corps SOAP.</span><span class="sxs-lookup"><span data-stu-id="15e1a-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="15e1a-123">À l’exception des codes de réponse d’erreur, la plupart des définitions dans messages. xsd sont propres à une opération.</span><span class="sxs-lookup"><span data-stu-id="15e1a-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="15e1a-124">Le schéma types. xsd contient les définitions des en-têtes SOAP et toutes les définitions communes qui sont partagées entre les opérations.</span><span class="sxs-lookup"><span data-stu-id="15e1a-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="15e1a-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15e1a-125">See also</span></span>

- [<span data-ttu-id="15e1a-126">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="15e1a-127">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="15e1a-128">Explorer l'API managée EWS, l’EWS et les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="15e1a-129">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="15e1a-130">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15e1a-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

