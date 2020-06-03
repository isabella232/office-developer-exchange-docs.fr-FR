---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: L’élément MailStore contient les spécifications permettant de connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 635228fcfeb3ad791c845050b82666a6e060b229
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459790"
---
# <a name="mailstore-pox"></a><span data-ttu-id="e629d-103">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-103">MailStore (POX)</span></span>

<span data-ttu-id="e629d-104">L’élément **mailstore** contient les spécifications permettant de connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="e629d-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="e629d-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="e629d-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="e629d-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="e629d-108">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="e629d-109">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e629d-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e629d-110">Attributes and elements</span></span>

<span data-ttu-id="e629d-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e629d-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e629d-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="e629d-112">Attributes</span></span>

<span data-ttu-id="e629d-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e629d-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e629d-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e629d-114">Child elements</span></span>

|<span data-ttu-id="e629d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e629d-115">**Element**</span></span>|<span data-ttu-id="e629d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="e629d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e629d-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="e629d-118">Contient l’URL à utiliser pour accéder à la boîte aux lettres de l’utilisateur depuis l’extérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e629d-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="e629d-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="e629d-120">Contient l’URL à utiliser pour accéder à la boîte aux lettres de l’utilisateur à partir du réseau de l’organisation au moyen du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="e629d-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e629d-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e629d-121">Parent elements</span></span>

|<span data-ttu-id="e629d-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e629d-122">**Element**</span></span>|<span data-ttu-id="e629d-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="e629d-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e629d-124">Protocol (POX)</span><span class="sxs-lookup"><span data-stu-id="e629d-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="e629d-125">Contient les spécifications relatives à la connexion d’un client au serveur d’accès au client.</span><span class="sxs-lookup"><span data-stu-id="e629d-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e629d-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="e629d-126">Remarks</span></span>

<span data-ttu-id="e629d-127">L’élément **mailstore** est présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) dont la valeur d’attribut **type** est « MAPI ».</span><span class="sxs-lookup"><span data-stu-id="e629d-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="e629d-128">L’élément **mailstore** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de la version 15.00.0847.032 (exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="e629d-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e629d-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e629d-129">See also</span></span>



[<span data-ttu-id="e629d-130">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e629d-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

