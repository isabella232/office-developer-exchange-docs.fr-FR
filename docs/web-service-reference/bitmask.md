---
title: Masque de bits
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: L’élément de masque de bits représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des exclusions.
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755401"
---
# <a name="bitmask"></a><span data-ttu-id="94083-103">Masque de bits</span><span class="sxs-lookup"><span data-stu-id="94083-103">Bitmask</span></span>

<span data-ttu-id="94083-104">L’élément de **masque de bits** représente un masque hexadécimal ou décimal à utiliser lors d’une opération de restriction des [exclusions](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="94083-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="94083-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="94083-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="94083-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="94083-106">Attributes and elements</span></span>

<span data-ttu-id="94083-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="94083-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94083-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="94083-108">Attributes</span></span>

|<span data-ttu-id="94083-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="94083-109">**Attribute**</span></span>|<span data-ttu-id="94083-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="94083-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="94083-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="94083-111">**Value**</span></span> | <span data-ttu-id="94083-112">Représente un masque de bits décimal ou hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="94083-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="94083-113">La valeur est représentée par l’expression régulière suivante :</span><span class="sxs-lookup"><span data-stu-id="94083-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="94083-114">« ((0 x</span><span class="sxs-lookup"><span data-stu-id="94083-114">\`((0x</span></span>|<span data-ttu-id="94083-115">0X)[0-9A-FA-f]\*)</span><span class="sxs-lookup"><span data-stu-id="94083-115">0X)[0-9A-Fa-f]\*)</span></span>|<span data-ttu-id="94083-116">([0-9] \*) ».</span><span class="sxs-lookup"><span data-stu-id="94083-116">([0-9]\*)\`.</span></span><br/><br/><span data-ttu-id="94083-117">Voici des exemples de valeurs hexadécimales pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="94083-117">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="94083-118">-0x12AF</span><span class="sxs-lookup"><span data-stu-id="94083-118">- 0x12AF</span></span><br/><span data-ttu-id="94083-119">-0X334AE</span><span class="sxs-lookup"><span data-stu-id="94083-119">- 0X334AE</span></span><br/><br/><span data-ttu-id="94083-120">Voici des exemples de valeurs décimales de cet attribut :</span><span class="sxs-lookup"><span data-stu-id="94083-120">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="94083-121">-10</span><span class="sxs-lookup"><span data-stu-id="94083-121">- 10</span></span><br/><span data-ttu-id="94083-122">-255</span><span class="sxs-lookup"><span data-stu-id="94083-122">- 255</span></span><br/><span data-ttu-id="94083-123">-4562</span><span class="sxs-lookup"><span data-stu-id="94083-123">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="94083-124">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="94083-124">Child elements</span></span>

<span data-ttu-id="94083-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="94083-125">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94083-126">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="94083-126">Parent elements</span></span>

|<span data-ttu-id="94083-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="94083-127">**Element**</span></span>|<span data-ttu-id="94083-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="94083-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94083-129">Exclut</span><span class="sxs-lookup"><span data-stu-id="94083-129">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="94083-130">Effectue un masque de bits des propriétés.</span><span class="sxs-lookup"><span data-stu-id="94083-130">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="94083-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="94083-131">Remarks</span></span>

<span data-ttu-id="94083-132">Des valeurs hexadécimales doivent avoir un préfixe 0 x ou 0 X.</span><span class="sxs-lookup"><span data-stu-id="94083-132">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="94083-133">Si ce préfixe n’existe pas, la valeur est supposée être un nombre décimal.</span><span class="sxs-lookup"><span data-stu-id="94083-133">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="94083-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="94083-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="94083-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="94083-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94083-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="94083-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94083-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="94083-137">Schema name</span></span>  <br/> |<span data-ttu-id="94083-138">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="94083-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="94083-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="94083-139">Validation file</span></span>  <br/> |<span data-ttu-id="94083-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94083-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94083-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="94083-141">Can be empty</span></span>  <br/> |<span data-ttu-id="94083-142">False</span><span class="sxs-lookup"><span data-stu-id="94083-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94083-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="94083-143">See also</span></span>

- [<span data-ttu-id="94083-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="94083-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

