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
ms.openlocfilehash: d7f6b0aa01aceb6a251fb0c46d89b34cad260acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530725"
---
# <a name="uniquerecipients"></a><span data-ttu-id="e8666-104">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e8666-104">UniqueRecipients</span></span>

<span data-ttu-id="e8666-p102">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **UniqueRecipients** contient la liste des destinataires d'une conversation dans un dossier spécifique. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e8666-p102">The **UniqueRecipients** element contains the recipient list of a conversation in a particular folder. This element is read-only.</span></span> 
  
[<span data-ttu-id="e8666-107">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="e8666-107">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="e8666-108">Conversations</span><span class="sxs-lookup"><span data-stu-id="e8666-108">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="e8666-109">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e8666-109">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="e8666-110">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="e8666-110">UniqueRecipients</span></span>](uniquerecipients.md)
  
```XML
<UniqueRecpients>
   <String/>
</UniqueRecpients>
```

 <span data-ttu-id="e8666-111">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="e8666-111">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8666-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e8666-112">Attributes and elements</span></span>

<span data-ttu-id="e8666-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e8666-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8666-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="e8666-114">Attributes</span></span>

<span data-ttu-id="e8666-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e8666-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8666-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e8666-116">Child elements</span></span>

|<span data-ttu-id="e8666-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e8666-117">**Element**</span></span>|<span data-ttu-id="e8666-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="e8666-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8666-119">String</span><span class="sxs-lookup"><span data-stu-id="e8666-119">String</span></span>](string.md) <br/> |<span data-ttu-id="e8666-p103">Représente un destinataire unique d'une conversation. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="e8666-p103">Represents a unique recipient of a conversation. This element is read-only.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8666-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e8666-122">Parent elements</span></span>

|<span data-ttu-id="e8666-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e8666-123">**Element**</span></span>|<span data-ttu-id="e8666-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="e8666-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8666-125">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="e8666-125">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="e8666-126">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="e8666-126">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8666-127">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e8666-127">Text value</span></span>

<span data-ttu-id="e8666-128">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e8666-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8666-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="e8666-129">Remarks</span></span>

<span data-ttu-id="e8666-130">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e8666-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8666-131">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e8666-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8666-132">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e8666-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8666-133">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e8666-133">Schema name</span></span>  <br/> |<span data-ttu-id="e8666-134">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="e8666-134">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8666-135">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e8666-135">Validation file</span></span>  <br/> |<span data-ttu-id="e8666-136">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e8666-136">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8666-137">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e8666-137">Can be empty</span></span>  <br/> |<span data-ttu-id="e8666-138">False</span><span class="sxs-lookup"><span data-stu-id="e8666-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8666-139">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e8666-139">See also</span></span>



[<span data-ttu-id="e8666-140">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="e8666-140">FindConversation operation</span></span>](findconversation-operation.md)


[<span data-ttu-id="e8666-141">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="e8666-141">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

