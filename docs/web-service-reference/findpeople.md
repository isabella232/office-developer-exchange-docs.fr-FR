---
title: FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 12c70441-77b9-4619-8e66-1b7e3a63ba48
description: 'L’élément FindPeople spécifie un ensemble de données utilisés dans une requête FindPeople. Les données contient zéro ou plusieurs des éléments suivants : une forme personnage (facultative), un affichage de l’élément indexé de page, une restriction (facultative), une restriction d’agrégation (facultative), un ordre de tri (facultatif), un Id du dossier parent et une chaîne de requête (facultative).'
ms.openlocfilehash: 79c8a4324cd217232442b781c33223296d8015e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756415"
---
# <a name="findpeople"></a><span data-ttu-id="ebb0e-104">FindPeople</span><span class="sxs-lookup"><span data-stu-id="ebb0e-104">FindPeople</span></span>

<span data-ttu-id="ebb0e-105">L’élément **FindPeople** spécifie un ensemble de données utilisés dans une requête FindPeople.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-105">The **FindPeople** element specifies a set of data used in a FindPeople request.</span></span> <span data-ttu-id="ebb0e-106">Les données contient zéro ou plusieurs des éléments suivants : une forme personnage (facultative), un affichage de l’élément indexé de page, une restriction (facultative), une restriction d’agrégation (facultative), un ordre de tri (facultatif), un Id du dossier parent et une chaîne de requête (facultative).</span><span class="sxs-lookup"><span data-stu-id="ebb0e-106">The data includes zero or more of the following elements: a persona shape (optional), an indexed page item view, a restriction (optional), an aggregation restriction (optional), a sort order (optional), a parent folder Id, and a query string (optional).</span></span> 
  
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

 <span data-ttu-id="ebb0e-107">**FindPeopleType**</span><span class="sxs-lookup"><span data-stu-id="ebb0e-107">**FindPeopleType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebb0e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebb0e-108">Attributes and elements</span></span>

<span data-ttu-id="ebb0e-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebb0e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebb0e-110">Attributes</span></span>

<span data-ttu-id="ebb0e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebb0e-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebb0e-112">Child elements</span></span>

<span data-ttu-id="ebb0e-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)  |  [ QueryString (QueryStringType)](querystring-querystringtype.md)</span><span class="sxs-lookup"><span data-stu-id="ebb0e-113">[PersonaShape](personashape.md) | [IndexedPageItemView](indexedpageitemview.md) | [Restriction](restriction.md) | [AggregationRestriction](aggregationrestriction.md) | [SortOrder](sortorder.md) | [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) | [QueryString (QueryStringType)](querystring-querystringtype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ebb0e-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebb0e-114">Parent elements</span></span>

<span data-ttu-id="ebb0e-115">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-115">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebb0e-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="ebb0e-116">Remarks</span></span>

<span data-ttu-id="ebb0e-117">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-117">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ebb0e-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ebb0e-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebb0e-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebb0e-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebb0e-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebb0e-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ebb0e-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebb0e-121">Schema name</span></span>  <br/> |<span data-ttu-id="ebb0e-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ebb0e-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ebb0e-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebb0e-123">Validation file</span></span>  <br/> |<span data-ttu-id="ebb0e-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ebb0e-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ebb0e-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebb0e-125">Can be empty</span></span>  <br/> |<span data-ttu-id="ebb0e-126">false</span><span class="sxs-lookup"><span data-stu-id="ebb0e-126">false</span></span>  <br/> |
   

