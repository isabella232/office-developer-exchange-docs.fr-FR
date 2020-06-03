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
description: L’élément DelegationState, représente l’état d’une tâche déléguée.
ms.openlocfilehash: b938b5a2240283c265006dd47cd6ff475ad80978
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457367"
---
# <a name="delegationstate"></a><span data-ttu-id="8d127-103">DelegationState</span><span class="sxs-lookup"><span data-stu-id="8d127-103">DelegationState</span></span>

<span data-ttu-id="8d127-104">L’élément **DelegationState,** représente l’état d’une tâche déléguée.</span><span class="sxs-lookup"><span data-stu-id="8d127-104">The **DelegationState** element represents the status of a delegated task.</span></span> 
  
```xml
<DelegationState/>
```

<span data-ttu-id="8d127-105">**TaskDelegateStateType**</span><span class="sxs-lookup"><span data-stu-id="8d127-105">**TaskDelegateStateType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8d127-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8d127-106">Attributes and elements</span></span>

<span data-ttu-id="8d127-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8d127-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d127-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8d127-108">Attributes</span></span>

<span data-ttu-id="8d127-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="8d127-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d127-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8d127-110">Child elements</span></span>

<span data-ttu-id="8d127-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8d127-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d127-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8d127-112">Parent elements</span></span>

|<span data-ttu-id="8d127-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="8d127-113">**Element**</span></span>|<span data-ttu-id="8d127-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="8d127-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d127-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="8d127-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="8d127-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="8d127-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d127-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="8d127-117">Text value</span></span>

<span data-ttu-id="8d127-118">Il s’agit d’une propriété en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="8d127-118">This is a read-only property.</span></span> <span data-ttu-id="8d127-119">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="8d127-119">The following are the possible values:</span></span>
  
- <span data-ttu-id="8d127-120">NoMatch</span><span class="sxs-lookup"><span data-stu-id="8d127-120">NoMatch</span></span>
    
- <span data-ttu-id="8d127-121">OwnNew</span><span class="sxs-lookup"><span data-stu-id="8d127-121">OwnNew</span></span>
    
- <span data-ttu-id="8d127-122">Appartien</span><span class="sxs-lookup"><span data-stu-id="8d127-122">Owned</span></span>
    
- <span data-ttu-id="8d127-123">Accepted</span><span class="sxs-lookup"><span data-stu-id="8d127-123">Accepted</span></span>
    
- <span data-ttu-id="8d127-124">Refusée</span><span class="sxs-lookup"><span data-stu-id="8d127-124">Declined</span></span>
    
- <span data-ttu-id="8d127-125">Max</span><span class="sxs-lookup"><span data-stu-id="8d127-125">Max</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8d127-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="8d127-126">Remarks</span></span>

<span data-ttu-id="8d127-127">Les services Web Exchange dans Microsoft Exchange Server 2007 ne prennent pas en charge les affectations de tâches.</span><span class="sxs-lookup"><span data-stu-id="8d127-127">Exchange Web Services in Microsoft Exchange Server 2007 does not support task assignments.</span></span>
  
<span data-ttu-id="8d127-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange 2007 sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="8d127-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d127-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8d127-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d127-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8d127-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d127-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8d127-131">Schema Name</span></span>  <br/> |<span data-ttu-id="8d127-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="8d127-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d127-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8d127-133">Validation File</span></span>  <br/> |<span data-ttu-id="8d127-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8d127-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d127-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8d127-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d127-136">False</span><span class="sxs-lookup"><span data-stu-id="8d127-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d127-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8d127-137">See also</span></span>

- [<span data-ttu-id="8d127-138">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="8d127-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

