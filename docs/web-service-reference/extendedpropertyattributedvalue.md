---
title: ExtendedPropertyAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90f3c5c5-f612-4e1b-b1f5-f92dd8524179
description: L’élément ExtendedPropertyAttributedValue spécifie les propriétés étendues d’un personnage.
ms.openlocfilehash: 5c2ad5918d7ac666d5e26af6597b2c4c3dde6202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460126"
---
# <a name="extendedpropertyattributedvalue"></a><span data-ttu-id="36dda-103">ExtendedPropertyAttributedValue</span><span class="sxs-lookup"><span data-stu-id="36dda-103">ExtendedPropertyAttributedValue</span></span>

<span data-ttu-id="36dda-104">L’élément **ExtendedPropertyAttributedValue** spécifie les propriétés étendues d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="36dda-104">The **ExtendedPropertyAttributedValue** element specifies extended properties for a persona.</span></span> 
  
```XML
<ExtendedPropertyAttributedValue>
    <Value/>
    <Attributions/>
</ExtendedPropertyAttributedValue>
```

 <span data-ttu-id="36dda-105">**ExtendedPropertyAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="36dda-105">**ExtendedPropertyAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36dda-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="36dda-106">Attributes and elements</span></span>

<span data-ttu-id="36dda-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="36dda-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36dda-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="36dda-108">Attributes</span></span>

<span data-ttu-id="36dda-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="36dda-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="36dda-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="36dda-110">Child elements</span></span>

|<span data-ttu-id="36dda-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36dda-111">**Element**</span></span>|<span data-ttu-id="36dda-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="36dda-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36dda-113">Valeur (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="36dda-113">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md) <br/> |<span data-ttu-id="36dda-114">Spécifie un tableau de propriétés étendues pour un personnage.</span><span class="sxs-lookup"><span data-stu-id="36dda-114">Specifies an array of extended properties for a persona.</span></span>  <br/> |
|[<span data-ttu-id="36dda-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="36dda-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="36dda-116">Spécifie un tableau des attributions de l’élément **value** associé.</span><span class="sxs-lookup"><span data-stu-id="36dda-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="36dda-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="36dda-117">Parent elements</span></span>

|<span data-ttu-id="36dda-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="36dda-118">**Element**</span></span>|<span data-ttu-id="36dda-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="36dda-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36dda-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span><span class="sxs-lookup"><span data-stu-id="36dda-120">ExtendedProperties (ArrayOfExtendedPropertyAttributedValueType)</span></span>](extendedproperties-arrayofextendedpropertyattributedvaluetype.md) <br/> |<span data-ttu-id="36dda-121">Contient les propriétés étendues utilisées pour les opérations du magasin de contacts unifié.</span><span class="sxs-lookup"><span data-stu-id="36dda-121">Contains the extended properties used for Unified Contact Store operations.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36dda-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="36dda-122">Remarks</span></span>

<span data-ttu-id="36dda-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="36dda-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="36dda-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="36dda-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="36dda-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="36dda-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36dda-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="36dda-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="36dda-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="36dda-127">Schema Name</span></span>  <br/> |<span data-ttu-id="36dda-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="36dda-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="36dda-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="36dda-129">Validation File</span></span>  <br/> |<span data-ttu-id="36dda-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="36dda-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="36dda-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="36dda-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="36dda-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="36dda-132">See also</span></span>



- [<span data-ttu-id="36dda-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="36dda-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

