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
description: L’élément ApplyConversationAction définit une demande pour appliquer des actions à des éléments dans une conversation.
ms.openlocfilehash: 1b672c6e6d2f60e50215417be7100e9cd77e2a58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755297"
---
# <a name="applyconversationaction"></a><span data-ttu-id="29e1d-103">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="29e1d-103">ApplyConversationAction</span></span>

<span data-ttu-id="29e1d-104">L’élément **ApplyConversationAction** définit une demande pour appliquer des actions à des éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="29e1d-104">The **ApplyConversationAction** element defines a request to apply actions to items in a conversation.</span></span> 
  
[<span data-ttu-id="29e1d-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="29e1d-105">ApplyConversationAction</span></span>](applyconversationaction.md)
  
```XML
<ApplyConversationAction>
   <ConversationActions/>
</ApplyConversationAction>
```

 <span data-ttu-id="29e1d-106">**ApplyConversationActionType**</span><span class="sxs-lookup"><span data-stu-id="29e1d-106">**ApplyConversationActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="29e1d-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="29e1d-107">Attributes and elements</span></span>

<span data-ttu-id="29e1d-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="29e1d-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="29e1d-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="29e1d-109">Attributes</span></span>

<span data-ttu-id="29e1d-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="29e1d-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="29e1d-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="29e1d-111">Child elements</span></span>

|<span data-ttu-id="29e1d-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="29e1d-112">**Element**</span></span>|<span data-ttu-id="29e1d-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="29e1d-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="29e1d-114">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="29e1d-114">ConversationActions</span></span>](conversationactions.md) <br/> |<span data-ttu-id="29e1d-115">Contient une collection des conversations et les actions à appliquer à leur.</span><span class="sxs-lookup"><span data-stu-id="29e1d-115">Contains a collection of conversations and the actions to apply to them.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="29e1d-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="29e1d-116">Parent elements</span></span>

<span data-ttu-id="29e1d-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="29e1d-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="29e1d-118">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="29e1d-118">Text value</span></span>

<span data-ttu-id="29e1d-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="29e1d-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="29e1d-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="29e1d-120">Remarks</span></span>

<span data-ttu-id="29e1d-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="29e1d-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="29e1d-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="29e1d-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="29e1d-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="29e1d-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="29e1d-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="29e1d-124">Schema Name</span></span>  <br/> |<span data-ttu-id="29e1d-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="29e1d-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="29e1d-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="29e1d-126">Validation File</span></span>  <br/> |<span data-ttu-id="29e1d-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="29e1d-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="29e1d-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="29e1d-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="29e1d-129">False</span><span class="sxs-lookup"><span data-stu-id="29e1d-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="29e1d-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="29e1d-130">See also</span></span>

- [<span data-ttu-id="29e1d-131">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="29e1d-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="29e1d-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="29e1d-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

