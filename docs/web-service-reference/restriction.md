---
title: Restriction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Restriction
api_type:
- schema
ms.assetid: 77f19014-d112-4999-8e83-ecc32a117a73
description: L’élément restriction représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.
ms.openlocfilehash: 6037ba15417d67d393ca70f3edf2248749c396e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465288"
---
# <a name="restriction"></a><span data-ttu-id="0b8ec-103">Restriction</span><span class="sxs-lookup"><span data-stu-id="0b8ec-103">Restriction</span></span>

<span data-ttu-id="0b8ec-104">L’élément **restriction** représente la restriction ou la requête utilisée pour filtrer des éléments ou des dossiers dans les opérations FindItem/FindFolder et Search Folder.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-104">The **Restriction** element represents the restriction or query that is used to filter items or folders in FindItem/FindFolder and search folder operations.</span></span> 
  
```xml
<Restriction>
   <SearchExpression/>
</Restriction>
```

 <span data-ttu-id="0b8ec-105">**RestrictionType**</span><span class="sxs-lookup"><span data-stu-id="0b8ec-105">**RestrictionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b8ec-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0b8ec-106">Attributes and elements</span></span>

<span data-ttu-id="0b8ec-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b8ec-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0b8ec-108">Attributes</span></span>

<span data-ttu-id="0b8ec-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b8ec-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0b8ec-110">Child elements</span></span>

|<span data-ttu-id="0b8ec-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0b8ec-111">**Element**</span></span>|<span data-ttu-id="0b8ec-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b8ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b8ec-113">And</span><span class="sxs-lookup"><span data-stu-id="0b8ec-113">And</span></span>](and.md) <br/> |<span data-ttu-id="0b8ec-114">Représente une expression de recherche qui vous permet d’effectuer une opération booléenne **et** une opération entre deux ou plusieurs expressions de recherche.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-114">Represents a search expression that enables you to perform a Boolean **AND** operation between two or more search expressions.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-115">Contains</span><span class="sxs-lookup"><span data-stu-id="0b8ec-115">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="0b8ec-116">Représente une expression de recherche qui détermine si une propriété donnée contient la valeur de chaîne de constante fournie.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-116">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-117">Exclut</span><span class="sxs-lookup"><span data-stu-id="0b8ec-117">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="0b8ec-118">Effectue un masque de bits des propriétés.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-118">Performs a bitwise mask of the properties.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-119">Exists</span><span class="sxs-lookup"><span data-stu-id="0b8ec-119">Exists</span></span>](exists.md) <br/> |<span data-ttu-id="0b8ec-120">Représente une expression de recherche qui renvoie la **valeur true** si la propriété fournie existe sur un élément.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-120">Represents a search expression that returns **true** if the supplied property exists on an item.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-121">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="0b8ec-121">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="0b8ec-122">Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et donne la **valeur true** si elles sont égales.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-122">Represents a search expression that compares a property with either a constant value or another property and evaluates to **true** if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-123">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="0b8ec-123">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="0b8ec-124">Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure à la valeur ou à la propriété.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-124">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-125">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0b8ec-125">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="0b8ec-126">Représente une expression de recherche qui compare une propriété avec une valeur de constante ou une autre propriété et renvoie la **valeur true** si la première propriété est supérieure ou égale à la valeur ou à la propriété.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-126">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is greater than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-127">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="0b8ec-127">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="0b8ec-128">Représente une expression de recherche qui compare une propriété à une valeur constante ou à une autre propriété et renvoie la **valeur true** si la première propriété est inférieure à la valeur ou à la propriété.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-128">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-129">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="0b8ec-129">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="0b8ec-130">Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et renvoie la **valeur true** si la première propriété est inférieure ou égale à la valeur ou à la propriété.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-130">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the first property is less than or equal to the value or property.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-131">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="0b8ec-131">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="0b8ec-132">Représente une expression de recherche qui compare une propriété à une valeur de constante ou à une autre propriété et renvoie la **valeur true** si les valeurs ne sont pas identiques.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-132">Represents a search expression that compares a property with either a constant value or another property and returns **true** if the values are not the same.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-133">Not</span><span class="sxs-lookup"><span data-stu-id="0b8ec-133">Not</span></span>](not.md) <br/> |<span data-ttu-id="0b8ec-134">Représente une expression de recherche qui nie la valeur booléenne de l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-134">Represents a search expression that negates the Boolean value of the search expression it contains.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-135">Or</span><span class="sxs-lookup"><span data-stu-id="0b8ec-135">Or</span></span>](or.md) <br/> |<span data-ttu-id="0b8ec-136">Représente une expression de recherche qui effectue une opération **or** logique sur l’expression de recherche qu’elle contient.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-136">Represents a search expression that performs a logical **OR** operation on the search expression it contains.</span></span> <span data-ttu-id="0b8ec-137">L’élément **ou** renvoie la **valeur true** si l’un de ses enfants renvoie la **valeur true**.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-137">The **Or** element will return **true** if any of its children return **true**.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-138">SearchExpression</span><span class="sxs-lookup"><span data-stu-id="0b8ec-138">SearchExpression</span></span>](searchexpression.md) <br/> |<span data-ttu-id="0b8ec-139">Représente l’élément substitué dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-139">Represents the substituted element within a restriction.</span></span> <span data-ttu-id="0b8ec-140">Cet élément n’est pas utilisé dans un document d’instance XML.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-140">This element is not used in an XML instance document.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b8ec-141">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0b8ec-141">Parent elements</span></span>

|<span data-ttu-id="0b8ec-142">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0b8ec-142">**Element**</span></span>|<span data-ttu-id="0b8ec-143">**Description**</span><span class="sxs-lookup"><span data-stu-id="0b8ec-143">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b8ec-144">FindFolder</span><span class="sxs-lookup"><span data-stu-id="0b8ec-144">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="0b8ec-145">Définit une demande pour identifier les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-145">Defines a request to identify folders in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-146">FindItem</span><span class="sxs-lookup"><span data-stu-id="0b8ec-146">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="0b8ec-147">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-147">Defines a request to find items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0b8ec-148">SearchParameters</span><span class="sxs-lookup"><span data-stu-id="0b8ec-148">SearchParameters</span></span>](searchparameters.md) <br/> |<span data-ttu-id="0b8ec-149">Représente les paramètres qui définissent un dossier de recherche.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-149">Represents the parameters that define a search folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b8ec-150">Remarques</span><span class="sxs-lookup"><span data-stu-id="0b8ec-150">Remarks</span></span>

<span data-ttu-id="0b8ec-151">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0b8ec-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b8ec-152">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0b8ec-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b8ec-153">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0b8ec-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b8ec-154">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0b8ec-154">Schema Name</span></span>  <br/> |<span data-ttu-id="0b8ec-155">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0b8ec-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b8ec-156">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0b8ec-156">Validation File</span></span>  <br/> |<span data-ttu-id="0b8ec-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0b8ec-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b8ec-158">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0b8ec-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b8ec-159">False</span><span class="sxs-lookup"><span data-stu-id="0b8ec-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b8ec-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0b8ec-160">See also</span></span>



- [<span data-ttu-id="0b8ec-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0b8ec-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

