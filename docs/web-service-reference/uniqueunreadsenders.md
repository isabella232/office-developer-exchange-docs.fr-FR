---
title: UniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueUnreadSenders
api_type:
- schema
ms.assetid: eb7d1274-ce2e-4ef8-b47f-e911174aab0c
description: L’élément UniqueUnreadSenders contient la liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation dans le dossier actif. Cet élément est en lecture seule.
ms.openlocfilehash: 0e45362e88be4930b8bc2f641c1fb00cc63c0605
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458851"
---
# <a name="uniqueunreadsenders"></a><span data-ttu-id="d89fe-104">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="d89fe-104">UniqueUnreadSenders</span></span>

<span data-ttu-id="d89fe-105">L’élément **UniqueUnreadSenders** contient la liste de toutes les personnes qui ont envoyé des messages non lus dans cette conversation dans le dossier actif.</span><span class="sxs-lookup"><span data-stu-id="d89fe-105">The **UniqueUnreadSenders** element contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="d89fe-106">Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="d89fe-106">This element is read-only.</span></span> 
  
[<span data-ttu-id="d89fe-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d89fe-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d89fe-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="d89fe-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="d89fe-109">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d89fe-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="d89fe-110">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="d89fe-110">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md)
  
```XML
<UniqueUnreadSenders>
   <String/>
</UniqueUnreadSenders>
```

 <span data-ttu-id="d89fe-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="d89fe-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d89fe-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d89fe-112">Attributes and elements</span></span>

<span data-ttu-id="d89fe-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d89fe-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d89fe-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="d89fe-114">Attributes</span></span>

<span data-ttu-id="d89fe-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d89fe-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d89fe-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d89fe-116">Child elements</span></span>

|<span data-ttu-id="d89fe-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d89fe-117">**Element**</span></span>|<span data-ttu-id="d89fe-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="d89fe-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89fe-119">String</span><span class="sxs-lookup"><span data-stu-id="d89fe-119">String</span></span>](string.md) <br/> |<span data-ttu-id="d89fe-120">Contient un seul expéditeur de conversation.</span><span class="sxs-lookup"><span data-stu-id="d89fe-120">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d89fe-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d89fe-121">Parent elements</span></span>

|<span data-ttu-id="d89fe-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d89fe-122">**Element**</span></span>|<span data-ttu-id="d89fe-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d89fe-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d89fe-124">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d89fe-124">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d89fe-125">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="d89fe-125">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d89fe-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d89fe-126">Text value</span></span>

<span data-ttu-id="d89fe-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d89fe-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d89fe-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="d89fe-128">Remarks</span></span>

<span data-ttu-id="d89fe-129">Cet élément a été introduit dans Exchange Server 2010 Service Pack 1 (SP1). Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d89fe-129">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d89fe-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d89fe-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d89fe-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d89fe-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d89fe-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d89fe-132">Schema name</span></span>  <br/> |<span data-ttu-id="d89fe-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d89fe-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d89fe-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d89fe-134">Validation file</span></span>  <br/> |<span data-ttu-id="d89fe-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d89fe-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d89fe-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d89fe-136">Can be empty</span></span>  <br/> |<span data-ttu-id="d89fe-137">False</span><span class="sxs-lookup"><span data-stu-id="d89fe-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d89fe-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d89fe-138">See also</span></span>



[<span data-ttu-id="d89fe-139">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="d89fe-139">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="d89fe-140">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="d89fe-140">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="d89fe-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="d89fe-141">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

