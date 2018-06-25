---
title: Nom (le suivi des messages)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Name
api_type:
- schema
ms.assetid: a1669f6d-53f3-4849-9b30-56909aaeac82
description: L’élément Name représente le nom de propriété pour un rapport de suivi des messages.
ms.openlocfilehash: c905df03842de47b2bcbd62897aa9a8cf464cc6d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828501"
---
# <a name="name-message-tracking"></a><span data-ttu-id="72237-103">Nom (le suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="72237-103">Name (Message Tracking)</span></span>

<span data-ttu-id="72237-104">L’élément **Name** représente le nom de propriété pour un rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="72237-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="72237-105">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="72237-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="72237-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="72237-106">Attributes and elements</span></span>

<span data-ttu-id="72237-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="72237-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72237-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="72237-108">Attributes</span></span>

<span data-ttu-id="72237-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="72237-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72237-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="72237-110">Child elements</span></span>

<span data-ttu-id="72237-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="72237-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72237-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="72237-112">Parent elements</span></span>

|<span data-ttu-id="72237-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="72237-113">**Element**</span></span>|<span data-ttu-id="72237-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="72237-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72237-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="72237-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="72237-116">Représente une paire nom / valeur de chaînes qui sert à créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="72237-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72237-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="72237-117">Text value</span></span>

<span data-ttu-id="72237-118">Une valeur de texte est obligatoire si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="72237-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72237-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="72237-119">Remarks</span></span>

<span data-ttu-id="72237-120">Cet élément peut se produire au maximum une seule fois dans l’élément [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="72237-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="72237-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="72237-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72237-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="72237-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72237-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="72237-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="72237-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="72237-124">Schema Name</span></span>  <br/> |<span data-ttu-id="72237-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="72237-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="72237-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="72237-126">Validation File</span></span>  <br/> |<span data-ttu-id="72237-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="72237-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="72237-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="72237-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="72237-129">False</span><span class="sxs-lookup"><span data-stu-id="72237-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72237-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="72237-130">See also</span></span>

- [<span data-ttu-id="72237-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72237-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

