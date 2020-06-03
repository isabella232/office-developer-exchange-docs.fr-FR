---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: L’élément IsHidden contient une valeur booléenne qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.
ms.openlocfilehash: a22628e9ab4a46de04fe395f2d6c1b70083a5c77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464237"
---
# <a name="ishidden"></a><span data-ttu-id="9b55c-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="9b55c-103">IsHidden</span></span>

<span data-ttu-id="9b55c-104">L’élément **IsHidden** contient une valeur booléenne qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="9b55c-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="9b55c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9b55c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9b55c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="9b55c-106">Attributes and elements</span></span>

<span data-ttu-id="9b55c-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="9b55c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9b55c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="9b55c-108">Attributes</span></span>

<span data-ttu-id="9b55c-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="9b55c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9b55c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="9b55c-110">Child elements</span></span>

<span data-ttu-id="9b55c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="9b55c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9b55c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="9b55c-112">Parent elements</span></span>

|<span data-ttu-id="9b55c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="9b55c-113">**Element**</span></span>|<span data-ttu-id="9b55c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="9b55c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9b55c-115">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="9b55c-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="9b55c-116">Spécifie une instance d'un tableau d'attributs pour un élément **Persona**.</span><span class="sxs-lookup"><span data-stu-id="9b55c-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9b55c-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="9b55c-117">Text value</span></span>

<span data-ttu-id="9b55c-118">Une valeur de texte de **true** pour l’élément **IsHidden** indique que le contact sous-jacent doit être masqué ou affiché en tant que partie du personnage.</span><span class="sxs-lookup"><span data-stu-id="9b55c-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="9b55c-119">La valeur **false** indique que le contact sous-jacent ne doit pas être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="9b55c-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9b55c-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="9b55c-120">Remarks</span></span>

<span data-ttu-id="9b55c-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9b55c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9b55c-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="9b55c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9b55c-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="9b55c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9b55c-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="9b55c-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9b55c-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="9b55c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="9b55c-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="9b55c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="9b55c-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="9b55c-127">Validation File</span></span>  <br/> |<span data-ttu-id="9b55c-128">types. xsd</span><span class="sxs-lookup"><span data-stu-id="9b55c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9b55c-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="9b55c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9b55c-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="9b55c-130">See also</span></span>



- [<span data-ttu-id="9b55c-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="9b55c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

