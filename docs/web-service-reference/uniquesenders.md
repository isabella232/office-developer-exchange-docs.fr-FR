---
title: UniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueSenders
api_type:
- schema
ms.assetid: 1f55f2fe-b2f2-4169-83c1-fa5c752bd695
description: L’élément UniqueSenders contient une liste de tous les expéditeurs des éléments de conversation dans le dossier actif. Cet élément est en lecture seule.
ms.openlocfilehash: b75846534141e23e6d8158bc36f0ef60bcb1d7ad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838825"
---
# <a name="uniquesenders"></a><span data-ttu-id="3be17-104">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="3be17-104">UniqueSenders</span></span>

<span data-ttu-id="3be17-105">L’élément **UniqueSenders** contient une liste de tous les expéditeurs des éléments de conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="3be17-105">The **UniqueSenders** element contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="3be17-106">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="3be17-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="3be17-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="3be17-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="3be17-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="3be17-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="3be17-109">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3be17-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="3be17-110">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="3be17-110">UniqueSenders</span></span>](uniquesenders.md)
  
```XML
<UniqueSenders>
   <String/>
</UniqueSenders>
```

 <span data-ttu-id="3be17-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="3be17-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3be17-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3be17-112">Attributes and elements</span></span>

<span data-ttu-id="3be17-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3be17-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3be17-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="3be17-114">Attributes</span></span>

<span data-ttu-id="3be17-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3be17-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3be17-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3be17-116">Child elements</span></span>

|<span data-ttu-id="3be17-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3be17-117">**Element**</span></span>|<span data-ttu-id="3be17-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="3be17-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3be17-119">String</span><span class="sxs-lookup"><span data-stu-id="3be17-119">String</span></span>](string.md) <br/> |<span data-ttu-id="3be17-120">Contient un expéditeur de conversation unique.</span><span class="sxs-lookup"><span data-stu-id="3be17-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3be17-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3be17-121">Parent elements</span></span>

|<span data-ttu-id="3be17-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3be17-122">**Element**</span></span>|<span data-ttu-id="3be17-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="3be17-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3be17-124">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3be17-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3be17-125">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="3be17-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3be17-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="3be17-126">Text value</span></span>

<span data-ttu-id="3be17-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3be17-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3be17-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="3be17-128">Remarks</span></span>

<span data-ttu-id="3be17-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="3be17-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3be17-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3be17-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3be17-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3be17-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3be17-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3be17-132">Schema name</span></span>  <br/> |<span data-ttu-id="3be17-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="3be17-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="3be17-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3be17-134">Validation file</span></span>  <br/> |<span data-ttu-id="3be17-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3be17-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3be17-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3be17-136">Can be empty</span></span>  <br/> |<span data-ttu-id="3be17-137">False</span><span class="sxs-lookup"><span data-stu-id="3be17-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3be17-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3be17-138">See also</span></span>



[<span data-ttu-id="3be17-139">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="3be17-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="3be17-140">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="3be17-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="3be17-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="3be17-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

