---
title: ContextFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContextFolderId
api_type:
- schema
ms.assetid: 48de92aa-e124-42b5-89bc-cdce5e93d78b
description: L’élément ContextFolderId indique le dossier ciblé pour les actions qui utilisent des dossiers. Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible.
ms.openlocfilehash: 60f1eaf3b45eee83632c7da6f453a1d09f54d9fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529258"
---
# <a name="contextfolderid"></a><span data-ttu-id="0aa60-104">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="0aa60-104">ContextFolderId</span></span>

<span data-ttu-id="0aa60-105">L’élément **ContextFolderId** indique le dossier ciblé pour les actions qui utilisent des dossiers.</span><span class="sxs-lookup"><span data-stu-id="0aa60-105">The **ContextFolderId** element indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="0aa60-106">Cet élément doit être présent lors de la copie, la suppression, le mouvement et la définition de l’état de lecture des éléments de conversation dans un dossier cible.</span><span class="sxs-lookup"><span data-stu-id="0aa60-106">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span> 
  
- [<span data-ttu-id="0aa60-107">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0aa60-107">ApplyConversationAction</span></span>](applyconversationaction.md) 
- [<span data-ttu-id="0aa60-108">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="0aa60-108">ConversationActions</span></span>](conversationactions.md)
- [<span data-ttu-id="0aa60-109">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="0aa60-109">ConversationAction</span></span>](conversationaction.md)
- [<span data-ttu-id="0aa60-110">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="0aa60-110">ContextFolderId</span></span>](contextfolderid.md)
  
```XML
<ContextFolderId>
   <FolderId/>
</ContextFolderId>
```

```XML
<ContextFolderId>
   <DistinguishedFolderId/>
</ContextFolderId>
```


<span data-ttu-id="0aa60-111">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="0aa60-111">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0aa60-112">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0aa60-112">Attributes and elements</span></span>

<span data-ttu-id="0aa60-113">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0aa60-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0aa60-114">Attributs</span><span class="sxs-lookup"><span data-stu-id="0aa60-114">Attributes</span></span>

<span data-ttu-id="0aa60-115">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0aa60-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0aa60-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0aa60-116">Child elements</span></span>

|<span data-ttu-id="0aa60-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0aa60-117">**Element**</span></span>|<span data-ttu-id="0aa60-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="0aa60-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa60-119">FolderId</span><span class="sxs-lookup"><span data-stu-id="0aa60-119">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="0aa60-120">Contient l’identificateur et la clé de modification du dossier de contexte.</span><span class="sxs-lookup"><span data-stu-id="0aa60-120">Contains the identifier and change key of the context folder.</span></span>  <br/> |
|[<span data-ttu-id="0aa60-121">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="0aa60-121">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="0aa60-122">Identifie les dossiers qui peuvent être référencés par leur nom.</span><span class="sxs-lookup"><span data-stu-id="0aa60-122">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0aa60-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0aa60-123">Parent elements</span></span>

|<span data-ttu-id="0aa60-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0aa60-124">**Element**</span></span>|<span data-ttu-id="0aa60-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="0aa60-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0aa60-126">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="0aa60-126">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="0aa60-127">Contient une seule action à appliquer à une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="0aa60-127">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0aa60-128">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0aa60-128">Text value</span></span>

<span data-ttu-id="0aa60-129">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0aa60-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0aa60-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="0aa60-130">Remarks</span></span>

<span data-ttu-id="0aa60-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0aa60-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0aa60-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0aa60-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0aa60-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0aa60-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0aa60-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0aa60-134">Schema Name</span></span>  <br/> |<span data-ttu-id="0aa60-135">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0aa60-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="0aa60-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0aa60-136">Validation File</span></span>  <br/> |<span data-ttu-id="0aa60-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0aa60-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0aa60-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0aa60-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="0aa60-139">False</span><span class="sxs-lookup"><span data-stu-id="0aa60-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0aa60-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0aa60-140">See also</span></span>

- [<span data-ttu-id="0aa60-141">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="0aa60-141">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

