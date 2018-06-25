---
title: GlobalUnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUnreadCount
api_type:
- schema
ms.assetid: 5e5ccf3e-2f95-4bf9-b915-8b7e59e807a5
description: L’élément GlobalUnreadCount contient un décompte de tous les éléments non lus de conversation dans la boîte aux lettres.
ms.openlocfilehash: fe001b70633198c0c1351e3c11c9542ed556a938
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827743"
---
# <a name="globalunreadcount"></a><span data-ttu-id="a7980-103">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="a7980-103">GlobalUnreadCount</span></span>

<span data-ttu-id="a7980-104">L’élément **GlobalUnreadCount** contient un décompte de tous les éléments non lus de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a7980-104">The **GlobalUnreadCount** element contains a count of all the unread conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="a7980-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="a7980-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="a7980-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="a7980-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="a7980-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a7980-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="a7980-108">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="a7980-108">GlobalUnreadCount</span></span>](globalunreadcount.md)
  
```XML
<GlobalUnreadCount/>
```

 <span data-ttu-id="a7980-109">**xs : int**</span><span class="sxs-lookup"><span data-stu-id="a7980-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a7980-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a7980-110">Attributes and elements</span></span>

<span data-ttu-id="a7980-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a7980-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a7980-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="a7980-112">Attributes</span></span>

<span data-ttu-id="a7980-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7980-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a7980-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a7980-114">Child elements</span></span>

<span data-ttu-id="a7980-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a7980-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a7980-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a7980-116">Parent elements</span></span>

|<span data-ttu-id="a7980-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a7980-117">**Element**</span></span>|<span data-ttu-id="a7980-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="a7980-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a7980-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="a7980-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="a7980-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="a7980-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a7980-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="a7980-121">Text value</span></span>

<span data-ttu-id="a7980-122">La valeur de texte de l’élément **GlobalUnreadCount** est une valeur entière qui représente le nombre de tous les éléments non lus de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a7980-122">The text value of the **GlobalUnreadCount** element is an integer value that represents a count of all the unread conversation items in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a7980-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="a7980-123">Remarks</span></span>

<span data-ttu-id="a7980-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a7980-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a7980-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a7980-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a7980-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a7980-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a7980-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a7980-127">Schema name</span></span>  <br/> |<span data-ttu-id="a7980-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="a7980-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="a7980-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a7980-129">Validation file</span></span>  <br/> |<span data-ttu-id="a7980-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a7980-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a7980-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a7980-131">Can be empty</span></span>  <br/> |<span data-ttu-id="a7980-132">False</span><span class="sxs-lookup"><span data-stu-id="a7980-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a7980-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a7980-133">See also</span></span>



[<span data-ttu-id="a7980-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="a7980-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="a7980-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="a7980-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="a7980-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="a7980-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

