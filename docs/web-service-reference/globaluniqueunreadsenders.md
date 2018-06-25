---
title: GlobalUniqueUnreadSenders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalUniqueUnreadSenders
api_type:
- schema
ms.assetid: 490abe30-7608-407a-923b-a4b3ddbca610
description: L’élément GlobalUniqueUnreadSenders spécifie une liste de toutes les personnes qui ont envoyé les messages qui sont actuellement non lus dans cette conversation entre tous les dossiers dans la boîte aux lettres.
ms.openlocfilehash: ae088577f5aac0c7c3ee9c11fde184b70ab12e64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827749"
---
# <a name="globaluniqueunreadsenders"></a><span data-ttu-id="67aaf-103">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="67aaf-103">GlobalUniqueUnreadSenders</span></span>

<span data-ttu-id="67aaf-104">L’élément **GlobalUniqueUnreadSenders** spécifie une liste de toutes les personnes qui ont envoyé les messages qui sont actuellement non lus dans cette conversation entre tous les dossiers dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="67aaf-104">The **GlobalUniqueUnreadSenders** element specifies a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="67aaf-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="67aaf-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="67aaf-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="67aaf-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="67aaf-107">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="67aaf-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="67aaf-108">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="67aaf-108">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md)
  
```XML
<GlobalUniqueUnreadSenders>
   <String/>
</GlobalUniqueUnreadSenders>
```

 <span data-ttu-id="67aaf-109">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="67aaf-109">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67aaf-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="67aaf-110">Attributes and elements</span></span>

<span data-ttu-id="67aaf-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="67aaf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67aaf-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="67aaf-112">Attributes</span></span>

<span data-ttu-id="67aaf-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="67aaf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67aaf-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="67aaf-114">Child elements</span></span>

|<span data-ttu-id="67aaf-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67aaf-115">**Element**</span></span>|<span data-ttu-id="67aaf-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="67aaf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67aaf-117">String</span><span class="sxs-lookup"><span data-stu-id="67aaf-117">String</span></span>](string.md) <br/> |<span data-ttu-id="67aaf-118">Contient un expéditeur de conversation unique.</span><span class="sxs-lookup"><span data-stu-id="67aaf-118">Contains a single conversation sender.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67aaf-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="67aaf-119">Parent elements</span></span>

|<span data-ttu-id="67aaf-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67aaf-120">**Element**</span></span>|<span data-ttu-id="67aaf-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="67aaf-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67aaf-122">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="67aaf-122">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="67aaf-123">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="67aaf-123">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67aaf-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="67aaf-124">Text value</span></span>

<span data-ttu-id="67aaf-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="67aaf-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="67aaf-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="67aaf-126">Remarks</span></span>

<span data-ttu-id="67aaf-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="67aaf-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67aaf-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="67aaf-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67aaf-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="67aaf-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="67aaf-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="67aaf-130">Schema name</span></span>  <br/> |<span data-ttu-id="67aaf-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="67aaf-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="67aaf-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="67aaf-132">Validation file</span></span>  <br/> |<span data-ttu-id="67aaf-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="67aaf-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="67aaf-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="67aaf-134">Can be empty</span></span>  <br/> |<span data-ttu-id="67aaf-135">False</span><span class="sxs-lookup"><span data-stu-id="67aaf-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67aaf-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67aaf-136">See also</span></span>



[<span data-ttu-id="67aaf-137">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="67aaf-137">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="67aaf-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="67aaf-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="67aaf-139">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="67aaf-139">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

