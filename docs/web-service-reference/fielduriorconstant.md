---
title: FieldURIOrConstant
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldURIOrConstant
api_type:
- schema
ms.assetid: 89d7a87e-7c93-49b8-83ec-8798e08c1052
description: L’élément FieldURIOrConstant représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.
ms.openlocfilehash: a24c2fa044e03d0ac6f900625e325600903df8d0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354224"
---
# <a name="fielduriorconstant"></a><span data-ttu-id="f04ff-103">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="f04ff-103">FieldURIOrConstant</span></span>

<span data-ttu-id="f04ff-104">L’élément **FieldURIOrConstant** représente une propriété ou une constante à utiliser lors de la comparaison avec une autre propriété.</span><span class="sxs-lookup"><span data-stu-id="f04ff-104">The **FieldURIOrConstant** element represents either a property or a constant value to be used when comparing with another property.</span></span> 
  
```xml
<FieldURIOrConstant>
   <Constant/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
    <IndexedFieldURI/> 
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <FieldURI/>
</FieldURIOrConstant>
```

```xml
<FieldURIOrConstant>
   <ExtendedFieldURI/> 
</FieldURIOrConstant>
```

<span data-ttu-id="f04ff-105">**FieldURIOrConstantType**</span><span class="sxs-lookup"><span data-stu-id="f04ff-105">**FieldURIOrConstantType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="f04ff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f04ff-106">Attributes and elements</span></span>

<span data-ttu-id="f04ff-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f04ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f04ff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f04ff-108">Attributes</span></span>

<span data-ttu-id="f04ff-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f04ff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f04ff-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f04ff-110">Child elements</span></span>

|<span data-ttu-id="f04ff-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f04ff-111">**Element**</span></span>|<span data-ttu-id="f04ff-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="f04ff-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f04ff-113">Constante</span><span class="sxs-lookup"><span data-stu-id="f04ff-113">Constant</span></span>](constant.md) <br/> |<span data-ttu-id="f04ff-114">Identifie une valeur de constante dans une restriction.</span><span class="sxs-lookup"><span data-stu-id="f04ff-114">Identifies a constant value in a restriction.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="f04ff-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="f04ff-116">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="f04ff-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f04ff-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="f04ff-118">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="f04ff-118">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-119">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="f04ff-119">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="f04ff-120">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="f04ff-120">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f04ff-121">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f04ff-121">Parent elements</span></span>

|<span data-ttu-id="f04ff-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f04ff-122">**Element**</span></span>|<span data-ttu-id="f04ff-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="f04ff-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f04ff-124">IsEqualTo</span><span class="sxs-lookup"><span data-stu-id="f04ff-124">IsEqualTo</span></span>](isequalto.md) <br/> |<span data-ttu-id="f04ff-125">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et donne la valeur true si elles sont égales.</span><span class="sxs-lookup"><span data-stu-id="f04ff-125">Represents a search expression that compares a property with either a constant value or another property and evaluates to true if they are equal.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-126">IsGreaterThan</span><span class="sxs-lookup"><span data-stu-id="f04ff-126">IsGreaterThan</span></span>](isgreaterthan.md) <br/> |<span data-ttu-id="f04ff-127">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est supérieure.</span><span class="sxs-lookup"><span data-stu-id="f04ff-127">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-128">IsGreaterThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f04ff-128">IsGreaterThanOrEqualTo</span></span>](isgreaterthanorequalto.md) <br/> |<span data-ttu-id="f04ff-129">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est supérieure ou égale à la seconde valeur ou la propriété.</span><span class="sxs-lookup"><span data-stu-id="f04ff-129">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is greater than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-130">IsLessThan</span><span class="sxs-lookup"><span data-stu-id="f04ff-130">IsLessThan</span></span>](islessthan.md) <br/> |<span data-ttu-id="f04ff-131">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est inférieure à la seconde valeur ou la propriété.</span><span class="sxs-lookup"><span data-stu-id="f04ff-131">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-132">IsLessThanOrEqualTo</span><span class="sxs-lookup"><span data-stu-id="f04ff-132">IsLessThanOrEqualTo</span></span>](islessthanorequalto.md) <br/> |<span data-ttu-id="f04ff-133">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si la première propriété est inférieure ou égale à la seconde valeur ou la propriété.</span><span class="sxs-lookup"><span data-stu-id="f04ff-133">Represents a search expression that compares a property with either a constant value or another property and returns true if the first property is less than or equal to the second value or property.</span></span>  <br/> |
|[<span data-ttu-id="f04ff-134">IsNotEqualTo</span><span class="sxs-lookup"><span data-stu-id="f04ff-134">IsNotEqualTo</span></span>](isnotequalto.md) <br/> |<span data-ttu-id="f04ff-135">Représente une expression de recherche qui compare une propriété avec une valeur constante ou une autre propriété et renvoie la valeur true si les valeurs ne sont pas identiques.</span><span class="sxs-lookup"><span data-stu-id="f04ff-135">Represents a search expression that compares a property with either a constant value or another property and returns true if the values are not the same.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f04ff-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="f04ff-136">Remarks</span></span>

<span data-ttu-id="f04ff-137">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f04ff-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="f04ff-138">Exemple</span><span class="sxs-lookup"><span data-stu-id="f04ff-138">Example</span></span>

<span data-ttu-id="f04ff-139">L’exemple XML suivant montre l’élément FieldURIOrConstant utilisé avec une constante et le champ URI.</span><span class="sxs-lookup"><span data-stu-id="f04ff-139">The following XML example shows the FieldURIOrConstant element used with both a constant and field URI.</span></span>
  
```xml
<Restriction>
  <Or xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
    <IsEqualTo>
      <FieldURI FieldURI="item:DateTimeCreated"/>
      <FieldURIOrConstant>
        <FieldURI FieldURI="item:DateTimeReceived"/>
      </FieldURIOrConstant>
    </IsEqualTo>
    <IsEqualTo>
      <FieldURI FieldURI="item:Subject"/>
      <FieldURIOrConstant>
        <Constant Value="Here is a test message"/>
      </FieldURIOrConstant>
    </IsEqualTo>
  </Or>
</Restriction>
```

## <a name="element-information"></a><span data-ttu-id="f04ff-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f04ff-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f04ff-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f04ff-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f04ff-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f04ff-142">Schema Name</span></span>  <br/> |<span data-ttu-id="f04ff-143">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f04ff-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="f04ff-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f04ff-144">Validation File</span></span>  <br/> |<span data-ttu-id="f04ff-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f04ff-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f04ff-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f04ff-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="f04ff-147">False</span><span class="sxs-lookup"><span data-stu-id="f04ff-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f04ff-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f04ff-148">See also</span></span>

- [<span data-ttu-id="f04ff-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f04ff-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

