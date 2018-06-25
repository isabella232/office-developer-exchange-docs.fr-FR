---
title: UniqueRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueRecipients
api_type:
- schema
ms.assetid: 9f46ed05-5370-46ee-80f5-83f97224c76e
description: L'élément UniqueRecipients contient la liste des destinataires d'une conversation dans un dossier spécifique. Cet élément est en lecture seule.
ms.openlocfilehash: 710559e599c6cec1db371165f01187f8960024f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838830"
---
# <a name="uniquerecipients"></a><span data-ttu-id="e93f0-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e93f0-104">UniqueRecipients</span></span>

<span data-ttu-id="e93f0-p102">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **UniqueRecipients** contient la liste des destinataires d'une conversation dans un dossier spécifique. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e93f0-p102">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder. This element is read-only.</span></span> 
  
[<span data-ttu-id="e93f0-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="e93f0-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="e93f0-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="e93f0-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="e93f0-109">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e93f0-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="e93f0-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e93f0-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="e93f0-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e93f0-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e93f0-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e93f0-112">Attributes and elements</span></span>

<span data-ttu-id="e93f0-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e93f0-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e93f0-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="e93f0-114">Attributes</span></span>

<span data-ttu-id="e93f0-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e93f0-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e93f0-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e93f0-116">Child elements</span></span>

|<span data-ttu-id="e93f0-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e93f0-117">**Element**</span></span>|<span data-ttu-id="e93f0-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="e93f0-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e93f0-119">String</span><span class="sxs-lookup"><span data-stu-id="e93f0-119">String</span></span>](string.md) <br/> |<span data-ttu-id="e93f0-p103">Représente un destinataire unique d'une conversation. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e93f0-p103">Represents a unique recipient of a conversation. This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e93f0-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e93f0-122">Parent elements</span></span>

|<span data-ttu-id="e93f0-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e93f0-123">**Element**</span></span>|<span data-ttu-id="e93f0-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="e93f0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e93f0-125">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e93f0-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e93f0-126">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="e93f0-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e93f0-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e93f0-127">Text value</span></span>

<span data-ttu-id="e93f0-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e93f0-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e93f0-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="e93f0-129">Remarks</span></span>

<span data-ttu-id="e93f0-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e93f0-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e93f0-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e93f0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e93f0-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e93f0-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e93f0-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e93f0-133">Schema name</span></span>  <br/> |<span data-ttu-id="e93f0-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e93f0-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e93f0-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e93f0-135">Validation file</span></span>  <br/> |<span data-ttu-id="e93f0-136">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e93f0-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e93f0-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e93f0-137">Can be empty</span></span>  <br/> |<span data-ttu-id="e93f0-138">False</span><span class="sxs-lookup"><span data-stu-id="e93f0-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e93f0-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e93f0-139">See also</span></span>



[<span data-ttu-id="e93f0-140">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="e93f0-140">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="e93f0-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="e93f0-141">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

