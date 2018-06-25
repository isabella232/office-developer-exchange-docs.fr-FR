---
title: IsHidden
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2377b584-bd1e-49fc-b80a-a6634721a297
description: L’élément IsHidden contient une valeur de type Boolean qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.
ms.openlocfilehash: ee20bf0af287e3cddaedb5bc6d3c63ef9a7a7006
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828032"
---
# <a name="ishidden"></a><span data-ttu-id="b35e6-103">IsHidden</span><span class="sxs-lookup"><span data-stu-id="b35e6-103">IsHidden</span></span>

<span data-ttu-id="b35e6-104">L’élément **IsHidden** contient une valeur de type Boolean qui indique si le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="b35e6-104">The **IsHidden** element contains a Boolean value that indicates whether the underlying contact should be hidden or displayed as part of the persona.</span></span> 
  
```XML
<IsHidden>true | false</IsHidden>
```

 <span data-ttu-id="b35e6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="b35e6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b35e6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b35e6-106">Attributes and elements</span></span>

<span data-ttu-id="b35e6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b35e6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b35e6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b35e6-108">Attributes</span></span>

<span data-ttu-id="b35e6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b35e6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b35e6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b35e6-110">Child elements</span></span>

<span data-ttu-id="b35e6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b35e6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b35e6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b35e6-112">Parent elements</span></span>

|<span data-ttu-id="b35e6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b35e6-113">**Element**</span></span>|<span data-ttu-id="b35e6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="b35e6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b35e6-115">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="b35e6-115">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="b35e6-116">Spécifie une instance d'un tableau d'attributs pour un élément **Persona**.</span><span class="sxs-lookup"><span data-stu-id="b35e6-116">Specifies an instance in an array of attributes for a **Persona** element.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b35e6-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="b35e6-117">Text value</span></span>

<span data-ttu-id="b35e6-118">Une valeur de texte de **la valeur true** pour l’élément **IsHidden** indique que le contact sous-jacent doit être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="b35e6-118">A text value of **true** for the **IsHidden** element indicates that the underlying contact should be hidden or displayed as part of the persona.</span></span> <span data-ttu-id="b35e6-119">La valeur **false** indique que le contact sous-jacent ne doit pas être masqué ou affiché dans le cadre du personnage.</span><span class="sxs-lookup"><span data-stu-id="b35e6-119">A value of **false** indicates that the underlying contact should not be hidden or displayed as part of the persona.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b35e6-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="b35e6-120">Remarks</span></span>

<span data-ttu-id="b35e6-121">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b35e6-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b35e6-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b35e6-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b35e6-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b35e6-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b35e6-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b35e6-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b35e6-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b35e6-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b35e6-126">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b35e6-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b35e6-127">Validation File</span><span class="sxs-lookup"><span data-stu-id="b35e6-127">Validation File</span></span>  <br/> |<span data-ttu-id="b35e6-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b35e6-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b35e6-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b35e6-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b35e6-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b35e6-130">See also</span></span>



- [<span data-ttu-id="b35e6-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b35e6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

