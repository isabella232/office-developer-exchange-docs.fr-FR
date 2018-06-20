---
title: IsGreaterThan
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsGreaterThan
api_type:
- schema
ms.assetid: a6e9d462-cfa7-40ec-903e-128c95050352
description: L’élément IsGreaterThan représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est supérieure.
ms.openlocfilehash: f36ad646e6c2d415d14d4311a9971a56a85a3121
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828031"
---
# <a name="isgreaterthan"></a><span data-ttu-id="e9dcb-103">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="e9dcb-103">IsGreaterThan</span></span>

<span data-ttu-id="e9dcb-104">L’élément **IsGreaterThan** représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie **la valeur true** si la première propriété est supérieure.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-104">The **IsGreaterThan** element represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater.</span></span> 
  
```xml
<IsGreaterThan>
   <FieldURI/>
   <FieldURIOrConstant/>
</IsGreaterThan>
```

 <span data-ttu-id="e9dcb-105">**IsGreaterThanType**</span><span class="sxs-lookup"><span data-stu-id="e9dcb-105">**IsGreaterThanType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e9dcb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e9dcb-106">Attributes and elements</span></span>

<span data-ttu-id="e9dcb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e9dcb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e9dcb-108">Attributes</span></span>

<span data-ttu-id="e9dcb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e9dcb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e9dcb-110">Child elements</span></span>

|<span data-ttu-id="e9dcb-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9dcb-111">**Element**</span></span>|<span data-ttu-id="e9dcb-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9dcb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9dcb-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e9dcb-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="e9dcb-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e9dcb-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="e9dcb-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e9dcb-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e9dcb-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-119">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="e9dcb-119">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="e9dcb-120">Représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-120">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e9dcb-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e9dcb-121">Parent elements</span></span>

|<span data-ttu-id="e9dcb-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e9dcb-122">**Element**</span></span>|<span data-ttu-id="e9dcb-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="e9dcb-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e9dcb-124">Restriction</span><span class="sxs-lookup"><span data-stu-id="e9dcb-124">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e9dcb-125">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-125">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-126">Pas</span><span class="sxs-lookup"><span data-stu-id="e9dcb-126">Not</span></span>](not.md) <br/> |<span data-ttu-id="e9dcb-127">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-127">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-128">And</span><span class="sxs-lookup"><span data-stu-id="e9dcb-128">And</span></span>](and.md) <br/> |<span data-ttu-id="e9dcb-129">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-129">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="e9dcb-130">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-130">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="e9dcb-131">Or</span><span class="sxs-lookup"><span data-stu-id="e9dcb-131">Or</span></span>](or.md) <br/> |<span data-ttu-id="e9dcb-132">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-132">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="e9dcb-133">[Ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-133">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e9dcb-134">Remarques</span><span class="sxs-lookup"><span data-stu-id="e9dcb-134">Remarks</span></span>

<span data-ttu-id="e9dcb-135">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e9dcb-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e9dcb-136">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e9dcb-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e9dcb-137">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e9dcb-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e9dcb-138">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e9dcb-138">Schema Name</span></span>  <br/> |<span data-ttu-id="e9dcb-139">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e9dcb-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="e9dcb-140">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e9dcb-140">Validation File</span></span>  <br/> |<span data-ttu-id="e9dcb-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e9dcb-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e9dcb-142">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e9dcb-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="e9dcb-143">False</span><span class="sxs-lookup"><span data-stu-id="e9dcb-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e9dcb-144">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e9dcb-144">See also</span></span>



- [<span data-ttu-id="e9dcb-145">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e9dcb-145">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

