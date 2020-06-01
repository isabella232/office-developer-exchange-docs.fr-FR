---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: L’élément AddressBook contient les spécifications permettant de connecter un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 0967ac123cd3bb0086fd004ea0d0d37c08d2e037
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463635"
---
# <a name="addressbook-pox"></a><span data-ttu-id="3e916-103">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-103">AddressBook (POX)</span></span>

<span data-ttu-id="3e916-104">L’élément **AddressBook** contient les spécifications permettant de connecter un client au serveur de carnet d’adresses à l’aide du protocole MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="3e916-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="3e916-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="3e916-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="3e916-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="3e916-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="3e916-109">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3e916-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3e916-110">Attributes and elements</span></span>

<span data-ttu-id="3e916-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3e916-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e916-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="3e916-112">Attributes</span></span>

<span data-ttu-id="3e916-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3e916-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e916-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3e916-114">Child elements</span></span>

|<span data-ttu-id="3e916-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e916-115">**Element**</span></span>|<span data-ttu-id="3e916-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e916-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e916-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="3e916-118">Contient l’URL à utiliser pour accéder au carnet d’adresses en dehors du réseau de l’organisation à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="3e916-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="3e916-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="3e916-120">Contient l’URL à utiliser pour accéder au carnet d’adresses depuis l’intérieur du réseau de l’organisation à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="3e916-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e916-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3e916-121">Parent elements</span></span>

|<span data-ttu-id="3e916-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e916-122">**Element**</span></span>|<span data-ttu-id="3e916-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e916-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e916-124">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="3e916-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="3e916-125">Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="3e916-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3e916-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="3e916-126">Remarks</span></span>

<span data-ttu-id="3e916-127">L’élément **AddressBook** est présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) avec une valeur d’attribut de **type** « MAPI ».</span><span class="sxs-lookup"><span data-stu-id="3e916-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="3e916-128">L’élément **AddressBook** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="3e916-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3e916-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e916-129">See also</span></span>

- [<span data-ttu-id="3e916-130">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3e916-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

