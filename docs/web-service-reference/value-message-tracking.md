---
title: Valeur (le suivi des messages)
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
description: L’élément de la valeur représente la valeur de propriété pour un rapport de suivi des messages.
ms.openlocfilehash: 152e4fe61a4cff8013ae02900bd84bf244ae84a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838996"
---
# <a name="value-message-tracking"></a><span data-ttu-id="0f2bc-103">Valeur (le suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="0f2bc-103">Value (Message Tracking)</span></span>

<span data-ttu-id="0f2bc-104">L’élément de la **valeur** représente la valeur de propriété pour un rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-104">The **Value** element represents the property value for a message tracking report.</span></span> 
  
```xml
<Value/>
```

<span data-ttu-id="0f2bc-105">**Chaîne**</span><span class="sxs-lookup"><span data-stu-id="0f2bc-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="0f2bc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f2bc-106">Attributes and elements</span></span>

<span data-ttu-id="0f2bc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f2bc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f2bc-108">Attributes</span></span>

<span data-ttu-id="0f2bc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f2bc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f2bc-110">Child elements</span></span>

<span data-ttu-id="0f2bc-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0f2bc-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f2bc-112">Parent elements</span></span>

|<span data-ttu-id="0f2bc-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f2bc-113">**Element**</span></span>|<span data-ttu-id="0f2bc-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f2bc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f2bc-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="0f2bc-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="0f2bc-116">Représente une paire nom / valeur de chaînes qui sert à créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0f2bc-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="0f2bc-117">Text value</span></span>

<span data-ttu-id="0f2bc-118">La valeur de texte est facultative.</span><span class="sxs-lookup"><span data-stu-id="0f2bc-118">The text value is optional.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0f2bc-119">Note</span><span class="sxs-lookup"><span data-stu-id="0f2bc-119">Remarks</span></span>

<span data-ttu-id="0f2bc-120">Cet élément peut se produire au maximum une seule fois dans l’élément [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="0f2bc-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="0f2bc-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="0f2bc-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f2bc-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f2bc-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f2bc-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f2bc-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0f2bc-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f2bc-124">Schema Name</span></span>  <br/> |<span data-ttu-id="0f2bc-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="0f2bc-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="0f2bc-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f2bc-126">Validation File</span></span>  <br/> |<span data-ttu-id="0f2bc-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0f2bc-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0f2bc-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f2bc-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="0f2bc-129">False</span><span class="sxs-lookup"><span data-stu-id="0f2bc-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f2bc-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f2bc-130">See also</span></span>

- [<span data-ttu-id="0f2bc-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f2bc-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

