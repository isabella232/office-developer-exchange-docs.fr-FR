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
description: L’élément GlobalUnreadCount contient le décompte de tous les éléments de conversation non lus dans la boîte aux lettres.
ms.openlocfilehash: 976067078908523936769b2856712e3e6908f0c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530112"
---
# <a name="globalunreadcount"></a><span data-ttu-id="bff07-103">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="bff07-103">GlobalUnreadCount</span></span>

<span data-ttu-id="bff07-104">L’élément **GlobalUnreadCount** contient le décompte de tous les éléments de conversation non lus dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bff07-104">The **GlobalUnreadCount** element contains a count of all the unread conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="bff07-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="bff07-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="bff07-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="bff07-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="bff07-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bff07-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="bff07-108">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="bff07-108">GlobalUnreadCount</span></span>](globalunreadcount.md)
  
```XML
<GlobalUnreadCount/>
```

 <span data-ttu-id="bff07-109">**XS : int**</span><span class="sxs-lookup"><span data-stu-id="bff07-109">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bff07-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="bff07-110">Attributes and elements</span></span>

<span data-ttu-id="bff07-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="bff07-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bff07-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="bff07-112">Attributes</span></span>

<span data-ttu-id="bff07-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="bff07-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bff07-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="bff07-114">Child elements</span></span>

<span data-ttu-id="bff07-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="bff07-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bff07-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="bff07-116">Parent elements</span></span>

|<span data-ttu-id="bff07-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="bff07-117">**Element**</span></span>|<span data-ttu-id="bff07-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="bff07-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bff07-119">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="bff07-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="bff07-120">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="bff07-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bff07-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="bff07-121">Text value</span></span>

<span data-ttu-id="bff07-122">La valeur de texte de l’élément **GlobalUnreadCount** est une valeur entière qui représente le nombre de tous les éléments de conversation non lus dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="bff07-122">The text value of the **GlobalUnreadCount** element is an integer value that represents a count of all the unread conversation items in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="bff07-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="bff07-123">Remarks</span></span>

<span data-ttu-id="bff07-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="bff07-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bff07-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="bff07-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bff07-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="bff07-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bff07-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="bff07-127">Schema name</span></span>  <br/> |<span data-ttu-id="bff07-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="bff07-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="bff07-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="bff07-129">Validation file</span></span>  <br/> |<span data-ttu-id="bff07-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bff07-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bff07-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="bff07-131">Can be empty</span></span>  <br/> |<span data-ttu-id="bff07-132">False</span><span class="sxs-lookup"><span data-stu-id="bff07-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bff07-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="bff07-133">See also</span></span>



[<span data-ttu-id="bff07-134">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="bff07-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="bff07-135">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="bff07-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="bff07-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="bff07-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

