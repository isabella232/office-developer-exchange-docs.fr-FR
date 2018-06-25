---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: L’élément FoldersToIgnore identifie une liste de dossiers qui sont ignorés lors de l’obtention d’éléments dans une conversation. Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse GetConversationItems.
ms.openlocfilehash: 96c094996c601e685dc1c7e6b869a790ce7d74a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756464"
---
# <a name="folderstoignore"></a><span data-ttu-id="5938b-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="5938b-104">FoldersToIgnore</span></span>

<span data-ttu-id="5938b-105">L’élément **FoldersToIgnore** identifie une liste de dossiers qui sont ignorés lors de l’obtention d’éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="5938b-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="5938b-106">Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="5938b-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="5938b-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="5938b-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5938b-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5938b-108">Attributes and elements</span></span>

<span data-ttu-id="5938b-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5938b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5938b-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5938b-110">Attributes</span></span>

<span data-ttu-id="5938b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5938b-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5938b-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5938b-112">Child elements</span></span>

<span data-ttu-id="5938b-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="5938b-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5938b-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5938b-114">Parent elements</span></span>

[<span data-ttu-id="5938b-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="5938b-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="5938b-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="5938b-116">Remarks</span></span>

<span data-ttu-id="5938b-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5938b-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5938b-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5938b-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5938b-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5938b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5938b-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5938b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5938b-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5938b-121">Schema name</span></span>  <br/> |<span data-ttu-id="5938b-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5938b-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="5938b-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5938b-123">Validation file</span></span>  <br/> |<span data-ttu-id="5938b-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5938b-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5938b-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5938b-125">Can be empty</span></span>  <br/> |<span data-ttu-id="5938b-126">false</span><span class="sxs-lookup"><span data-stu-id="5938b-126">false</span></span>  <br/> |
   

