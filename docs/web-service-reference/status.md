---
title: État
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 80121e41-291b-4fc0-a55e-6f677d4b5fb5
description: L’élément Status représente l’état d’un élément de tâche.
ms.openlocfilehash: 224b61913a5ae8e5b4aa0d756a9f2488df2741bd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829584"
---
# <a name="status"></a><span data-ttu-id="fb45b-103">État</span><span class="sxs-lookup"><span data-stu-id="fb45b-103">Status</span></span>

<span data-ttu-id="fb45b-104">L’élément **Status** représente l’état d’un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="fb45b-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="fb45b-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="fb45b-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb45b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="fb45b-106">Attributes and elements</span></span>

<span data-ttu-id="fb45b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="fb45b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb45b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="fb45b-108">Attributes</span></span>

<span data-ttu-id="fb45b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb45b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb45b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="fb45b-110">Child elements</span></span>

<span data-ttu-id="fb45b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="fb45b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb45b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="fb45b-112">Parent elements</span></span>

|<span data-ttu-id="fb45b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="fb45b-113">**Element**</span></span>|<span data-ttu-id="fb45b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="fb45b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fb45b-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="fb45b-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="fb45b-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="fb45b-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fb45b-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="fb45b-117">Text value</span></span>

<span data-ttu-id="fb45b-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="fb45b-118">A text value is required.</span></span> <span data-ttu-id="fb45b-119">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="fb45b-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="fb45b-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="fb45b-120">NotStarted</span></span>
    
- <span data-ttu-id="fb45b-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="fb45b-121">InProgress</span></span>
    
- <span data-ttu-id="fb45b-122">Achevé</span><span class="sxs-lookup"><span data-stu-id="fb45b-122">Completed</span></span>
    
- <span data-ttu-id="fb45b-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="fb45b-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="fb45b-124">Différé</span><span class="sxs-lookup"><span data-stu-id="fb45b-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="fb45b-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="fb45b-125">Remarks</span></span>

<span data-ttu-id="fb45b-126">Définition de [CompleteDate](completedate.md) a le même effet que la définition [PercentComplete](percentcomplete.md) à 100 ou **état** sur **terminée**.</span><span class="sxs-lookup"><span data-stu-id="fb45b-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="fb45b-127">Dans une demande qu’au moins deux jeux de ces propriétés, la dernière propriété traitée détermine la valeur est définie pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="fb45b-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="fb45b-128">Par exemple, si **PercentComplete** est 100, **CompleteDate** est 1/1/2007 et **l’état** est NotStarted et les propriétés sont transmises dans l’ordre suivant, l’effet sera pour définir l' **état** de la tâche est NotStarted, la **CompleteDate ** **null**et le **PercentComplete** à 0.</span><span class="sxs-lookup"><span data-stu-id="fb45b-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="fb45b-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="fb45b-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb45b-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="fb45b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb45b-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="fb45b-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb45b-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="fb45b-132">Schema Name</span></span>  <br/> |<span data-ttu-id="fb45b-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="fb45b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb45b-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="fb45b-134">Validation File</span></span>  <br/> |<span data-ttu-id="fb45b-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fb45b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb45b-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="fb45b-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="fb45b-137">False</span><span class="sxs-lookup"><span data-stu-id="fb45b-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fb45b-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="fb45b-138">See also</span></span>



- [<span data-ttu-id="fb45b-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="fb45b-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="fb45b-140">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="fb45b-140">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="fb45b-141">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="fb45b-141">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

