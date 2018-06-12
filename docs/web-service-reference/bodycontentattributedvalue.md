---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: L’élément BodyContentAttributedValue Spécifie le contenu du corps d’un élément.
ms.openlocfilehash: f5b8f0a19b77ce550b1d7f1c415cc8ee4340863a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755424"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="4fe21-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4fe21-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="4fe21-104">L’élément **BodyContentAttributedValue** Spécifie le contenu du corps d’un élément.</span><span class="sxs-lookup"><span data-stu-id="4fe21-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="4fe21-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="4fe21-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fe21-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4fe21-106">Attributes and elements</span></span>

<span data-ttu-id="4fe21-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4fe21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe21-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4fe21-108">Attributes</span></span>

<span data-ttu-id="4fe21-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4fe21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fe21-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4fe21-110">Child elements</span></span>

|<span data-ttu-id="4fe21-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4fe21-111">**Element**</span></span>|<span data-ttu-id="4fe21-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4fe21-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe21-113">Valeur (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="4fe21-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="4fe21-114">Spécifie la valeur d’un élément **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="4fe21-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="4fe21-115">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="4fe21-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="4fe21-116">Spécifie un tableau des informations d’attribution pour une ou plusieurs contacts ou les destinataires active directory dans le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="4fe21-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4fe21-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4fe21-117">Parent elements</span></span>

|<span data-ttu-id="4fe21-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4fe21-118">**Element**</span></span>|<span data-ttu-id="4fe21-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="4fe21-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe21-120">Corps</span><span class="sxs-lookup"><span data-stu-id="4fe21-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="4fe21-121">Spécifie un tableau d’éléments **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="4fe21-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4fe21-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="4fe21-122">Remarks</span></span>

<span data-ttu-id="4fe21-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4fe21-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4fe21-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4fe21-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fe21-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4fe21-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe21-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4fe21-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fe21-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4fe21-127">Schema Name</span></span>  <br/> |<span data-ttu-id="4fe21-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="4fe21-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="4fe21-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="4fe21-129">Validation File</span></span>  <br/> |<span data-ttu-id="4fe21-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fe21-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fe21-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4fe21-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4fe21-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4fe21-132">See also</span></span>



- [<span data-ttu-id="4fe21-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe21-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

