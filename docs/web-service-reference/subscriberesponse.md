---
title: SubscribeResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponse
api_type:
- schema
ms.assetid: fd87e9b7-c231-44fa-9f5b-19ae96cda5cc
description: L’élément SubscribeResponse définit une réponse à une demande subscribe.
ms.openlocfilehash: 1f7079694c873aacbf44b1030e495cbe2f48d163
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530950"
---
# <a name="subscriberesponse"></a><span data-ttu-id="bb679-103">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="bb679-103">SubscribeResponse</span></span>

<span data-ttu-id="bb679-104">L’élément **SubscribeResponse** définit une réponse à une demande subscribe.</span><span class="sxs-lookup"><span data-stu-id="bb679-104">The **SubscribeResponse** element defines a response to a Subscribe request.</span></span> 
  
[<span data-ttu-id="bb679-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="bb679-105">SubscribeResponse</span></span>](subscriberesponse.md)
  
```xml
<SubscribeResponse>
   <ResponseMessages/>
</SubscribeResponse>
```

 <span data-ttu-id="bb679-106">**SubscribeResponseType**</span><span class="sxs-lookup"><span data-stu-id="bb679-106">**SubscribeResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bb679-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bb679-107">Attributes and elements</span></span>

<span data-ttu-id="bb679-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bb679-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bb679-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="bb679-109">Attributes</span></span>

<span data-ttu-id="bb679-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bb679-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bb679-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bb679-111">Child elements</span></span>

|<span data-ttu-id="bb679-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bb679-112">**Element**</span></span>|<span data-ttu-id="bb679-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="bb679-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb679-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bb679-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bb679-115">Contient les messages de réponse pour une demande des services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="bb679-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bb679-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bb679-116">Parent elements</span></span>

<span data-ttu-id="bb679-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bb679-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bb679-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="bb679-118">Remarks</span></span>

<span data-ttu-id="bb679-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="bb679-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bb679-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bb679-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bb679-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bb679-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bb679-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bb679-122">Schema name</span></span>  <br/> |<span data-ttu-id="bb679-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="bb679-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="bb679-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bb679-124">Validation file</span></span>  <br/> |<span data-ttu-id="bb679-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bb679-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bb679-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bb679-126">Can be empty</span></span>  <br/> |<span data-ttu-id="bb679-127">True</span><span class="sxs-lookup"><span data-stu-id="bb679-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bb679-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bb679-128">See also</span></span>



[<span data-ttu-id="bb679-129">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="bb679-129">Subscribe operation</span></span>](subscribe-operation.md)

