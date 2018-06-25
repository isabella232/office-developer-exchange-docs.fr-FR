---
title: UnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnreadCount
api_type:
- schema
ms.assetid: 53b22647-1453-4707-9ea0-6a8369748d56
description: L’élément UnreadCount indique le nombre d’éléments non lus dans un dossier.
ms.openlocfilehash: fbe887f8f6d83fbcf48ed9593b3d19322a7f48be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838838"
---
# <a name="unreadcount"></a><span data-ttu-id="cd009-103">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="cd009-103">UnreadCount</span></span>

<span data-ttu-id="cd009-104">L’élément **UnreadCount** indique le nombre d’éléments non lus dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="cd009-104">The **UnreadCount** element contains the count of unread items within a folder.</span></span> 
  
```XML
<UnreadCount/>
```

 <span data-ttu-id="cd009-105">**xs : int**</span><span class="sxs-lookup"><span data-stu-id="cd009-105">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd009-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cd009-106">Attributes and elements</span></span>

<span data-ttu-id="cd009-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cd009-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd009-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cd009-108">Attributes</span></span>

<span data-ttu-id="cd009-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cd009-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd009-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cd009-110">Child elements</span></span>

<span data-ttu-id="cd009-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cd009-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd009-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cd009-112">Parent elements</span></span>

|<span data-ttu-id="cd009-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cd009-113">**Element**</span></span>|<span data-ttu-id="cd009-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cd009-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd009-115">Conversation (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="cd009-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="cd009-116">Représente une conversation unique.</span><span class="sxs-lookup"><span data-stu-id="cd009-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="cd009-117">Folder</span><span class="sxs-lookup"><span data-stu-id="cd009-117">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="cd009-118">Représente un dossier dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cd009-118">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cd009-119">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="cd009-119">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="cd009-120">Représente un événement où un élément ou un dossier est modifié.</span><span class="sxs-lookup"><span data-stu-id="cd009-120">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="cd009-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="cd009-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="cd009-122">Représente un dossier de recherche dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cd009-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="cd009-123">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="cd009-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="cd009-124">Représente un dossier de tâches dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cd009-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cd009-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cd009-125">Text value</span></span>

<span data-ttu-id="cd009-126">La valeur de texte représente une valeur entière.</span><span class="sxs-lookup"><span data-stu-id="cd009-126">The text value represents an integer value.</span></span> <span data-ttu-id="cd009-127">Cette propriété est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="cd009-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cd009-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="cd009-128">Remarks</span></span>

<span data-ttu-id="cd009-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd009-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd009-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cd009-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd009-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cd009-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd009-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cd009-132">Schema Name</span></span>  <br/> |<span data-ttu-id="cd009-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="cd009-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd009-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cd009-134">Validation File</span></span>  <br/> |<span data-ttu-id="cd009-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cd009-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd009-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cd009-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd009-137">False</span><span class="sxs-lookup"><span data-stu-id="cd009-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd009-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cd009-138">See also</span></span>



- [<span data-ttu-id="cd009-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cd009-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

