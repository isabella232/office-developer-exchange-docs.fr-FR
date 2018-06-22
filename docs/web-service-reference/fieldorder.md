---
title: FieldOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FieldOrder
api_type:
- schema
ms.assetid: b9364842-bbe2-4221-afef-bf5022bc89ec
description: L’élément FieldOrder représente un seul champ à utiliser pour trier les résultats et indique le sens du tri.
ms.openlocfilehash: 10e28f066f7fa6799bf6b03b694d98825f95626d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756355"
---
# <a name="fieldorder"></a><span data-ttu-id="c96ff-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="c96ff-103">FieldOrder</span></span>

<span data-ttu-id="c96ff-104">L’élément **FieldOrder** représente un seul champ à utiliser pour trier les résultats et indique le sens du tri.</span><span class="sxs-lookup"><span data-stu-id="c96ff-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

 <span data-ttu-id="c96ff-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="c96ff-105">**FieldOrderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c96ff-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c96ff-106">Attributes and elements</span></span>

<span data-ttu-id="c96ff-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c96ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c96ff-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c96ff-108">Attributes</span></span>

|<span data-ttu-id="c96ff-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="c96ff-109">**Attribute**</span></span>|<span data-ttu-id="c96ff-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="c96ff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c96ff-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="c96ff-111">**Order**</span></span> <br/> | <span data-ttu-id="c96ff-112">Décrit la direction d’ordre de tri.</span><span class="sxs-lookup"><span data-stu-id="c96ff-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="c96ff-113">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="c96ff-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="c96ff-114">-Croissant</span><span class="sxs-lookup"><span data-stu-id="c96ff-114">-  Ascending</span></span>  <br/><span data-ttu-id="c96ff-115">-Décroissant</span><span class="sxs-lookup"><span data-stu-id="c96ff-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c96ff-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c96ff-116">Child elements</span></span>

|<span data-ttu-id="c96ff-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c96ff-117">**Element**</span></span>|<span data-ttu-id="c96ff-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="c96ff-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c96ff-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="c96ff-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="c96ff-120">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="c96ff-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="c96ff-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c96ff-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="c96ff-122">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="c96ff-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="c96ff-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="c96ff-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="c96ff-124">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="c96ff-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c96ff-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c96ff-125">Parent elements</span></span>

|<span data-ttu-id="c96ff-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c96ff-126">**Element**</span></span>|<span data-ttu-id="c96ff-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="c96ff-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c96ff-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="c96ff-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="c96ff-129">Définit comment les éléments sont triés dans une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="c96ff-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="c96ff-130">Vous trouverez ci-dessous l’expression XPath pour cet élément :`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="c96ff-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c96ff-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="c96ff-131">Remarks</span></span>

<span data-ttu-id="c96ff-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="c96ff-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c96ff-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c96ff-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c96ff-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c96ff-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c96ff-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c96ff-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c96ff-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c96ff-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c96ff-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c96ff-137">Validation File</span></span>  <br/> |<span data-ttu-id="c96ff-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c96ff-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c96ff-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c96ff-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c96ff-140">False</span><span class="sxs-lookup"><span data-stu-id="c96ff-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c96ff-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c96ff-141">See also</span></span>

- [<span data-ttu-id="c96ff-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c96ff-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

