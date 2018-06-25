---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: L’élément DeleteItemField représente une opération de suppression d’une propriété donnée d’un élément pendant un appel UpdateItem.
ms.openlocfilehash: 2388bd10379211a31890b7c4f27920431ce444c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755870"
---
# <a name="deleteitemfield"></a><span data-ttu-id="07314-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="07314-103">DeleteItemField</span></span>

<span data-ttu-id="07314-104">L’élément **DeleteItemField** représente une opération de suppression d’une propriété donnée d’un élément pendant un appel UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="07314-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="07314-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="07314-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="07314-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="07314-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="07314-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="07314-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="07314-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="07314-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="07314-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="07314-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

 <span data-ttu-id="07314-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="07314-110">**DeleteItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07314-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="07314-111">Attributes and elements</span></span>

<span data-ttu-id="07314-112">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="07314-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07314-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="07314-113">Attributes</span></span>

<span data-ttu-id="07314-114">Aucun.</span><span class="sxs-lookup"><span data-stu-id="07314-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07314-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="07314-115">Child elements</span></span>

|<span data-ttu-id="07314-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07314-116">**Element**</span></span>|<span data-ttu-id="07314-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="07314-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07314-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="07314-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="07314-119">Identifie les propriétés fréquemment référencées par un URI.</span><span class="sxs-lookup"><span data-stu-id="07314-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="07314-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="07314-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="07314-121">Identifie les membres individuels d’une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="07314-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="07314-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="07314-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="07314-123">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="07314-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07314-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="07314-124">Parent elements</span></span>

|<span data-ttu-id="07314-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="07314-125">**Element**</span></span>|<span data-ttu-id="07314-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="07314-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07314-127">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="07314-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="07314-128">Contient un ensemble d’éléments qui définissent append, définir et supprimer les modifications apportées aux propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="07314-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="07314-129">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="07314-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07314-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="07314-130">Remarks</span></span>

<span data-ttu-id="07314-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="07314-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07314-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="07314-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07314-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="07314-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07314-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="07314-134">Schema Name</span></span>  <br/> |<span data-ttu-id="07314-135">schéma de types</span><span class="sxs-lookup"><span data-stu-id="07314-135">types schema</span></span>  <br/> |
|<span data-ttu-id="07314-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="07314-136">Validation File</span></span>  <br/> |<span data-ttu-id="07314-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07314-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07314-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="07314-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="07314-139">False</span><span class="sxs-lookup"><span data-stu-id="07314-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07314-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="07314-140">See also</span></span>

- [<span data-ttu-id="07314-141">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="07314-141">UpdateItem operation</span></span>](updateitem-operation.md)

