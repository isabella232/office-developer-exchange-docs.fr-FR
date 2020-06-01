---
title: ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: e0ee8f30-529b-4d87-8bc0-b6616e75fb6b
description: L’élément ApplyConversationAction définit une demande d’application d’actions à des éléments d’une conversation.
ms.openlocfilehash: 659b3392778bb1a318c3942a0c8e314f12110c12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461687"
---
# <a name="applyconversationaction"></a><span data-ttu-id="89812-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="89812-103">ApplyConversationAction</span></span>

<span data-ttu-id="89812-104">L’élément **ApplyConversationAction** définit une demande d’application d’actions à des éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="89812-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="89812-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="89812-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="89812-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="89812-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89812-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="89812-107">Attributes and elements</span></span>

<span data-ttu-id="89812-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="89812-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89812-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="89812-109">Attributes</span></span>

<span data-ttu-id="89812-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="89812-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89812-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="89812-111">Child elements</span></span>

|<span data-ttu-id="89812-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="89812-112">**Element**</span></span>|<span data-ttu-id="89812-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="89812-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89812-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="89812-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="89812-115">Contient une collection de conversations et les actions à leur appliquer.</span><span class="sxs-lookup"><span data-stu-id="89812-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89812-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="89812-116">Parent elements</span></span>

<span data-ttu-id="89812-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89812-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="89812-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="89812-118">Text value</span></span>

<span data-ttu-id="89812-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="89812-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89812-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="89812-120">Remarks</span></span>

<span data-ttu-id="89812-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="89812-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89812-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="89812-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89812-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="89812-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89812-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="89812-124">Schema Name</span></span>  <br/> |<span data-ttu-id="89812-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="89812-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89812-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="89812-126">Validation File</span></span>  <br/> |<span data-ttu-id="89812-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="89812-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89812-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="89812-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="89812-129">False</span><span class="sxs-lookup"><span data-stu-id="89812-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89812-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="89812-130">See also</span></span>

- [<span data-ttu-id="89812-131">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="89812-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="89812-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="89812-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

