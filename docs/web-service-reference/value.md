---
title: Valeur
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: 9a30cadd-909e-41b1-b4e9-291643dd89c6
description: L’élément value contient la valeur d’une propriété étendue.
ms.openlocfilehash: 5de1528dda6d58ea772d050e709c0720e389fae6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465211"
---
# <a name="value"></a><span data-ttu-id="02070-103">Valeur</span><span class="sxs-lookup"><span data-stu-id="02070-103">Value</span></span>

<span data-ttu-id="02070-104">L’élément **value** contient la valeur d’une propriété étendue.</span><span class="sxs-lookup"><span data-stu-id="02070-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="02070-105">**String**</span><span class="sxs-lookup"><span data-stu-id="02070-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="02070-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="02070-106">Attributes and elements</span></span>

<span data-ttu-id="02070-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="02070-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="02070-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="02070-108">Attributes</span></span>

<span data-ttu-id="02070-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="02070-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="02070-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="02070-110">Child elements</span></span>

<span data-ttu-id="02070-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="02070-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="02070-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="02070-112">Parent elements</span></span>

|<span data-ttu-id="02070-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="02070-113">**Element**</span></span>|<span data-ttu-id="02070-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="02070-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="02070-115">Valeurs</span><span class="sxs-lookup"><span data-stu-id="02070-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="02070-116">Contient une collection de valeurs pour une propriété étendue.</span><span class="sxs-lookup"><span data-stu-id="02070-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="02070-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="02070-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="02070-118">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="02070-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="02070-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="02070-119">Text value</span></span>

<span data-ttu-id="02070-120">La valeur de texte doit être compatible avec le type indiqué par l’attribut PropertyType de l’ExtendedFieldURI.</span><span class="sxs-lookup"><span data-stu-id="02070-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="02070-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="02070-121">Remarks</span></span>

<span data-ttu-id="02070-122">Un élément **value** peut se produire dans des instances de propriétés étendues à valeur unique ou à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="02070-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="02070-123">Pour les instances à valeur unique, elle existe en tant qu’enfant direct de l’élément [ExtendedProperty](extendedproperty.md) .</span><span class="sxs-lookup"><span data-stu-id="02070-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="02070-124">Pour une instance à valeurs multiples, elle existe en tant qu’enfant direct de la collection **values** .</span><span class="sxs-lookup"><span data-stu-id="02070-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="02070-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="02070-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="02070-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="02070-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="02070-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="02070-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="02070-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="02070-128">Schema Name</span></span>  <br/> |<span data-ttu-id="02070-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="02070-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="02070-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="02070-130">Validation File</span></span>  <br/> |<span data-ttu-id="02070-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="02070-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="02070-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="02070-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="02070-133">False</span><span class="sxs-lookup"><span data-stu-id="02070-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="02070-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="02070-134">See also</span></span>

- [<span data-ttu-id="02070-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="02070-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

