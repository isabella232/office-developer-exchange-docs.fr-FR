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
description: L’élément DeleteItemField représente une opération permettant de supprimer une propriété donnée d’un élément lors d’un appel UpdateItem.
ms.openlocfilehash: e6f5ee8a1130d7c040f3ddd94021eff6d4a758b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455673"
---
# <a name="deleteitemfield"></a><span data-ttu-id="fc4be-103">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="fc4be-103">DeleteItemField</span></span>

<span data-ttu-id="fc4be-104">L’élément **DeleteItemField** représente une opération permettant de supprimer une propriété donnée d’un élément lors d’un appel UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="fc4be-104">The **DeleteItemField** element represents an operation to delete a given property from an item during an UpdateItem call.</span></span> 
 
- [<span data-ttu-id="fc4be-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="fc4be-105">UpdateItem</span></span>](updateitem.md)  
- [<span data-ttu-id="fc4be-106">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="fc4be-106">ItemChanges</span></span>](itemchanges.md) 
- [<span data-ttu-id="fc4be-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="fc4be-107">ItemChange</span></span>](itemchange.md) 
- [<span data-ttu-id="fc4be-108">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="fc4be-108">Updates (Item)</span></span>](updates-item.md) 
- [<span data-ttu-id="fc4be-109">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="fc4be-109">DeleteItemField</span></span>](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

```xml
<DeleteItemField>
   <IndexedFieldURI/> 
</DeleteItemField>
```

```xml
<DeleteItemField>
   <ExtendedFieldURI/>
</DeleteItemField>
```

<span data-ttu-id="fc4be-110">**DeleteItemFieldType**</span><span class="sxs-lookup"><span data-stu-id="fc4be-110">**DeleteItemFieldType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fc4be-111">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fc4be-111">Attributes and elements</span></span>

<span data-ttu-id="fc4be-112">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fc4be-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc4be-113">Attributs</span><span class="sxs-lookup"><span data-stu-id="fc4be-113">Attributes</span></span>

<span data-ttu-id="fc4be-114">Aucune.</span><span class="sxs-lookup"><span data-stu-id="fc4be-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc4be-115">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fc4be-115">Child elements</span></span>

|<span data-ttu-id="fc4be-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc4be-116">**Element**</span></span>|<span data-ttu-id="fc4be-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc4be-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc4be-118">FieldURI</span><span class="sxs-lookup"><span data-stu-id="fc4be-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="fc4be-119">Identifie les propriétés référencées fréquemment par URI.</span><span class="sxs-lookup"><span data-stu-id="fc4be-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="fc4be-120">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fc4be-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="fc4be-121">Identifie les membres individuels d’une propriété de dictionnaire.</span><span class="sxs-lookup"><span data-stu-id="fc4be-121">Identifies individual members of a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="fc4be-122">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="fc4be-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="fc4be-123">Identifie les propriétés MAPI étendues.</span><span class="sxs-lookup"><span data-stu-id="fc4be-123">Identifies extended MAPI properties.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc4be-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fc4be-124">Parent elements</span></span>

|<span data-ttu-id="fc4be-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fc4be-125">**Element**</span></span>|<span data-ttu-id="fc4be-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="fc4be-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc4be-127">Mises à jour (élément)</span><span class="sxs-lookup"><span data-stu-id="fc4be-127">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="fc4be-128">Contient un ensemble d’éléments qui définissent les modifications apportées aux propriétés des éléments par ajout, définition et suppression.</span><span class="sxs-lookup"><span data-stu-id="fc4be-128">Contains a set of elements that define append, set, and delete changes to item properties.</span></span>  <br/><br/><span data-ttu-id="fc4be-129">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="fc4be-129">The following is the XPath expression to this element:</span></span><br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc4be-130">Remarques</span><span class="sxs-lookup"><span data-stu-id="fc4be-130">Remarks</span></span>

<span data-ttu-id="fc4be-131">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fc4be-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc4be-132">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fc4be-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc4be-133">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fc4be-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc4be-134">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fc4be-134">Schema Name</span></span>  <br/> |<span data-ttu-id="fc4be-135">schéma de types</span><span class="sxs-lookup"><span data-stu-id="fc4be-135">types schema</span></span>  <br/> |
|<span data-ttu-id="fc4be-136">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fc4be-136">Validation File</span></span>  <br/> |<span data-ttu-id="fc4be-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fc4be-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc4be-138">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fc4be-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc4be-139">False</span><span class="sxs-lookup"><span data-stu-id="fc4be-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc4be-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fc4be-140">See also</span></span>

- [<span data-ttu-id="fc4be-141">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="fc4be-141">UpdateItem operation</span></span>](updateitem-operation.md)

