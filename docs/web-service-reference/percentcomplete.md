---
title: PercentComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PercentComplete
api_type:
- schema
ms.assetid: 58a67f8a-c4dc-42dc-97ae-a9e5cc672d2d
description: L’élément PercentComplete décrit l’état d’achèvement d’une tâche.
ms.openlocfilehash: 18e53221ecdf60df195445ed7692c03795bdcc1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828717"
---
# <a name="percentcomplete"></a><span data-ttu-id="353d7-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="353d7-103">PercentComplete</span></span>

<span data-ttu-id="353d7-104">L’élément **PercentComplete** décrit l’état d’achèvement d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="353d7-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="353d7-105">**Double**</span><span class="sxs-lookup"><span data-stu-id="353d7-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="353d7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="353d7-106">Attributes and elements</span></span>

<span data-ttu-id="353d7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="353d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="353d7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="353d7-108">Attributes</span></span>

<span data-ttu-id="353d7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="353d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="353d7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="353d7-110">Child elements</span></span>

<span data-ttu-id="353d7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="353d7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="353d7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="353d7-112">Parent elements</span></span>

|<span data-ttu-id="353d7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="353d7-113">**Element**</span></span>|<span data-ttu-id="353d7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="353d7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="353d7-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="353d7-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="353d7-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="353d7-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="353d7-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="353d7-117">Text value</span></span>

<span data-ttu-id="353d7-118">Une valeur de texte qui représente un entier compris entre 0 et 100 est requise.</span><span class="sxs-lookup"><span data-stu-id="353d7-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="353d7-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="353d7-119">Remarks</span></span>

<span data-ttu-id="353d7-120">Paramètre **PercentComplete** à 100 a le même effet que la définition de l’élément [CompleteDate](completedate.md) ou la définition de l’élément [d’état](status.md) sur **terminée**.</span><span class="sxs-lookup"><span data-stu-id="353d7-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="353d7-121">Dans une demande qu’au moins deux jeux de ces propriétés, la dernière propriété traitée détermine la valeur est définie pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="353d7-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="353d7-122">Par exemple, si **PercentComplete** est 100, [CompleteDate](completedate.md) est le 1er janvier 2007, [l’état](status.md) est NotStarted et les propriétés sont transmises dans cet ordre, l’effet sera pour définir l' [état](status.md) de la tâche est NotStarted, le [ CompleteDate](completedate.md) **null**et le **PercentComplete** à 0.</span><span class="sxs-lookup"><span data-stu-id="353d7-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="353d7-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="353d7-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="353d7-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="353d7-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="353d7-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="353d7-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="353d7-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="353d7-126">Schema Name</span></span>  <br/> |<span data-ttu-id="353d7-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="353d7-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="353d7-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="353d7-128">Validation File</span></span>  <br/> |<span data-ttu-id="353d7-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="353d7-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="353d7-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="353d7-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="353d7-131">False</span><span class="sxs-lookup"><span data-stu-id="353d7-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="353d7-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="353d7-132">See also</span></span>



- [<span data-ttu-id="353d7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="353d7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="353d7-134">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="353d7-134">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="353d7-135">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="353d7-135">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

