---
title: Conversations
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversations
api_type:
- schema
ms.assetid: 1d18f98c-6457-45e9-a934-32da20885ac6
description: L’élément conversations contient un tableau de conversations qui sont renvoyées dans la réponse FindConversation.
ms.openlocfilehash: 8af1023db51dd955c544422520ec5565f09f5372
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463796"
---
# <a name="conversations"></a><span data-ttu-id="d0c5b-103">Conversations</span><span class="sxs-lookup"><span data-stu-id="d0c5b-103">Conversations</span></span>

<span data-ttu-id="d0c5b-104">L’élément **conversations** contient un tableau de conversations qui sont renvoyées dans la réponse **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d0c5b-104">The **Conversations** element contains an array of conversations that are returned in the **FindConversation** response.</span></span> 
  
[<span data-ttu-id="d0c5b-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d0c5b-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="d0c5b-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="d0c5b-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
```xml
<Conversations>
   <Conversation/>
</Conversations>
```

 <span data-ttu-id="d0c5b-107">**ArrayOfConversationsType**</span><span class="sxs-lookup"><span data-stu-id="d0c5b-107">**ArrayOfConversationsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0c5b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d0c5b-108">Attributes and elements</span></span>

<span data-ttu-id="d0c5b-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d0c5b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0c5b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d0c5b-110">Attributes</span></span>

<span data-ttu-id="d0c5b-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d0c5b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0c5b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d0c5b-112">Child elements</span></span>

|<span data-ttu-id="d0c5b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0c5b-113">**Element**</span></span>|<span data-ttu-id="d0c5b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0c5b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0c5b-115">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d0c5b-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d0c5b-116">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="d0c5b-116">Represents a single conversation.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0c5b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d0c5b-117">Parent elements</span></span>

|<span data-ttu-id="d0c5b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0c5b-118">**Element**</span></span>|<span data-ttu-id="d0c5b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0c5b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0c5b-120">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="d0c5b-120">FindConversationResponse</span></span>](findconversationresponse.md) <br/> |<span data-ttu-id="d0c5b-121">Définit une réponse à une demande **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="d0c5b-121">Defines a response to a **FindConversation** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0c5b-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d0c5b-122">Text value</span></span>

<span data-ttu-id="d0c5b-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0c5b-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0c5b-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="d0c5b-124">Remarks</span></span>

<span data-ttu-id="d0c5b-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="d0c5b-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0c5b-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d0c5b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0c5b-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d0c5b-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0c5b-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d0c5b-128">Schema name</span></span>  <br/> |<span data-ttu-id="d0c5b-129">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d0c5b-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0c5b-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d0c5b-130">Validation file</span></span>  <br/> |<span data-ttu-id="d0c5b-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d0c5b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0c5b-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d0c5b-132">Can be empty</span></span>  <br/> |<span data-ttu-id="d0c5b-133">False</span><span class="sxs-lookup"><span data-stu-id="d0c5b-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0c5b-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0c5b-134">See also</span></span>



[<span data-ttu-id="d0c5b-135">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="d0c5b-135">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="d0c5b-136">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="d0c5b-136">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

