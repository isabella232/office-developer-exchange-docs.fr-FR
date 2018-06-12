---
title: DestinationFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DestinationFolderId
api_type:
- schema
ms.assetid: 77d2d222-320b-4aab-88e4-934ef177f55c
description: L’élément DestinationFolderId indique le dossier de destination de copie et les actions de déplacement.
ms.openlocfilehash: 5fb6cae7db9cdb09e23b3627e26e695ecf6418f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755906"
---
# <a name="destinationfolderid"></a><span data-ttu-id="93991-103">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="93991-103">DestinationFolderId</span></span>

<span data-ttu-id="93991-104">L’élément **DestinationFolderId** indique le dossier de destination de copie et les actions de déplacement.</span><span class="sxs-lookup"><span data-stu-id="93991-104">The **DestinationFolderId** element indicates the destination folder for copy and move actions.</span></span> 
  
- [<span data-ttu-id="93991-105">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="93991-105">ApplyConversationAction</span></span>](applyconversationaction.md)  
- [<span data-ttu-id="93991-106">ConversationActions</span><span class="sxs-lookup"><span data-stu-id="93991-106">ConversationActions</span></span>](conversationactions.md) 
- [<span data-ttu-id="93991-107">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="93991-107">ConversationAction</span></span>](conversationaction.md)  
- [<span data-ttu-id="93991-108">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="93991-108">DestinationFolderId</span></span>](destinationfolderid.md)
  
```XML
<DestinationFolderId>
   <FolderId/>
</DestinationFolderId>
```

 <span data-ttu-id="93991-109">**TargetFolderIdType**</span><span class="sxs-lookup"><span data-stu-id="93991-109">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93991-110">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="93991-110">Attributes and elements</span></span>

<span data-ttu-id="93991-111">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="93991-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93991-112">Attributs</span><span class="sxs-lookup"><span data-stu-id="93991-112">Attributes</span></span>

<span data-ttu-id="93991-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93991-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93991-114">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="93991-114">Child elements</span></span>

|<span data-ttu-id="93991-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93991-115">**Element**</span></span>|<span data-ttu-id="93991-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="93991-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93991-117">FolderId</span><span class="sxs-lookup"><span data-stu-id="93991-117">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="93991-118">Contient la clé d’identificateur et modification du dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="93991-118">Contains the identifier and change key of the destination folder.</span></span>  <br/> |
|[<span data-ttu-id="93991-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="93991-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="93991-120">Identifie les dossiers qui peuvent être référencés par un nom.</span><span class="sxs-lookup"><span data-stu-id="93991-120">Identifies folders that can be referenced by name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93991-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="93991-121">Parent elements</span></span>

|<span data-ttu-id="93991-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93991-122">**Element**</span></span>|<span data-ttu-id="93991-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="93991-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93991-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="93991-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="93991-125">Contient une seule action à appliquer à une même conversation.</span><span class="sxs-lookup"><span data-stu-id="93991-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="93991-126">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="93991-126">Text value</span></span>

<span data-ttu-id="93991-127">Aucun.</span><span class="sxs-lookup"><span data-stu-id="93991-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="93991-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="93991-128">Remarks</span></span>

<span data-ttu-id="93991-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="93991-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93991-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="93991-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93991-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="93991-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93991-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="93991-132">Schema Name</span></span>  <br/> |<span data-ttu-id="93991-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="93991-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="93991-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="93991-134">Validation File</span></span>  <br/> |<span data-ttu-id="93991-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="93991-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="93991-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="93991-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="93991-137">False</span><span class="sxs-lookup"><span data-stu-id="93991-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93991-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="93991-138">See also</span></span>

- [<span data-ttu-id="93991-139">Opération de ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="93991-139">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)

