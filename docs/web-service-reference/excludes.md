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
description: L’élément excludes effectue un masque de bits de la propriété spécifiée et une valeur fournie.
ms.openlocfilehash: d5fcd8b86b454aa731bd43974b5b7d674fe76ed6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530613"
---
# <a name="excludes"></a><span data-ttu-id="e2325-103">Exclut</span><span class="sxs-lookup"><span data-stu-id="e2325-103">Excludes</span></span>

<span data-ttu-id="e2325-104">L’élément **excludes** effectue un masque de bits de la propriété spécifiée et une valeur fournie.</span><span class="sxs-lookup"><span data-stu-id="e2325-104">The **Excludes** element performs a bitwise mask of the specified property and a supplied value.</span></span> 
  
```xml
<Excludes>
   <FieldURI/>
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <ExtendedFieldURI/> 
   <Bitmask/>
</Excludes>
```

```xml
<Excludes>
   <IndexedFieldURI/> 
   <Bitmask/>
</Excludes>
```

<span data-ttu-id="e2325-105">**ExcludesType**</span><span class="sxs-lookup"><span data-stu-id="e2325-105">**ExcludesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e2325-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e2325-106">Attributes and elements</span></span>

<span data-ttu-id="e2325-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e2325-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2325-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e2325-108">Attributes</span></span>

<span data-ttu-id="e2325-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e2325-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2325-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e2325-110">Child elements</span></span>

|<span data-ttu-id="e2325-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2325-111">**Element**</span></span>|<span data-ttu-id="e2325-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2325-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2325-113">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e2325-113">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="e2325-114">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="e2325-114">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="e2325-115">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e2325-115">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="e2325-116">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="e2325-116">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="e2325-117">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="e2325-117">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="e2325-118">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="e2325-118">Identifies MAPI properties.</span></span>  <br/> |
|[<span data-ttu-id="e2325-119">Composé</span><span class="sxs-lookup"><span data-stu-id="e2325-119">Bitmask</span></span>](bitmask.md) <br/> |<span data-ttu-id="e2325-120">Représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction [exclusions](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="e2325-120">Represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> <span data-ttu-id="e2325-121">Si le masque binaire représente un nombre hexadécimal, il doit être préfixé par 0x ou 0X.</span><span class="sxs-lookup"><span data-stu-id="e2325-121">If the bitmask represents a hexadecimal number, it must be prefixed by 0x or 0X.</span></span> <span data-ttu-id="e2325-122">Sinon, il est considéré comme un nombre décimal.</span><span class="sxs-lookup"><span data-stu-id="e2325-122">Otherwise, it will be considered a decimal number.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2325-123">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e2325-123">Parent elements</span></span>

|<span data-ttu-id="e2325-124">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e2325-124">**Element**</span></span>|<span data-ttu-id="e2325-125">**Description**</span><span class="sxs-lookup"><span data-stu-id="e2325-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2325-126">Restriction</span><span class="sxs-lookup"><span data-stu-id="e2325-126">Restriction</span></span>](restriction.md) <br/> |<span data-ttu-id="e2325-127">Représente la restriction ou la requête qui est utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="e2325-127">Represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span>  <br/> |
|[<span data-ttu-id="e2325-128">Not</span><span class="sxs-lookup"><span data-stu-id="e2325-128">Not</span></span>](not.md) <br/> |<span data-ttu-id="e2325-129">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="e2325-129">Represents a search expression that negates the Boolean value of the search expression that it contains.</span></span>  <br/> |
|[<span data-ttu-id="e2325-130">And</span><span class="sxs-lookup"><span data-stu-id="e2325-130">And</span></span>](and.md) <br/> |<span data-ttu-id="e2325-131">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne et une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="e2325-131">Represents a search expression that allows you to perform a Boolean And operation between two or more search expressions.</span></span> <span data-ttu-id="e2325-132">Le résultat de l’opération and est **true** si toutes les expressions de recherche contenues dans le et sont **vraies**.</span><span class="sxs-lookup"><span data-stu-id="e2325-132">The result of the And operation is **true** if all of the search expressions contained within the And are **true**.</span></span>  <br/> |
|[<span data-ttu-id="e2325-133">Or</span><span class="sxs-lookup"><span data-stu-id="e2325-133">Or</span></span>](or.md) <br/> |<span data-ttu-id="e2325-134">Représente une expression de recherche qui effectue une ou logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="e2325-134">Represents a search expression that performs a logical OR on the search expression it contains.</span></span> <span data-ttu-id="e2325-135">L’élément [ou](or.md) renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="e2325-135">The [Or](or.md) element will return **true** if any of its children return **true**.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e2325-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="e2325-136">Remarks</span></span>

<span data-ttu-id="e2325-137">**Exclusions** se traduit par la **valeur true** si une opération and effectuée sur les valeurs suivantes est résolue à 0 :</span><span class="sxs-lookup"><span data-stu-id="e2325-137">**Excludes** will resolve to **true** if an AND operation performed on the following resolves to 0:</span></span> 
  
1. <span data-ttu-id="e2325-138">Valeur de bits de la propriété</span><span class="sxs-lookup"><span data-stu-id="e2325-138">The bitwise value for the property</span></span>
    
2. <span data-ttu-id="e2325-139">Valeur de masque de masque de la propriété</span><span class="sxs-lookup"><span data-stu-id="e2325-139">The bitmask value for the property</span></span>
    
<span data-ttu-id="e2325-140">Les **exclusions** ne peuvent être appliquées qu’à une propriété qui a une valeur entière.</span><span class="sxs-lookup"><span data-stu-id="e2325-140">**Excludes** can only be applied to a property that has an integer value.</span></span> <span data-ttu-id="e2325-141">Si le type de propriété n’est pas un entier, un code d’erreur **ErrorUnsupportedPathForQuery** est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="e2325-141">If the property type is anything other than an integer, an error code of **ErrorUnsupportedPathForQuery** is returned in the response.</span></span> 
  
<span data-ttu-id="e2325-142">Vous pouvez effectuer l’opération inverse en appelant la méthode not (exclut).</span><span class="sxs-lookup"><span data-stu-id="e2325-142">You can perform the reverse operation by calling Not(Excludes).</span></span>
  
<span data-ttu-id="e2325-143">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e2325-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2325-144">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e2325-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2325-145">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e2325-145">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2325-146">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e2325-146">Schema Name</span></span>  <br/> |<span data-ttu-id="e2325-147">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e2325-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2325-148">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e2325-148">Validation File</span></span>  <br/> |<span data-ttu-id="e2325-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2325-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2325-150">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e2325-150">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2325-151">False</span><span class="sxs-lookup"><span data-stu-id="e2325-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2325-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e2325-152">See also</span></span>

- [<span data-ttu-id="e2325-153">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e2325-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

