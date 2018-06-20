---
title: ProcessRightAway
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ProcessRightAway
api_type:
- schema
ms.assetid: f6bba68b-ae4f-41c1-b3e7-c8a31cdb1b0c
description: L’élément ProcessRightAway indique si la réponse est envoyée dès que l’action démarre le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée. Cet élément doit être présent pour la réponse à envoyer asynchrone à l’action demandée.
ms.openlocfilehash: 940f8e8fa0a53801ce1c3a45c3aecf1bdb6f519d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828898"
---
# <a name="processrightaway"></a><span data-ttu-id="42e2e-104">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="42e2e-104">ProcessRightAway</span></span>

<span data-ttu-id="42e2e-105">L’élément **ProcessRightAway** indique si la réponse est envoyée dès que l’action démarre le traitement sur le serveur ou si la réponse est envoyée une fois l’action terminée.</span><span class="sxs-lookup"><span data-stu-id="42e2e-105">The **ProcessRightAway** element indicates whether the response is sent as soon as the action starts processing on the server or whether the response is sent after the action has completed.</span></span> <span data-ttu-id="42e2e-106">Cet élément doit être présent pour la réponse à envoyer asynchrone à l’action demandée.</span><span class="sxs-lookup"><span data-stu-id="42e2e-106">This element must be present for the response to be sent asynchronous to the requested action.</span></span> 
  
[<span data-ttu-id="42e2e-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="42e2e-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="42e2e-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="42e2e-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="42e2e-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="42e2e-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="42e2e-110">ProcessRightAway</span><span class="sxs-lookup"><span data-stu-id="42e2e-110">ProcessRightAway</span></span>](processrightaway.md)
  
```XML
<ProcessRightAway/>
```

 <span data-ttu-id="42e2e-111">**xs : Boolean**</span><span class="sxs-lookup"><span data-stu-id="42e2e-111">**xs:boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42e2e-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="42e2e-112">Attributes and elements</span></span>

<span data-ttu-id="42e2e-113">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="42e2e-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42e2e-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="42e2e-114">Attributes</span></span>

<span data-ttu-id="42e2e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="42e2e-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="42e2e-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="42e2e-116">Child elements</span></span>

<span data-ttu-id="42e2e-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="42e2e-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42e2e-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="42e2e-118">Parent elements</span></span>

|<span data-ttu-id="42e2e-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="42e2e-119">**Element**</span></span>|<span data-ttu-id="42e2e-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="42e2e-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="42e2e-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="42e2e-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="42e2e-122">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="42e2e-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="42e2e-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="42e2e-123">Text value</span></span>

<span data-ttu-id="42e2e-124">Une valeur de texte de **la valeur true** indique que la réponse est envoyée dès que l’action lance le traitement sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="42e2e-124">A text value of **true** indicates that the response is sent as soon as the action starts processing on the server.</span></span> <span data-ttu-id="42e2e-125">Texte la valeur **false** indique que la réponse est envoyée une fois l’action terminée.</span><span class="sxs-lookup"><span data-stu-id="42e2e-125">A text value of **false** indicates that the response is sent after the action has completed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="42e2e-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="42e2e-126">Remarks</span></span>

<span data-ttu-id="42e2e-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="42e2e-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42e2e-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="42e2e-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42e2e-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="42e2e-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42e2e-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="42e2e-130">Schema Name</span></span>  <br/> |<span data-ttu-id="42e2e-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="42e2e-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="42e2e-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="42e2e-132">Validation File</span></span>  <br/> |<span data-ttu-id="42e2e-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42e2e-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42e2e-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="42e2e-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="42e2e-135">False</span><span class="sxs-lookup"><span data-stu-id="42e2e-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="42e2e-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="42e2e-136">See also</span></span>



[<span data-ttu-id="42e2e-137">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="42e2e-137">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="42e2e-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="42e2e-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

