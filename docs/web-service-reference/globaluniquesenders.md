---
title: GlobalUniqueSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueSenders
api_type:
- schema
ms.assetid: 6bd9e9cb-19c8-45af-b211-dfb8a6003b1b
description: L’élément GlobalUniqueSender contient une liste de tous les expéditeurs des éléments de conversation dans la boîte aux lettres.
ms.openlocfilehash: 72dec056880c41ac9e79235dddb3c82102580a31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827751"
---
# <a name="globaluniquesenders"></a><span data-ttu-id="dafa4-103">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="dafa4-103">GlobalUniqueSenders</span></span>

<span data-ttu-id="dafa4-104">L’élément **GlobalUniqueSender** contient une liste de tous les expéditeurs des éléments de conversation dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dafa4-104">The **GlobalUniqueSender** element contains a list of all the senders of conversation items in the mailbox.</span></span> 
  
[<span data-ttu-id="dafa4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="dafa4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="dafa4-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="dafa4-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="dafa4-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="dafa4-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="dafa4-108">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="dafa4-108">GlobalUniqueSenders</span></span>](globaluniquesenders.md)
  
```XML
<GlobalUniqueSender>
   <String/>
</GlobalUniqueSender>
```

 <span data-ttu-id="dafa4-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="dafa4-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dafa4-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dafa4-110">Attributes and elements</span></span>

<span data-ttu-id="dafa4-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dafa4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dafa4-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="dafa4-112">Attributes</span></span>

<span data-ttu-id="dafa4-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dafa4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dafa4-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dafa4-114">Child elements</span></span>

|<span data-ttu-id="dafa4-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dafa4-115">**Element**</span></span>|<span data-ttu-id="dafa4-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="dafa4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dafa4-117">String</span><span class="sxs-lookup"><span data-stu-id="dafa4-117">String</span></span>](string.md) <br/> |<span data-ttu-id="dafa4-118">Contient un expéditeur de conversation unique.</span><span class="sxs-lookup"><span data-stu-id="dafa4-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dafa4-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dafa4-119">Parent elements</span></span>

|<span data-ttu-id="dafa4-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dafa4-120">**Element**</span></span>|<span data-ttu-id="dafa4-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="dafa4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dafa4-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="dafa4-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="dafa4-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="dafa4-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dafa4-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="dafa4-124">Text value</span></span>

<span data-ttu-id="dafa4-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dafa4-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dafa4-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="dafa4-126">Remarks</span></span>

<span data-ttu-id="dafa4-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="dafa4-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dafa4-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dafa4-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dafa4-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dafa4-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dafa4-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dafa4-130">Schema name</span></span>  <br/> |<span data-ttu-id="dafa4-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="dafa4-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="dafa4-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dafa4-132">Validation file</span></span>  <br/> |<span data-ttu-id="dafa4-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dafa4-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dafa4-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dafa4-134">Can be empty</span></span>  <br/> |<span data-ttu-id="dafa4-135">False</span><span class="sxs-lookup"><span data-stu-id="dafa4-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dafa4-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dafa4-136">See also</span></span>



[<span data-ttu-id="dafa4-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="dafa4-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="dafa4-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="dafa4-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="dafa4-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="dafa4-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)
