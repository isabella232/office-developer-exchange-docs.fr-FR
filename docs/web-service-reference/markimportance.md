---
title: MarkImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkImportance
api_type:
- schema
ms.assetid: 32b8b08f-65e9-4764-b40a-63245551f4a3
description: L’élément MarkImportance spécifie l’importance à marquer sur les messages.
ms.openlocfilehash: 051307c0943a22e0c46439410806d168603d8a69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530880"
---
# <a name="markimportance"></a><span data-ttu-id="4db12-103">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="4db12-103">MarkImportance</span></span>

<span data-ttu-id="4db12-104">L’élément **MarkImportance** spécifie l’importance à marquer sur les messages.</span><span class="sxs-lookup"><span data-stu-id="4db12-104">The **MarkImportance** element specifies the importance that is to be stamped on messages.</span></span> 
  
```XML
<MarkImportance/>
```

 <span data-ttu-id="4db12-105">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="4db12-105">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4db12-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4db12-106">Attributes and elements</span></span>

<span data-ttu-id="4db12-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4db12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4db12-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4db12-108">Attributes</span></span>

<span data-ttu-id="4db12-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4db12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4db12-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4db12-110">Child elements</span></span>

<span data-ttu-id="4db12-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4db12-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4db12-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4db12-112">Parent elements</span></span>

|<span data-ttu-id="4db12-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4db12-113">**Element**</span></span>|<span data-ttu-id="4db12-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4db12-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4db12-115">Actions</span><span class="sxs-lookup"><span data-stu-id="4db12-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="4db12-116">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="4db12-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4db12-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4db12-117">Text value</span></span>

<span data-ttu-id="4db12-118">La valeur de texte de cet élément est restreinte à l’une des valeurs String suivantes :</span><span class="sxs-lookup"><span data-stu-id="4db12-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="4db12-119">Faible</span><span class="sxs-lookup"><span data-stu-id="4db12-119">Low</span></span>
    
- <span data-ttu-id="4db12-120">Normal</span><span class="sxs-lookup"><span data-stu-id="4db12-120">Normal</span></span>
    
- <span data-ttu-id="4db12-121">Importante</span><span class="sxs-lookup"><span data-stu-id="4db12-121">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="4db12-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="4db12-122">Remarks</span></span>

<span data-ttu-id="4db12-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4db12-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4db12-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4db12-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4db12-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4db12-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4db12-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4db12-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4db12-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4db12-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4db12-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4db12-128">Validation File</span></span>  <br/> |<span data-ttu-id="4db12-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4db12-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4db12-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4db12-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4db12-131">True</span><span class="sxs-lookup"><span data-stu-id="4db12-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4db12-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4db12-132">See also</span></span>



- [<span data-ttu-id="4db12-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4db12-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

