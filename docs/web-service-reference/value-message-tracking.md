---
title: Valeur (suivi des messages)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Value
api_type:
- schema
ms.assetid: cb2f228f-775a-4c7d-82e7-41c7c953c808
description: L’élément Value représente la valeur de la propriété d’un rapport de suivi des messages.
ms.openlocfilehash: 4f6b5cb9d82a35bbe010b36e409cdc9f3a70173d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465007"
---
# <a name="value-message-tracking"></a><span data-ttu-id="829b7-103">Valeur (suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="829b7-103">Value (Message Tracking)</span></span>

<span data-ttu-id="829b7-104">L’élément **value** représente la valeur de la propriété d’un rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="829b7-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="829b7-105">**String**</span><span class="sxs-lookup"><span data-stu-id="829b7-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="829b7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="829b7-106">Attributes and elements</span></span>

<span data-ttu-id="829b7-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="829b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="829b7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="829b7-108">Attributes</span></span>

<span data-ttu-id="829b7-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="829b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="829b7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="829b7-110">Child elements</span></span>

<span data-ttu-id="829b7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="829b7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="829b7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="829b7-112">Parent elements</span></span>

|<span data-ttu-id="829b7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="829b7-113">**Element**</span></span>|<span data-ttu-id="829b7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="829b7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="829b7-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="829b7-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="829b7-116">Représente une paire nom/valeur de chaînes qui est utilisée pour créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="829b7-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="829b7-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="829b7-117">Text value</span></span>

<span data-ttu-id="829b7-118">La valeur texte est facultative.</span><span class="sxs-lookup"><span data-stu-id="829b7-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="829b7-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="829b7-119">Remarks</span></span>

<span data-ttu-id="829b7-120">Cet élément peut apparaître au plus une fois dans l’élément [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="829b7-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="829b7-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="829b7-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="829b7-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="829b7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="829b7-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="829b7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="829b7-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="829b7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="829b7-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="829b7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="829b7-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="829b7-126">Validation File</span></span>  <br/> |<span data-ttu-id="829b7-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="829b7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="829b7-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="829b7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="829b7-129">False</span><span class="sxs-lookup"><span data-stu-id="829b7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="829b7-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="829b7-130">See also</span></span>

- [<span data-ttu-id="829b7-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="829b7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

