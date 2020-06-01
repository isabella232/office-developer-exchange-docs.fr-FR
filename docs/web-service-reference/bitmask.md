---
title: Composé
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
description: L’élément masque binaire représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction exclusions.
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458809"
---
# <a name="bitmask"></a><span data-ttu-id="c6d05-103">Composé</span><span class="sxs-lookup"><span data-stu-id="c6d05-103">Bitmask</span></span>

<span data-ttu-id="c6d05-104">L’élément **masque binaire** représente un masque hexadécimal ou décimal à utiliser pendant une opération de restriction [exclusions](excludes.md) .</span><span class="sxs-lookup"><span data-stu-id="c6d05-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="c6d05-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="c6d05-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c6d05-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c6d05-106">Attributes and elements</span></span>

<span data-ttu-id="c6d05-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c6d05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6d05-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c6d05-108">Attributes</span></span>

|<span data-ttu-id="c6d05-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c6d05-109">**Attribute**</span></span>|<span data-ttu-id="c6d05-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6d05-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c6d05-111">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c6d05-111">**Value**</span></span> | <span data-ttu-id="c6d05-112">Représente un masque de réfixe décimal ou hexadécimal.</span><span class="sxs-lookup"><span data-stu-id="c6d05-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="c6d05-113">La valeur est représentée par l’expression régulière suivante :</span><span class="sxs-lookup"><span data-stu-id="c6d05-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="c6d05-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span><span class="sxs-lookup"><span data-stu-id="c6d05-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span></span><br/><br/><span data-ttu-id="c6d05-115">Voici des exemples de valeurs hexadécimales pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="c6d05-115">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="c6d05-116">- 0x12AF</span><span class="sxs-lookup"><span data-stu-id="c6d05-116">- 0x12AF</span></span><br/><span data-ttu-id="c6d05-117">- 0X334AE</span><span class="sxs-lookup"><span data-stu-id="c6d05-117">- 0X334AE</span></span><br/><br/><span data-ttu-id="c6d05-118">Voici des exemples de valeurs décimales pour cet attribut :</span><span class="sxs-lookup"><span data-stu-id="c6d05-118">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="c6d05-119">-10</span><span class="sxs-lookup"><span data-stu-id="c6d05-119">- 10</span></span><br/><span data-ttu-id="c6d05-120">-255</span><span class="sxs-lookup"><span data-stu-id="c6d05-120">- 255</span></span><br/><span data-ttu-id="c6d05-121">-4562</span><span class="sxs-lookup"><span data-stu-id="c6d05-121">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="c6d05-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c6d05-122">Child elements</span></span>

<span data-ttu-id="c6d05-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c6d05-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6d05-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c6d05-124">Parent elements</span></span>

|<span data-ttu-id="c6d05-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c6d05-125">**Element**</span></span>|<span data-ttu-id="c6d05-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="c6d05-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6d05-127">Exclut</span><span class="sxs-lookup"><span data-stu-id="c6d05-127">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="c6d05-128">Effectue un masque de bits des propriétés.</span><span class="sxs-lookup"><span data-stu-id="c6d05-128">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c6d05-129">Remarques</span><span class="sxs-lookup"><span data-stu-id="c6d05-129">Remarks</span></span>

<span data-ttu-id="c6d05-130">Les valeurs hexadécimales doivent avoir un préfixe 0x ou 0X.</span><span class="sxs-lookup"><span data-stu-id="c6d05-130">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="c6d05-131">Si ce préfixe n’existe pas, la valeur est supposée être un nombre décimal.</span><span class="sxs-lookup"><span data-stu-id="c6d05-131">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="c6d05-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c6d05-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6d05-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c6d05-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6d05-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c6d05-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6d05-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c6d05-135">Schema name</span></span>  <br/> |<span data-ttu-id="c6d05-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c6d05-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6d05-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c6d05-137">Validation file</span></span>  <br/> |<span data-ttu-id="c6d05-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c6d05-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6d05-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c6d05-139">Can be empty</span></span>  <br/> |<span data-ttu-id="c6d05-140">False</span><span class="sxs-lookup"><span data-stu-id="c6d05-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6d05-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c6d05-141">See also</span></span>

- [<span data-ttu-id="c6d05-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c6d05-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

