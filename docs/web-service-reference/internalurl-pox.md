---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: L’élément InternalUrl contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à partir de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 9c6ba621a681ec54d88089de6b7ae1eefdebc679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465575"
---
# <a name="internalurl-pox"></a><span data-ttu-id="6fb00-103">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="6fb00-103">InternalUrl (POX)</span></span>

<span data-ttu-id="6fb00-104">L’élément **InternalURL** contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à partir de l’organisation de l’utilisateur à l’aide du protocole MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="6fb00-104">The **InternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from inside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6fb00-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6fb00-105">Attributes and elements</span></span>

<span data-ttu-id="6fb00-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6fb00-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fb00-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="6fb00-107">Attributes</span></span>

<span data-ttu-id="6fb00-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="6fb00-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fb00-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6fb00-109">Child elements</span></span>

<span data-ttu-id="6fb00-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6fb00-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6fb00-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6fb00-111">Parent elements</span></span>

|<span data-ttu-id="6fb00-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6fb00-112">**Element**</span></span>|<span data-ttu-id="6fb00-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6fb00-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fb00-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="6fb00-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="6fb00-115">Contient les spécifications relatives à la connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="6fb00-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="6fb00-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="6fb00-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="6fb00-117">Contient les spécifications relatives à la connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="6fb00-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6fb00-118">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="6fb00-118">Text value</span></span>

<span data-ttu-id="6fb00-119">La valeur texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou à une boîte aux lettres de l’utilisateur à l’intérieur de l’organisation de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="6fb00-119">The text value represents a URL that can be used to access an address book server or user's mailbox from inside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6fb00-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="6fb00-120">Remarks</span></span>

<span data-ttu-id="6fb00-121">L’élément **InternalURL** peut être présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) avec une valeur d’attribut **type** « MAPI ».</span><span class="sxs-lookup"><span data-stu-id="6fb00-121">The **InternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="6fb00-122">L’élément **InternalURL** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de la version 15.00.0847.032 (exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="6fb00-122">The **InternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6fb00-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6fb00-123">See also</span></span>



[<span data-ttu-id="6fb00-124">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="6fb00-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

