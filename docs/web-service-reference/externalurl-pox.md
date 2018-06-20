---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: L’élément ExternalUrl contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756338"
---
# <a name="externalurl-pox"></a><span data-ttu-id="e15ce-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e15ce-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="e15ce-104">L’élément **ExternalUrl** contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e15ce-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e15ce-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e15ce-105">Attributes and elements</span></span>

<span data-ttu-id="e15ce-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e15ce-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e15ce-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="e15ce-107">Attributes</span></span>

<span data-ttu-id="e15ce-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e15ce-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e15ce-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e15ce-109">Child elements</span></span>

<span data-ttu-id="e15ce-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e15ce-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e15ce-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e15ce-111">Parent elements</span></span>

|<span data-ttu-id="e15ce-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e15ce-112">**Element**</span></span>|<span data-ttu-id="e15ce-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="e15ce-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e15ce-114">Carnet d’adresses (POX)</span><span class="sxs-lookup"><span data-stu-id="e15ce-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="e15ce-115">Contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e15ce-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="e15ce-116">Magasin de courrier électronique (POX)</span><span class="sxs-lookup"><span data-stu-id="e15ce-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="e15ce-117">Contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e15ce-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e15ce-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e15ce-118">Text value</span></span>

<span data-ttu-id="e15ce-119">La valeur de texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou de boîte aux lettres à partir de l’extérieur de l’organisation de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="e15ce-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e15ce-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="e15ce-120">Remarks</span></span>

<span data-ttu-id="e15ce-121">L’élément **ExternalUrl** peut être présent dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ».</span><span class="sxs-lookup"><span data-stu-id="e15ce-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="e15ce-122">L’élément **ExternalUrl** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) .</span><span class="sxs-lookup"><span data-stu-id="e15ce-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e15ce-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e15ce-123">See also</span></span>



[<span data-ttu-id="e15ce-124">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e15ce-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

