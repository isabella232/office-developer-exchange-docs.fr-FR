---
title: DeleteType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteType
api_type:
- schema
ms.assetid: 6e3136cd-9cb4-493a-aa85-9678f719002d
description: L’élément DeleteType indique le mode de suppression des éléments d’une conversation.
ms.openlocfilehash: 199f7afc29fe866865509d2fb90d24944113d5c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442632"
---
# <a name="deletetype"></a><span data-ttu-id="f85e8-103">DeleteType</span><span class="sxs-lookup"><span data-stu-id="f85e8-103">DeleteType</span></span>

<span data-ttu-id="f85e8-104">L’élément **DeleteType** indique le mode de suppression des éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="f85e8-104">The **DeleteType** element indicates how items in a conversation are deleted.</span></span> 
  
- [<span data-ttu-id="f85e8-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f85e8-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="f85e8-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="f85e8-106">ConversationActions</span></span>](conversationactions.md)  
- [<span data-ttu-id="f85e8-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f85e8-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="f85e8-108">DeleteType</span><span class="sxs-lookup"><span data-stu-id="f85e8-108">DeleteType</span></span>](deletetype.md)
  
```XML
<DeleteType> HardDelete | MoveToDeletedItems | SoftDelete </DeleteType>
```

 <span data-ttu-id="f85e8-109">**DisposalType**</span><span class="sxs-lookup"><span data-stu-id="f85e8-109">**DisposalType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f85e8-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f85e8-110">Attributes and elements</span></span>

<span data-ttu-id="f85e8-111">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f85e8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f85e8-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="f85e8-112">Attributes</span></span>

<span data-ttu-id="f85e8-113">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f85e8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f85e8-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f85e8-114">Child elements</span></span>

<span data-ttu-id="f85e8-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f85e8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f85e8-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f85e8-116">Parent elements</span></span>

|<span data-ttu-id="f85e8-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f85e8-117">**Element**</span></span>|<span data-ttu-id="f85e8-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="f85e8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f85e8-119">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="f85e8-119">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="f85e8-120">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="f85e8-120">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f85e8-121">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f85e8-121">Text value</span></span>

<span data-ttu-id="f85e8-122">La valeur de texte de l’élément **DeleteType** indique le mode de suppression des éléments d’une conversation.</span><span class="sxs-lookup"><span data-stu-id="f85e8-122">The text value of the **DeleteType** element indicates how items in a conversation are deleted.</span></span> <span data-ttu-id="f85e8-123">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="f85e8-123">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="f85e8-124">HardDelete : indique que les éléments d’une conversation sont définitivement supprimés de la base de données de boîtes aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f85e8-124">HardDelete - Indicates that items in a conversation are permanently removed from the mailbox database.</span></span>
    
- <span data-ttu-id="f85e8-125">MoveToDeleteItems : indique que les éléments d’une conversation sont déplacés vers le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="f85e8-125">MoveToDeleteItems - Indicates that items in a conversation are moved to the Deleted Items folder.</span></span>
    
- <span data-ttu-id="f85e8-126">SoftDelete : indique que les éléments d’une conversation sont déplacés vers la benne si la benne est activée.</span><span class="sxs-lookup"><span data-stu-id="f85e8-126">SoftDelete - Indicates that items in a conversation are moved to the dumpster if the dumpster is enabled.</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f85e8-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="f85e8-127">Remarks</span></span>

<span data-ttu-id="f85e8-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f85e8-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f85e8-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f85e8-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f85e8-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f85e8-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f85e8-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f85e8-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f85e8-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f85e8-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="f85e8-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f85e8-133">Validation File</span></span>  <br/> |<span data-ttu-id="f85e8-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f85e8-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f85e8-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f85e8-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="f85e8-136">False</span><span class="sxs-lookup"><span data-stu-id="f85e8-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f85e8-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f85e8-137">See also</span></span>

- [<span data-ttu-id="f85e8-138">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f85e8-138">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="f85e8-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f85e8-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

