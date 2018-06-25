---
title: Magasin de courrier électronique (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: L’élément de magasin de courrier électronique contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828301"
---
# <a name="mailstore-pox"></a><span data-ttu-id="4334a-103">Magasin de courrier électronique (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-103">MailStore (POX)</span></span>

<span data-ttu-id="4334a-104">L’élément de **magasin de courrier électronique** contient les spécifications pour connecter un client à la boîte aux lettres de l’utilisateur à l’aide du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="4334a-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="4334a-105">Découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="4334a-106">Réponse (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="4334a-107">Compte (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="4334a-108">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="4334a-109">Magasin de courrier électronique (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="4334a-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4334a-110">Attributes and elements</span></span>

<span data-ttu-id="4334a-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4334a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4334a-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="4334a-112">Attributes</span></span>

<span data-ttu-id="4334a-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4334a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4334a-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4334a-114">Child elements</span></span>

|<span data-ttu-id="4334a-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4334a-115">**Element**</span></span>|<span data-ttu-id="4334a-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="4334a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4334a-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="4334a-118">Contient l’URL qui doit être utilisé pour accéder à la boîte aux lettres à partir de l’extérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="4334a-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="4334a-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="4334a-120">Contient l’URL qui doit être utilisé pour accéder à la boîte aux lettres à partir de l’intérieur du réseau de l’organisation au moyen du protocole MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="4334a-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4334a-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4334a-121">Parent elements</span></span>

|<span data-ttu-id="4334a-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4334a-122">**Element**</span></span>|<span data-ttu-id="4334a-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="4334a-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4334a-124">Protocole (POX)</span><span class="sxs-lookup"><span data-stu-id="4334a-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="4334a-125">Contient les spécifications pour la connexion d’un client vers le serveur d’accès au Client.</span><span class="sxs-lookup"><span data-stu-id="4334a-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4334a-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="4334a-126">Remarks</span></span>

<span data-ttu-id="4334a-127">L’élément de **magasin de courrier électronique** est présente dans une réponse qui a un élément de [Protocole (POX)](protocol-pox.md) avec une valeur d’attribut de **Type** de « mapiHttp ».</span><span class="sxs-lookup"><span data-stu-id="4334a-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="4334a-128">L’élément de **magasin de courrier électronique** est disponible pour les clients qui implémentent le protocole MAPI/HTTP et cible Exchange Online, Exchange Online dans le cadre d’Office 365, et créer des versions locales d’Exchange commençant par 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="4334a-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4334a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4334a-129">See also</span></span>



[<span data-ttu-id="4334a-130">Éléments du fichier XML Autodiscover variole pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4334a-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

