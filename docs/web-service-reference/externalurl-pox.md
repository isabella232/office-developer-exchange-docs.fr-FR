---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: L’élément ExternalUrl contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 94265051be68ed06d1dab8d46dd4ce29d8694c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457955"
---
# <a name="externalurl-pox"></a><span data-ttu-id="0e2f2-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="0e2f2-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="0e2f2-104">L’élément **ExternalURL** contient l’URL permettant de connecter un client au serveur de carnet d’adresses ou à la boîte aux lettres d’un utilisateur à l’extérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/http.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0e2f2-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0e2f2-105">Attributes and elements</span></span>

<span data-ttu-id="0e2f2-106">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e2f2-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="0e2f2-107">Attributes</span></span>

<span data-ttu-id="0e2f2-108">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e2f2-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0e2f2-109">Child elements</span></span>

<span data-ttu-id="0e2f2-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e2f2-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0e2f2-111">Parent elements</span></span>

|<span data-ttu-id="0e2f2-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0e2f2-112">**Element**</span></span>|<span data-ttu-id="0e2f2-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="0e2f2-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e2f2-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="0e2f2-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="0e2f2-115">Contient les spécifications relatives à la connexion d’un client au serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="0e2f2-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="0e2f2-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="0e2f2-117">Contient les spécifications relatives à la connexion d’un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e2f2-118">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="0e2f2-118">Text value</span></span>

<span data-ttu-id="0e2f2-119">La valeur texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou à une boîte aux lettres d’utilisateur à l’extérieur de l’organisation de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0e2f2-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e2f2-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="0e2f2-120">Remarks</span></span>

<span data-ttu-id="0e2f2-121">L’élément **ExternalURL** peut être présent dans une réponse qui a un élément [Protocol (POX)](protocol-pox.md) avec une valeur d’attribut **type** « MAPI ».</span><span class="sxs-lookup"><span data-stu-id="0e2f2-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="0e2f2-122">L’élément **ExternalURL** est disponible pour les clients qui implémentent le protocole MAPI/http et ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir de Build 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="0e2f2-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="0e2f2-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0e2f2-123">See also</span></span>



[<span data-ttu-id="0e2f2-124">Éléments XML de découverte automatique de la VARIOle pour Exchange</span><span class="sxs-lookup"><span data-stu-id="0e2f2-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

