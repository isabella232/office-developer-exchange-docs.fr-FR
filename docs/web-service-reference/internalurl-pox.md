---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: L’élément InternalUrl contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’intérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827950"
---
# <a name="internalurl-pox"></a><span data-ttu-id="19212-103">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="19212-103">InternalUrl (POX)</span></span>

<span data-ttu-id="19212-104">L’élément **InternalUrl** contient l’URL pour la connexion d’un client pour le serveur de carnet d’adresses ou de boîte aux lettres d’un utilisateur à l’intérieur de l’organisation de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="19212-104">The **InternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from inside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="19212-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19212-105">Attributes and elements</span></span>

<span data-ttu-id="19212-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19212-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19212-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="19212-107">Attributes</span></span>

<span data-ttu-id="19212-108">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19212-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19212-109">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19212-109">Child elements</span></span>

<span data-ttu-id="19212-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19212-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19212-111">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19212-111">Parent elements</span></span>

|<span data-ttu-id="19212-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19212-112">**Element**</span></span>|<span data-ttu-id="19212-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="19212-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19212-114">Carnet d’adresses (POX)</span><span class="sxs-lookup"><span data-stu-id="19212-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="19212-115">Contient les spécifications pour la connexion d’un client pour le serveur de carnet d’adresses à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="19212-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="19212-116">Magasin de courrier électronique (POX)</span><span class="sxs-lookup"><span data-stu-id="19212-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="19212-117">Contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="19212-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19212-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="19212-118">Text value</span></span>

<span data-ttu-id="19212-119">La valeur de texte représente une URL qui peut être utilisée pour accéder à un serveur de carnet d’adresses ou de boîte aux lettres d’utilisateur à l’intérieur de l’organisation de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="19212-119">The text value represents a URL that can be used to access an address book server or user's mailbox from inside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19212-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="19212-120">Remarks</span></span>

<span data-ttu-id="19212-121">L’élément **InternalUrl** peut être présent dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ».</span><span class="sxs-lookup"><span data-stu-id="19212-121">The **InternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="19212-122">L’élément **InternalUrl** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1) .</span><span class="sxs-lookup"><span data-stu-id="19212-122">The **InternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="19212-123">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="19212-123">See also</span></span>



[<span data-ttu-id="19212-124">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="19212-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

