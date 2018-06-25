---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: L’élément ExtendedPropertyAttributedValue spécifie les propriétés étendues pour un personnage.
ms.openlocfilehash: 92e4ec7f192ccb36ea68d7862e66cb7b3349819a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756295"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="c884f-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="c884f-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="c884f-104">L’élément **ExtendedPropertyAttributedValue** spécifie les propriétés étendues pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="c884f-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="c884f-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="c884f-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c884f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c884f-106">Attributes and elements</span></span>

<span data-ttu-id="c884f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c884f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c884f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c884f-108">Attributes</span></span>

<span data-ttu-id="c884f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c884f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c884f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c884f-110">Child elements</span></span>

|<span data-ttu-id="c884f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c884f-111">**Element**</span></span>|<span data-ttu-id="c884f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c884f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c884f-113">Valeur (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="c884f-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="c884f-114">Spécifie un tableau de propriétés étendues pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="c884f-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="c884f-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="c884f-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="c884f-116">Spécifie un tableau des affectations pour sa **valeur** de l’élément associé.</span><span class="sxs-lookup"><span data-stu-id="c884f-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c884f-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c884f-117">Parent elements</span></span>

|<span data-ttu-id="c884f-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c884f-118">**Element**</span></span>|<span data-ttu-id="c884f-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="c884f-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c884f-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="c884f-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="c884f-121">Contient les propriétés étendues utilisées pour les opérations de magasin de contacts unifié.</span><span class="sxs-lookup"><span data-stu-id="c884f-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c884f-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c884f-122">Remarks</span></span>

<span data-ttu-id="c884f-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c884f-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c884f-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c884f-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c884f-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c884f-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c884f-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c884f-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c884f-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c884f-127">Schema Name</span></span>  <br/> |<span data-ttu-id="c884f-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="c884f-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="c884f-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="c884f-129">Validation File</span></span>  <br/> |<span data-ttu-id="c884f-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="c884f-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="c884f-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c884f-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="c884f-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c884f-132">See also</span></span>



- [<span data-ttu-id="c884f-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c884f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

