---
title: BodyContentAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f99e9590-8388-4203-ac30-1ea394f351a6
description: L’élément BodyContentAttributedValue spécifie le contenu du corps d’un élément.
ms.openlocfilehash: 3550d9307e9bd652afc217f72610379a0a5b2f68
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527396"
---
# <a name="bodycontentattributedvalue"></a><span data-ttu-id="3f36a-103">BodyContentAttributedValue</span><span class="sxs-lookup"><span data-stu-id="3f36a-103">BodyContentAttributedValue</span></span>

<span data-ttu-id="3f36a-104">L’élément **BodyContentAttributedValue** spécifie le contenu du corps d’un élément.</span><span class="sxs-lookup"><span data-stu-id="3f36a-104">The **BodyContentAttributedValue** element specifies the body content of an item.</span></span> 
  
```XML
<BodyContentAttributedValue>
   <Value></Value>
   <Attributions></Attributions>
</ BodyContentAttributedValue>
```

 <span data-ttu-id="3f36a-105">**BodyContentAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="3f36a-105">**BodyContentAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f36a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3f36a-106">Attributes and elements</span></span>

<span data-ttu-id="3f36a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3f36a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f36a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3f36a-108">Attributes</span></span>

<span data-ttu-id="3f36a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3f36a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f36a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3f36a-110">Child elements</span></span>

|<span data-ttu-id="3f36a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f36a-111">**Element**</span></span>|<span data-ttu-id="3f36a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f36a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f36a-113">Valeur (BodyContentType)</span><span class="sxs-lookup"><span data-stu-id="3f36a-113">Value (BodyContentType)</span></span>](value-bodycontenttype.md) <br/> |<span data-ttu-id="3f36a-114">Spécifie la valeur d’un élément **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="3f36a-114">Specifies the value of a **BodyContentAttributedValue** element.</span></span>  <br/> |
|[<span data-ttu-id="3f36a-115">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="3f36a-115">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="3f36a-116">Spécifie un tableau d’informations d’attribution pour un ou plusieurs contacts ou destinataires Active Directory agrégés dans le personnage associé.</span><span class="sxs-lookup"><span data-stu-id="3f36a-116">Specifies an array of attribution information for one or more of the contacts or active directory recipients aggregated into the associated persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3f36a-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3f36a-117">Parent elements</span></span>

|<span data-ttu-id="3f36a-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3f36a-118">**Element**</span></span>|<span data-ttu-id="3f36a-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="3f36a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f36a-120">Compétent</span><span class="sxs-lookup"><span data-stu-id="3f36a-120">Bodies</span></span>](bodies.md) <br/> |<span data-ttu-id="3f36a-121">Spécifie un tableau d’éléments **BodyContentAttributedValue** .</span><span class="sxs-lookup"><span data-stu-id="3f36a-121">Specifies an array of **BodyContentAttributedValue** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3f36a-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="3f36a-122">Remarks</span></span>

<span data-ttu-id="3f36a-123">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3f36a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3f36a-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3f36a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f36a-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3f36a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f36a-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3f36a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f36a-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3f36a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3f36a-128">Schéma type</span><span class="sxs-lookup"><span data-stu-id="3f36a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3f36a-129">Validation File</span><span class="sxs-lookup"><span data-stu-id="3f36a-129">Validation File</span></span>  <br/> |<span data-ttu-id="3f36a-130">types. xsd</span><span class="sxs-lookup"><span data-stu-id="3f36a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f36a-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3f36a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3f36a-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3f36a-132">See also</span></span>



- [<span data-ttu-id="3f36a-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3f36a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

