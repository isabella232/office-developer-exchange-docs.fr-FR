---
title: DelegationState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegationState
api_type:
- schema
ms.assetid: 9dbb83ed-1ded-48f3-8e06-2489fc8b28d5
description: L’élément DelegationState représente l’état d’une tâche déléguée.
ms.openlocfilehash: 00b0e41ae223f1c70f9a3a21662e8858f8690a86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755840"
---
# <a name="delegationstate"></a><span data-ttu-id="c7436-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="c7436-103">DelegationState</span></span>

<span data-ttu-id="c7436-104">L’élément **DelegationState** représente l’état d’une tâche déléguée.</span><span class="sxs-lookup"><span data-stu-id="c7436-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="c7436-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="c7436-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c7436-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c7436-106">Attributes and elements</span></span>

<span data-ttu-id="c7436-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c7436-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7436-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c7436-108">Attributes</span></span>

<span data-ttu-id="c7436-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c7436-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7436-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c7436-110">Child elements</span></span>

<span data-ttu-id="c7436-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c7436-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c7436-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c7436-112">Parent elements</span></span>

|<span data-ttu-id="c7436-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c7436-113">**Element**</span></span>|<span data-ttu-id="c7436-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="c7436-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7436-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="c7436-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="c7436-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7436-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c7436-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c7436-117">Text value</span></span>

<span data-ttu-id="c7436-118">Il s’agit d’une propriété en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="c7436-118">This is a read-only property.</span></span> <span data-ttu-id="c7436-119">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="c7436-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="c7436-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="c7436-120">NoMatch</span></span>
    
- <span data-ttu-id="c7436-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="c7436-121">OwnNew</span></span>
    
- <span data-ttu-id="c7436-122">Propriétaire</span><span class="sxs-lookup"><span data-stu-id="c7436-122">Owned</span></span>
    
- <span data-ttu-id="c7436-123">Acceptée</span><span class="sxs-lookup"><span data-stu-id="c7436-123">Accepted</span></span>
    
- <span data-ttu-id="c7436-124">Refusée</span><span class="sxs-lookup"><span data-stu-id="c7436-124">Declined</span></span>
    
- <span data-ttu-id="c7436-125">Max</span><span class="sxs-lookup"><span data-stu-id="c7436-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="c7436-126">Note</span><span class="sxs-lookup"><span data-stu-id="c7436-126">Remarks</span></span>

<span data-ttu-id="c7436-127">Exchange Web Services dans Microsoft Exchange Server 2007 ne prend pas en charge les affectations de tâches.</span><span class="sxs-lookup"><span data-stu-id="c7436-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="c7436-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c7436-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7436-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c7436-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7436-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c7436-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7436-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c7436-131">Schema Name</span></span>  <br/> |<span data-ttu-id="c7436-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c7436-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7436-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c7436-133">Validation File</span></span>  <br/> |<span data-ttu-id="c7436-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c7436-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7436-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c7436-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7436-136">False</span><span class="sxs-lookup"><span data-stu-id="c7436-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7436-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c7436-137">See also</span></span>

- [<span data-ttu-id="c7436-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c7436-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

