---
title: Nom (suivi des messages)
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
description: L’élément Name représente le nom de la propriété pour un rapport de suivi des messages.
ms.openlocfilehash: 86f049c0a90dbeb55418a5eee58079adf17e5ded
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466898"
---
# <a name="name-message-tracking"></a><span data-ttu-id="8a3f1-103">Nom (suivi des messages)</span><span class="sxs-lookup"><span data-stu-id="8a3f1-103">Name (Message Tracking)</span></span>

<span data-ttu-id="8a3f1-104">L’élément **Name** représente le nom de la propriété pour un rapport de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-104">The **Name** element represents the property name for a message tracking report.</span></span> 
  
```xml
<Name/>
```

<span data-ttu-id="8a3f1-105">**String**</span><span class="sxs-lookup"><span data-stu-id="8a3f1-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8a3f1-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8a3f1-106">Attributes and elements</span></span>

<span data-ttu-id="8a3f1-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a3f1-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8a3f1-108">Attributes</span></span>

<span data-ttu-id="8a3f1-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8a3f1-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8a3f1-110">Child elements</span></span>

<span data-ttu-id="8a3f1-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8a3f1-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8a3f1-112">Parent elements</span></span>

|<span data-ttu-id="8a3f1-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8a3f1-113">**Element**</span></span>|<span data-ttu-id="8a3f1-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8a3f1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a3f1-115">TrackingPropertyType</span><span class="sxs-lookup"><span data-stu-id="8a3f1-115">TrackingPropertyType</span></span>](trackingpropertytype.md) <br/> |<span data-ttu-id="8a3f1-116">Représente une paire nom/valeur de chaînes qui est utilisée pour créer des propriétés pour les rapports de suivi des messages.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-116">Represents a name and value pair of strings that is used to create properties for message tracking reports.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8a3f1-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8a3f1-117">Text value</span></span>

<span data-ttu-id="8a3f1-118">Une valeur de texte est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="8a3f1-118">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8a3f1-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="8a3f1-119">Remarks</span></span>

<span data-ttu-id="8a3f1-120">Cet élément peut apparaître au plus une fois dans l’élément [TrackingPropertyType](trackingpropertytype.md) .</span><span class="sxs-lookup"><span data-stu-id="8a3f1-120">This element can occur at most one time in the [TrackingPropertyType](trackingpropertytype.md) element.</span></span> 
  
<span data-ttu-id="8a3f1-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="8a3f1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a3f1-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8a3f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a3f1-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8a3f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a3f1-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8a3f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="8a3f1-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8a3f1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a3f1-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8a3f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="8a3f1-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a3f1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a3f1-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8a3f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a3f1-129">False</span><span class="sxs-lookup"><span data-stu-id="8a3f1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a3f1-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8a3f1-130">See also</span></span>

- [<span data-ttu-id="8a3f1-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8a3f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

