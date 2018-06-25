---
title: Constante
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: L’élément constante identifie une constante dans une restriction.
ms.openlocfilehash: 73912bc1981c5d54040f7c4a563ad805916fe721
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755547"
---
# <a name="constant"></a><span data-ttu-id="6f0bf-103">Constante</span><span class="sxs-lookup"><span data-stu-id="6f0bf-103">Constant</span></span>

<span data-ttu-id="6f0bf-104">L’élément **constante** identifie une constante dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="6f0bf-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6f0bf-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6f0bf-106">Attributes and elements</span></span>

<span data-ttu-id="6f0bf-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6f0bf-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6f0bf-108">Attributes</span></span>

|<span data-ttu-id="6f0bf-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-109">**Attribute**</span></span>|<span data-ttu-id="6f0bf-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6f0bf-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-111">**Value**</span></span> <br/> |<span data-ttu-id="6f0bf-112">Spécifie la valeur à comparer dans la restriction.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6f0bf-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6f0bf-113">Child elements</span></span>

<span data-ttu-id="6f0bf-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6f0bf-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6f0bf-115">Parent elements</span></span>

|<span data-ttu-id="6f0bf-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-116">**Element**</span></span>|<span data-ttu-id="6f0bf-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="6f0bf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6f0bf-118">Contient</span><span class="sxs-lookup"><span data-stu-id="6f0bf-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="6f0bf-119">Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne constante fournie.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="6f0bf-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="6f0bf-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="6f0bf-121">Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6f0bf-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="6f0bf-122">Remarks</span></span>

<span data-ttu-id="6f0bf-123">La valeur de chaîne dans l’attribut **Value** doit être convertie dans le type que vous essayez de comparer.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="6f0bf-124">Par exemple, si vous comparez une propriété de date/heure par rapport à une valeur constante, la valeur de chaîne doit représenter une date/heure.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="6f0bf-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="6f0bf-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6f0bf-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6f0bf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6f0bf-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6f0bf-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6f0bf-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6f0bf-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6f0bf-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6f0bf-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="6f0bf-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6f0bf-130">Validation File</span></span>  <br/> |<span data-ttu-id="6f0bf-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6f0bf-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6f0bf-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6f0bf-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6f0bf-133">False</span><span class="sxs-lookup"><span data-stu-id="6f0bf-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6f0bf-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6f0bf-134">See also</span></span>



- [<span data-ttu-id="6f0bf-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6f0bf-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

