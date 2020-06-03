---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'L’élément FindPeople spécifie un ensemble de données utilisé dans une demande FindPeople. Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), une vue d’élément de page indexée, une restriction (facultative), une restriction d’agrégation (facultatif), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultatif).'
ms.openlocfilehash: 4777601b7146ec857b5c79fa9d4ced59a7247889
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462900"
---
# <a name="findpeople"></a><span data-ttu-id="ff6d2-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="ff6d2-104">FindPeople</span></span>

<span data-ttu-id="ff6d2-105">L’élément **FindPeople** spécifie un ensemble de données utilisé dans une demande FindPeople.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="ff6d2-106">Les données incluent zéro ou plusieurs des éléments suivants : une forme de personnage (facultatif), une vue d’élément de page indexée, une restriction (facultative), une restriction d’agrégation (facultatif), un ordre de tri (facultatif), un ID de dossier parent et une chaîne de requête (facultatif).</span><span class="sxs-lookup"><span data-stu-id="ff6d2-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
```XML
<FindPeople>
   <PersonaShape/>
   <IndexedPageItemView/>
   <Restriction/>
   <AggregationRestriction/>
   <SortOrder/>
   <ParentFolderId/>
   <QueryString/>
</FindPeople>
```

 <span data-ttu-id="ff6d2-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="ff6d2-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff6d2-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff6d2-108">Attributes and elements</span></span>

<span data-ttu-id="ff6d2-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff6d2-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff6d2-110">Attributes</span></span>

<span data-ttu-id="ff6d2-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff6d2-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff6d2-112">Child elements</span></span>

<span data-ttu-id="ff6d2-113">[PersonaShape](personashape.md)  |  [IndexedPageItemView](indexedpageitemview.md)  |  [Restriction](restriction.md)  |  [AggregationRestriction](aggregationrestriction.md)  |  [OrdreTri (SortOrder](sortorder.md)  |  ) [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [QueryString (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="ff6d2-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff6d2-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff6d2-114">Parent elements</span></span>

<span data-ttu-id="ff6d2-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff6d2-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="ff6d2-116">Remarks</span></span>

<span data-ttu-id="ff6d2-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ff6d2-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff6d2-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff6d2-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff6d2-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff6d2-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff6d2-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ff6d2-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff6d2-121">Schema name</span></span>  <br/> |<span data-ttu-id="ff6d2-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ff6d2-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ff6d2-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ff6d2-123">Validation file</span></span>  <br/> |<span data-ttu-id="ff6d2-124">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff6d2-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff6d2-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff6d2-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ff6d2-126">false</span><span class="sxs-lookup"><span data-stu-id="ff6d2-126">false</span></span>  <br/> |
   

