---
title: Carnet d’adresses (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: L’élément de carnet d’adresses contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: c30f0ee7c36de7e63157d07d003a11187d661fd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755179"
---
# <a name="addressbook-pox"></a><span data-ttu-id="bd619-103">Carnet d’adresses (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-103">AddressBook (POX)</span></span>

<span data-ttu-id="bd619-104">L’élément de **Carnet d’adresses** contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="bd619-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="bd619-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="bd619-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="bd619-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="bd619-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="bd619-109">Carnet d’adresses (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="bd619-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bd619-110">Attributes and elements</span></span>

<span data-ttu-id="bd619-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bd619-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd619-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="bd619-112">Attributes</span></span>

<span data-ttu-id="bd619-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bd619-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd619-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bd619-114">Child elements</span></span>

|<span data-ttu-id="bd619-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd619-115">**Element**</span></span>|<span data-ttu-id="bd619-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd619-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd619-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="bd619-118">Contient l’URL qui doit être utilisé pour accéder au carnet d’adresses à partir de l’extérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="bd619-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="bd619-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="bd619-120">Contient l’URL qui doit être utilisé pour accéder à du carnet d’adresses à partir de l’intérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="bd619-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd619-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bd619-121">Parent elements</span></span>

|<span data-ttu-id="bd619-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bd619-122">**Element**</span></span>|<span data-ttu-id="bd619-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="bd619-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd619-124">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="bd619-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="bd619-125">Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="bd619-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd619-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="bd619-126">Remarks</span></span>

<span data-ttu-id="bd619-127">L’élément de **Carnet d’adresses** est présente dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ».</span><span class="sxs-lookup"><span data-stu-id="bd619-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="bd619-128">L’élément de **Carnet d’adresses** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) .</span><span class="sxs-lookup"><span data-stu-id="bd619-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bd619-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bd619-129">See also</span></span>

- [<span data-ttu-id="bd619-130">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="bd619-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
