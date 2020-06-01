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
description: L’élément FieldOrder représente un champ unique par lequel trier les résultats et indique le sens du tri.
ms.openlocfilehash: 19dee7175d541dd99b53e004ea8ccd785b619184
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461260"
---
# <a name="fieldorder"></a><span data-ttu-id="5de9a-103">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="5de9a-103">FieldOrder</span></span>

<span data-ttu-id="5de9a-104">L’élément **FieldOrder** représente un champ unique par lequel trier les résultats et indique le sens du tri.</span><span class="sxs-lookup"><span data-stu-id="5de9a-104">The **FieldOrder** element represents a single field by which to sort results and indicates the direction for the sort.</span></span> 
  
```xml
<FieldOrder Order="">
   <FieldURI/>
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <ExtendedFieldURI/> 
</FieldOrder>
```

```xml
<FieldOrder Order="">
   <IndexedFieldURI/>
</FieldOrder>
```

<span data-ttu-id="5de9a-105">**FieldOrderType**</span><span class="sxs-lookup"><span data-stu-id="5de9a-105">**FieldOrderType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="5de9a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5de9a-106">Attributes and elements</span></span>

<span data-ttu-id="5de9a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5de9a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5de9a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5de9a-108">Attributes</span></span>

|<span data-ttu-id="5de9a-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="5de9a-109">**Attribute**</span></span>|<span data-ttu-id="5de9a-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="5de9a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5de9a-111">**Order**</span><span class="sxs-lookup"><span data-stu-id="5de9a-111">**Order**</span></span> <br/> | <span data-ttu-id="5de9a-112">Décrit la direction de l’ordre de tri.</span><span class="sxs-lookup"><span data-stu-id="5de9a-112">Describes the sort order direction.</span></span><br/><br/> <span data-ttu-id="5de9a-113">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="5de9a-113">The following are the possible values:</span></span> <br/> <br/><span data-ttu-id="5de9a-114">-Croissant</span><span class="sxs-lookup"><span data-stu-id="5de9a-114">-  Ascending</span></span>  <br/><span data-ttu-id="5de9a-115">-Descending</span><span class="sxs-lookup"><span data-stu-id="5de9a-115">-  Descending</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5de9a-116">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5de9a-116">Child elements</span></span>

|<span data-ttu-id="5de9a-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5de9a-117">**Element**</span></span>|<span data-ttu-id="5de9a-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="5de9a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5de9a-119">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5de9a-119">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="5de9a-120">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="5de9a-120">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="5de9a-121">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5de9a-121">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="5de9a-122">Identifie les membres individuels d’un dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="5de9a-122">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="5de9a-123">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="5de9a-123">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="5de9a-124">Identifie les propriétés MAPI.</span><span class="sxs-lookup"><span data-stu-id="5de9a-124">Identifies MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5de9a-125">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5de9a-125">Parent elements</span></span>

|<span data-ttu-id="5de9a-126">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5de9a-126">**Element**</span></span>|<span data-ttu-id="5de9a-127">**Description**</span><span class="sxs-lookup"><span data-stu-id="5de9a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5de9a-128">SortOrder</span><span class="sxs-lookup"><span data-stu-id="5de9a-128">SortOrder</span></span>](sortorder.md) <br/> |<span data-ttu-id="5de9a-129">Définit le mode de tri des éléments dans une requête FindItem.</span><span class="sxs-lookup"><span data-stu-id="5de9a-129">Defines how items are sorted in a FindItem request.</span></span>  <br/> <span data-ttu-id="5de9a-130">Voici l’expression XPath de cet élément :`/FindItem/SortOrder`</span><span class="sxs-lookup"><span data-stu-id="5de9a-130">The following is the XPath expression to this element:  `/FindItem/SortOrder`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5de9a-131">Remarques</span><span class="sxs-lookup"><span data-stu-id="5de9a-131">Remarks</span></span>

<span data-ttu-id="5de9a-132">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5de9a-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5de9a-133">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5de9a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5de9a-134">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5de9a-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5de9a-135">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5de9a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="5de9a-136">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="5de9a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="5de9a-137">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5de9a-137">Validation File</span></span>  <br/> |<span data-ttu-id="5de9a-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5de9a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5de9a-139">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5de9a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="5de9a-140">False</span><span class="sxs-lookup"><span data-stu-id="5de9a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5de9a-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5de9a-141">See also</span></span>

- [<span data-ttu-id="5de9a-142">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5de9a-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

