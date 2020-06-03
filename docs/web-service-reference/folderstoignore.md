---
title: FoldersToIgnore
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b5d18516-a617-4daf-8baf-c7ce29c76f6b
description: L’élément FoldersToIgnore identifie une liste de dossiers ignorés lors de l’obtention d’éléments dans une conversation. Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse GetConversationItems.
ms.openlocfilehash: 07813a54a9a3afa3de23ae94f1c9b191d1cb6fac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44453356"
---
# <a name="folderstoignore"></a><span data-ttu-id="23e76-104">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="23e76-104">FoldersToIgnore</span></span>

<span data-ttu-id="23e76-105">L’élément **FoldersToIgnore** identifie une liste de dossiers ignorés lors de l’obtention d’éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="23e76-105">The **FoldersToIgnore** element identifies a list of folders that are ignored when getting items in a conversation.</span></span> <span data-ttu-id="23e76-106">Tous les éléments de conversation dans les dossiers ignorés ne sont pas renvoyés dans une réponse **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="23e76-106">All conversation items in the ignored folders are not returned in a **GetConversationItems** response.</span></span> 
  
```XML
<FoldersToIgnore>
   <FolderId/>
   <DistinguishedFolderId/>
</FoldersToIgnore>
```

 <span data-ttu-id="23e76-107">**NonEmptyArrayOfBaseFolderIdsType**</span><span class="sxs-lookup"><span data-stu-id="23e76-107">**NonEmptyArrayOfBaseFolderIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23e76-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="23e76-108">Attributes and elements</span></span>

<span data-ttu-id="23e76-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="23e76-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23e76-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="23e76-110">Attributes</span></span>

<span data-ttu-id="23e76-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="23e76-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23e76-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="23e76-112">Child elements</span></span>

<span data-ttu-id="23e76-113">[FolderId](folderid.md)  |  [DistinguishedFolderId](distinguishedfolderid.md)</span><span class="sxs-lookup"><span data-stu-id="23e76-113">[FolderId](folderid.md) | [DistinguishedFolderId](distinguishedfolderid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="23e76-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="23e76-114">Parent elements</span></span>

[<span data-ttu-id="23e76-115">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="23e76-115">GetConversationItems</span></span>](getconversationitems.md)
  
## <a name="remarks"></a><span data-ttu-id="23e76-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="23e76-116">Remarks</span></span>

<span data-ttu-id="23e76-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="23e76-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="23e76-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="23e76-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23e76-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="23e76-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23e76-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="23e76-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="23e76-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="23e76-121">Schema name</span></span>  <br/> |<span data-ttu-id="23e76-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="23e76-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="23e76-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="23e76-123">Validation file</span></span>  <br/> |<span data-ttu-id="23e76-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="23e76-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="23e76-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="23e76-125">Can be empty</span></span>  <br/> |<span data-ttu-id="23e76-126">false</span><span class="sxs-lookup"><span data-stu-id="23e76-126">false</span></span>  <br/> |
   

