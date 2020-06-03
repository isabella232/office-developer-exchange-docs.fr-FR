---
title: InstanceKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb4dbe9b-aea0-4527-b7d6-e928066caf38
description: L’élément InstanceKey spécifie une clé d’instance pour un élément ou une conversation.
ms.openlocfilehash: a6b55b9021fe63be7f678f0a1bcb24e88aeba005
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459972"
---
# <a name="instancekey"></a><span data-ttu-id="231bb-103">InstanceKey</span><span class="sxs-lookup"><span data-stu-id="231bb-103">InstanceKey</span></span>

<span data-ttu-id="231bb-104">L’élément **InstanceKey** spécifie une clé d’instance pour un élément ou une conversation.</span><span class="sxs-lookup"><span data-stu-id="231bb-104">The **InstanceKey** element specifies an instance key for an item or conversation.</span></span> 
  
```XML
<InstanceKey></InstanceKey>
```

 <span data-ttu-id="231bb-105">**Au base64Binary**</span><span class="sxs-lookup"><span data-stu-id="231bb-105">**base64Binary**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="231bb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="231bb-106">Attributes and elements</span></span>

<span data-ttu-id="231bb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="231bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="231bb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="231bb-108">Attributes</span></span>

<span data-ttu-id="231bb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="231bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="231bb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="231bb-110">Child elements</span></span>

<span data-ttu-id="231bb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="231bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="231bb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="231bb-112">Parent elements</span></span>

|<span data-ttu-id="231bb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="231bb-113">**Element**</span></span>|<span data-ttu-id="231bb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="231bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="231bb-115">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="231bb-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="231bb-116">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="231bb-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="231bb-117">Élément</span><span class="sxs-lookup"><span data-stu-id="231bb-117">Item</span></span>](item.md) <br/> |<span data-ttu-id="231bb-118">Représente un élément générique dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="231bb-118">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="231bb-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="231bb-119">Text value</span></span>

<span data-ttu-id="231bb-120">La valeur de texte de l’élément **InstanceKey** est la clé d’instance d’un élément ou d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="231bb-120">The text value of the **InstanceKey** element is the instance key for an item or conversation.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="231bb-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="231bb-121">Remarks</span></span>

<span data-ttu-id="231bb-122">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="231bb-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="231bb-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="231bb-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="231bb-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="231bb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="231bb-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="231bb-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="231bb-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="231bb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="231bb-127">Schéma type</span><span class="sxs-lookup"><span data-stu-id="231bb-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="231bb-128">Validation File</span><span class="sxs-lookup"><span data-stu-id="231bb-128">Validation File</span></span>  <br/> |<span data-ttu-id="231bb-129">types. xsd</span><span class="sxs-lookup"><span data-stu-id="231bb-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="231bb-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="231bb-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="231bb-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="231bb-131">See also</span></span>



- [<span data-ttu-id="231bb-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="231bb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

