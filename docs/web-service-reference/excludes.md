---
title: Exclut
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Excludes
api_type:
- schema
ms.assetid: bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1
description: L’élément exclut effectue un masque de bits de la propriété spécifiée et une valeur fournie.
ms.openlocfilehash: 73e4eb782a4f54c113ea9a9b67fcf185a9028153
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756249"
---
# <a name="excludes"></a><span data-ttu-id="33968-103">Exclut</span><span class="sxs-lookup"><span data-stu-id="33968-103">Excludes</span></span>

<span data-ttu-id="33968-104">L’élément **exclut** effectue un masque de bits de la propriété spécifiée et une valeur fournie.</span><span class="sxs-lookup"><span data-stu-id="33968-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

 <span data-ttu-id="33968-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="33968-105">**ExcludesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33968-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="33968-106">Attributes and elements</span></span>

<span data-ttu-id="33968-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="33968-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33968-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="33968-108">Attributes</span></span>

<span data-ttu-id="33968-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="33968-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33968-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="33968-110">Child elements</span></span>

|<span data-ttu-id="33968-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="33968-111">**Element**</span></span>|<span data-ttu-id="33968-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="33968-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33968-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="33968-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="33968-114">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="33968-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="33968-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="33968-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="33968-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="33968-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="33968-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="33968-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="33968-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="33968-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="33968-119">Masque de bits</span><span class="sxs-lookup"><span data-stu-id="33968-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="33968-120">Représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des [exclusions](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="33968-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="33968-121">Si le masque de bits représente un nombre hexadécimal, il doit être précédé 0 x ou 0 X.</span><span class="sxs-lookup"><span data-stu-id="33968-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="33968-122">Dans le cas contraire, il sera considéré un nombre décimal.</span><span class="sxs-lookup"><span data-stu-id="33968-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="33968-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="33968-123">Parent elements</span></span>

|<span data-ttu-id="33968-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="33968-124">**Element**</span></span>|<span data-ttu-id="33968-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="33968-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33968-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="33968-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="33968-127">Représente la restriction ou la requête qui est utilisé pour filtrer des éléments ou des dossiers dans les opérations de dossier FindItem/FindFolder et la recherche.</span><span class="sxs-lookup"><span data-stu-id="33968-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="33968-128">Pas</span><span class="sxs-lookup"><span data-stu-id="33968-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="33968-129">Représente une expression de recherche qui inverse la valeur booléenne de l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="33968-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="33968-130">And</span><span class="sxs-lookup"><span data-stu-id="33968-130">And</span></span>](and.md) <br/> |<span data-ttu-id="33968-131">Représente une expression de recherche qui vous permet d’effectuer une opération de type Boolean et entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="33968-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="33968-132">Le résultat de l’opération est **la valeur true** si toutes les expressions de recherche contenues dans l’And sont **remplies**.</span><span class="sxs-lookup"><span data-stu-id="33968-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="33968-133">Or</span><span class="sxs-lookup"><span data-stu-id="33968-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="33968-134">Représente une expression de recherche qui effectue une opération OR logique sur l’expression de recherche qu’il contient.</span><span class="sxs-lookup"><span data-stu-id="33968-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="33968-135">L’élément [ou](or.md) renvoie **la valeur true** si un de ses enfants retourne **true**.</span><span class="sxs-lookup"><span data-stu-id="33968-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="33968-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="33968-136">Remarks</span></span>

 <span data-ttu-id="33968-137">**Exclut** permettra de résoudre **la valeur True** si une opération et effectuée sur les éléments suivants est résolu à 0 :</span><span class="sxs-lookup"><span data-stu-id="33968-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="33968-138">La valeur de la propriété binaire</span><span class="sxs-lookup"><span data-stu-id="33968-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="33968-139">La valeur de masque de bits pour la propriété</span><span class="sxs-lookup"><span data-stu-id="33968-139">The bitmask value for the property</span></span>
    
 <span data-ttu-id="33968-140">**Exclut** peut uniquement être appliqué à une propriété qui a une valeur entière.</span><span class="sxs-lookup"><span data-stu-id="33968-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="33968-141">Si le type de propriété n’est pas un entier, un code d’erreur de **ErrorUnsupportedPathForQuery** est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="33968-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="33968-142">Vous pouvez effectuer l’opération inverse en appelant Not(Excludes).</span><span class="sxs-lookup"><span data-stu-id="33968-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="33968-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="33968-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="33968-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="33968-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33968-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="33968-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33968-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="33968-146">Schema Name</span></span>  <br/> |<span data-ttu-id="33968-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="33968-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="33968-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="33968-148">Validation File</span></span>  <br/> |<span data-ttu-id="33968-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="33968-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33968-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="33968-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="33968-151">False</span><span class="sxs-lookup"><span data-stu-id="33968-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33968-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="33968-152">See also</span></span>



- [<span data-ttu-id="33968-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="33968-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

