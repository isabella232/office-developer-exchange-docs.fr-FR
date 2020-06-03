---
title: ConversationLastSyncTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationLastSyncTime
api_type:
- schema
ms.assetid: 90f8f9e3-5fc6-4a6a-bdfb-fc91fa51f8a2
description: L’élément ConversationLastSyncTime contient la date et l’heure de la dernière synchronisation d’une conversation. Cet élément doit être présent lors de la tentative de suppression de tous les éléments d’une conversation qui ont été reçus pendant la durée spécifiée.
ms.openlocfilehash: f7cc6e205ab9936685d7b8c1f34129b799a53021
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461428"
---
# <a name="conversationlastsynctime"></a><span data-ttu-id="8f559-104">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="8f559-104">ConversationLastSyncTime</span></span>

<span data-ttu-id="8f559-105">L’élément **ConversationLastSyncTime** contient la date et l’heure de la dernière synchronisation d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="8f559-105">The **ConversationLastSyncTime** element contains the date and time that a conversation was last synchronized.</span></span> <span data-ttu-id="8f559-106">Cet élément doit être présent lors de la tentative de suppression de tous les éléments d’une conversation qui ont été reçus pendant la durée spécifiée.</span><span class="sxs-lookup"><span data-stu-id="8f559-106">This element must be present when trying to delete all items in a conversation that were received up to the specified time.</span></span> 
  
[<span data-ttu-id="8f559-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f559-107">ApplyConversationAction</span></span>](applyconversationaction.md)
  
[<span data-ttu-id="8f559-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="8f559-108">ConversationActions</span></span>](conversationactions.md)
  
[<span data-ttu-id="8f559-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f559-109">ConversationAction</span></span>](conversationaction.md)
  
[<span data-ttu-id="8f559-110">ConversationLastSyncTime</span><span class="sxs-lookup"><span data-stu-id="8f559-110">ConversationLastSyncTime</span></span>](conversationlastsynctime.md)
  
```XML
<ConversationLastSyncTime/>
```

 <span data-ttu-id="8f559-111">**XS : dateTime**</span><span class="sxs-lookup"><span data-stu-id="8f559-111">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f559-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8f559-112">Attributes and elements</span></span>

<span data-ttu-id="8f559-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8f559-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f559-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="8f559-114">Attributes</span></span>

<span data-ttu-id="8f559-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8f559-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f559-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8f559-116">Child elements</span></span>

<span data-ttu-id="8f559-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8f559-117">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8f559-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8f559-118">Parent elements</span></span>

|<span data-ttu-id="8f559-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8f559-119">**Element**</span></span>|<span data-ttu-id="8f559-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="8f559-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f559-121">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f559-121">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="8f559-122">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="8f559-122">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f559-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8f559-123">Text value</span></span>

<span data-ttu-id="8f559-124">La valeur de texte du **ConversationLastSyncTime** indique la date de la dernière synchronisation de la conversation.</span><span class="sxs-lookup"><span data-stu-id="8f559-124">The text value of the **ConversationLastSyncTime** indicates the last time the conversation was synchronized.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8f559-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="8f559-125">Remarks</span></span>

<span data-ttu-id="8f559-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8f559-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f559-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8f559-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f559-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8f559-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f559-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8f559-129">Schema Name</span></span>  <br/> |<span data-ttu-id="8f559-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8f559-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f559-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8f559-131">Validation File</span></span>  <br/> |<span data-ttu-id="8f559-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f559-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f559-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8f559-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f559-134">False</span><span class="sxs-lookup"><span data-stu-id="8f559-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f559-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8f559-135">See also</span></span>



[<span data-ttu-id="8f559-136">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="8f559-136">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="8f559-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8f559-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

