---
title: SortOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SortOrder
api_type:
- schema
ms.assetid: c2413f0b-8c03-46ae-9990-13338b3c53a6
description: L’élément SortOrder définit le mode de tri des éléments dans une requête FindItem ou FindConversation.
ms.openlocfilehash: b520bb3ca6daadc777e7235b2b7420a12e425048
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468368"
---
# <a name="sortorder"></a><span data-ttu-id="57905-103">SortOrder</span><span class="sxs-lookup"><span data-stu-id="57905-103">SortOrder</span></span>

<span data-ttu-id="57905-104">L’élément **SortOrder** définit le mode de tri des éléments dans une requête **FindItem** ou **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="57905-104">The **SortOrder** element defines how items are sorted in a **FindItem** or **FindConversation** request.</span></span> 
  
```xml
<SortOrder>
   <FieldOrder/>
</SortOrder>
```

 <span data-ttu-id="57905-105">**NonEmptyArrayOfFieldOrdersType**</span><span class="sxs-lookup"><span data-stu-id="57905-105">**NonEmptyArrayOfFieldOrdersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57905-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="57905-106">Attributes and elements</span></span>

<span data-ttu-id="57905-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="57905-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57905-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="57905-108">Attributes</span></span>

<span data-ttu-id="57905-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="57905-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57905-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="57905-110">Child elements</span></span>

|<span data-ttu-id="57905-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="57905-111">**Element**</span></span>|<span data-ttu-id="57905-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="57905-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57905-113">FieldOrder</span><span class="sxs-lookup"><span data-stu-id="57905-113">FieldOrder</span></span>](fieldorder.md) <br/> |<span data-ttu-id="57905-114">Représente un champ unique par lequel trier les résultats et indique le sens du tri.</span><span class="sxs-lookup"><span data-stu-id="57905-114">Represents a single field by which to sort results and indicates the direction for the sort.</span></span> <span data-ttu-id="57905-115">Un ou plusieurs de ces éléments peuvent être inclus.</span><span class="sxs-lookup"><span data-stu-id="57905-115">One or more of these elements may be included.</span></span> <span data-ttu-id="57905-116">Les éléments [FieldOrder](fieldorder.md) sont appliqués dans l’ordre spécifié pour le tri.</span><span class="sxs-lookup"><span data-stu-id="57905-116">[FieldOrder](fieldorder.md) elements are applied in the order specified for sorting.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57905-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="57905-117">Parent elements</span></span>

|<span data-ttu-id="57905-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="57905-118">**Element**</span></span>|<span data-ttu-id="57905-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="57905-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57905-120">FindItem</span><span class="sxs-lookup"><span data-stu-id="57905-120">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="57905-121">Définit une requête pour rechercher des éléments dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57905-121">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="57905-122">Voici l’expression XPath de cet élément :`/FindItem`</span><span class="sxs-lookup"><span data-stu-id="57905-122">The following is the XPath expression to this element:  `/FindItem`</span></span> <br/> |
|[<span data-ttu-id="57905-123">FindConversation</span><span class="sxs-lookup"><span data-stu-id="57905-123">FindConversation</span></span>](findconversation.md) <br/> |<span data-ttu-id="57905-124">Définit une requête pour rechercher des conversations dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="57905-124">Defines a request to find conversations in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57905-125">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="57905-125">Text value</span></span>

<span data-ttu-id="57905-126">Aucun.</span><span class="sxs-lookup"><span data-stu-id="57905-126">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57905-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="57905-127">Remarks</span></span>

<span data-ttu-id="57905-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="57905-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57905-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="57905-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57905-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="57905-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57905-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="57905-131">Schema Name</span></span>  <br/> |<span data-ttu-id="57905-132">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="57905-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57905-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="57905-133">Validation File</span></span>  <br/> |<span data-ttu-id="57905-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="57905-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57905-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="57905-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="57905-136">False</span><span class="sxs-lookup"><span data-stu-id="57905-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57905-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="57905-137">See also</span></span>



[<span data-ttu-id="57905-138">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="57905-138">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="57905-139">Opération FindConversation</span><span class="sxs-lookup"><span data-stu-id="57905-139">FindConversation operation</span></span>](findconversation-operation.md)


- [<span data-ttu-id="57905-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="57905-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

