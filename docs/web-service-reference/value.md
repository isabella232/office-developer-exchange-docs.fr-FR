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
description: L’élément Value contient la valeur d’une propriété étendue.
ms.openlocfilehash: 4b8674d267b78f0384f9457e794e88ace8234826
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839008"
---
# <a name="value"></a><span data-ttu-id="8d99a-103">Valeur</span><span class="sxs-lookup"><span data-stu-id="8d99a-103">Value</span></span>

<span data-ttu-id="8d99a-104">L’élément **Value** contient la valeur d’une propriété étendue.</span><span class="sxs-lookup"><span data-stu-id="8d99a-104">The **Value** element contains the value of an extended property.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="8d99a-105">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="8d99a-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8d99a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8d99a-106">Attributes and elements</span></span>

<span data-ttu-id="8d99a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8d99a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d99a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8d99a-108">Attributes</span></span>

<span data-ttu-id="8d99a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d99a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d99a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8d99a-110">Child elements</span></span>

<span data-ttu-id="8d99a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d99a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d99a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8d99a-112">Parent elements</span></span>

|<span data-ttu-id="8d99a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8d99a-113">**Element**</span></span>|<span data-ttu-id="8d99a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d99a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d99a-115">Values</span><span class="sxs-lookup"><span data-stu-id="8d99a-115">Values</span></span>](values.md) <br/> |<span data-ttu-id="8d99a-116">Contient une collection de valeurs pour une propriété étendue.</span><span class="sxs-lookup"><span data-stu-id="8d99a-116">Contains a collection of values for an extended property.</span></span>  <br/> |
|[<span data-ttu-id="8d99a-117">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="8d99a-117">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="8d99a-118">Identifie les propriétés étendues sur les dossiers et les éléments.</span><span class="sxs-lookup"><span data-stu-id="8d99a-118">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d99a-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="8d99a-119">Text value</span></span>

<span data-ttu-id="8d99a-120">La valeur de texte doit être compatible avec le type est indiqué par l’attribut PropertyType de la ExtendedFieldURI.</span><span class="sxs-lookup"><span data-stu-id="8d99a-120">The text value must be compatible with the type that is indicated by the PropertyType attribute of the ExtendedFieldURI.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d99a-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="8d99a-121">Remarks</span></span>

<span data-ttu-id="8d99a-122">Un élément de la **valeur** peut se produire dans les deux instances de la propriété étendue unique et à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="8d99a-122">A **Value** element can occur in both single and multivalued extended property instances.</span></span> <span data-ttu-id="8d99a-123">Pour les instances à valeur unique, il existe en tant qu’enfant de l’élément [ExtendedProperty](extendedproperty.md) direct.</span><span class="sxs-lookup"><span data-stu-id="8d99a-123">For single-valued instances, it exists as a direct child of the [ExtendedProperty](extendedproperty.md) element.</span></span> <span data-ttu-id="8d99a-124">Pour l’instance à valeurs multiples, il existe en tant qu’un enfant direct de la collection de **valeurs** .</span><span class="sxs-lookup"><span data-stu-id="8d99a-124">For multivalued instance, it exists as a direct child of the **Values** collection.</span></span> 
  
<span data-ttu-id="8d99a-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8d99a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d99a-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8d99a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d99a-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8d99a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d99a-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8d99a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="8d99a-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8d99a-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d99a-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8d99a-130">Validation File</span></span>  <br/> |<span data-ttu-id="8d99a-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d99a-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d99a-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8d99a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d99a-133">False</span><span class="sxs-lookup"><span data-stu-id="8d99a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d99a-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8d99a-134">See also</span></span>

- [<span data-ttu-id="8d99a-135">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8d99a-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

