---
title: Exists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exists
api_type:
- schema
ms.assetid: 55d568bd-8dbc-4d50-b9d7-54b74a54d4b5
description: L’élément Exists représente une expression de recherche qui renvoie true si la propriété fournie existe sur un élément.
ms.openlocfilehash: d30f4b505afcac32afbfeaf2289c964ba145668e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756252"
---
# <a name="exists"></a><span data-ttu-id="f2c78-103">Exists</span><span class="sxs-lookup"><span data-stu-id="f2c78-103">Exists</span></span>

<span data-ttu-id="f2c78-104">L’élément **Exists** représente une expression de recherche qui retourne la **valeur true** si la propriété fournie existe sur un élément.</span><span class="sxs-lookup"><span data-stu-id="f2c78-104">The **Exists** element represents a search expression that returns **true** if the supplied property exists on an item.</span></span> 
  
```xml
<Exists>
   <Path/>
</Exists>
```

 <span data-ttu-id="f2c78-105">**ExistsType**</span><span class="sxs-lookup"><span data-stu-id="f2c78-105">**ExistsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2c78-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f2c78-106">Attributes and elements</span></span>

<span data-ttu-id="f2c78-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f2c78-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2c78-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f2c78-108">Attributes</span></span>

<span data-ttu-id="f2c78-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f2c78-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2c78-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f2c78-110">Child elements</span></span>

|<span data-ttu-id="f2c78-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2c78-111">**Element**</span></span>|<span data-ttu-id="f2c78-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2c78-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2c78-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="f2c78-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f2c78-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="f2c78-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f2c78-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f2c78-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f2c78-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="f2c78-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f2c78-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f2c78-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f2c78-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="f2c78-118">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2c78-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f2c78-119">Parent elements</span></span>

|<span data-ttu-id="f2c78-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f2c78-120">**Element**</span></span>|<span data-ttu-id="f2c78-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="f2c78-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2c78-122">Restriction</span><span class="sxs-lookup"><span data-stu-id="f2c78-122">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="f2c78-123">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="f2c78-123">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="f2c78-124">Pas</span><span class="sxs-lookup"><span data-stu-id="f2c78-124">Not</span></span>](not.md) <br/> |<span data-ttu-id="f2c78-125">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="f2c78-125">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="f2c78-126">And</span><span class="sxs-lookup"><span data-stu-id="f2c78-126">And</span></span>](and.md) <br/> |<span data-ttu-id="f2c78-127">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="f2c78-127">Represents a search expression that enables you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="f2c78-128">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="f2c78-128">The result of the And operation is **true** if all the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="f2c78-129">Or</span><span class="sxs-lookup"><span data-stu-id="f2c78-129">Or</span></span>](or.md) <br/> |<span data-ttu-id="f2c78-130">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="f2c78-130">Represents a search expression that performs a logical OR on the search expression that it contains.</span></span> <span data-ttu-id="f2c78-131">[Ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="f2c78-131">[Or](or.md) will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2c78-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="f2c78-132">Remarks</span></span>

<span data-ttu-id="f2c78-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f2c78-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2c78-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f2c78-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2c78-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f2c78-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2c78-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f2c78-136">Schema Name</span></span>  <br/> |<span data-ttu-id="f2c78-137">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f2c78-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2c78-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f2c78-138">Validation File</span></span>  <br/> |<span data-ttu-id="f2c78-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f2c78-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2c78-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f2c78-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2c78-141">False</span><span class="sxs-lookup"><span data-stu-id="f2c78-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2c78-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f2c78-142">See also</span></span>



- [<span data-ttu-id="f2c78-143">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f2c78-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

