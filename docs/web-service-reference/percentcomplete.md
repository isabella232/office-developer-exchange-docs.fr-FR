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
ms.openlocfilehash: b7dd2f18bd3ef6addeb6d3a7b004510f35b9cb3d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456884"
---
# <a name="percentcomplete"></a><span data-ttu-id="e1020-103">PercentComplete</span><span class="sxs-lookup"><span data-stu-id="e1020-103">PercentComplete</span></span>

<span data-ttu-id="e1020-104">L’élément **PercentComplete** décrit l’état d’achèvement d’une tâche.</span><span class="sxs-lookup"><span data-stu-id="e1020-104">The **PercentComplete** element describes the completion status of a task.</span></span> 
  
```xml
<PercentComplete/>
```

 <span data-ttu-id="e1020-105">**fois**</span><span class="sxs-lookup"><span data-stu-id="e1020-105">**double**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1020-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e1020-106">Attributes and elements</span></span>

<span data-ttu-id="e1020-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e1020-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1020-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e1020-108">Attributes</span></span>

<span data-ttu-id="e1020-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="e1020-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1020-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e1020-110">Child elements</span></span>

<span data-ttu-id="e1020-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e1020-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1020-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e1020-112">Parent elements</span></span>

|<span data-ttu-id="e1020-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="e1020-113">**Element**</span></span>|<span data-ttu-id="e1020-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="e1020-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1020-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="e1020-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="e1020-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="e1020-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1020-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="e1020-117">Text value</span></span>

<span data-ttu-id="e1020-118">Une valeur de texte qui représente un entier compris entre 0 et 100 est requise.</span><span class="sxs-lookup"><span data-stu-id="e1020-118">A text value that represents an integer between 0 and 100 is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1020-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="e1020-119">Remarks</span></span>

<span data-ttu-id="e1020-120">La définition de **PercentComplete** sur 100 a le même effet que la définition de l’élément [Completed](completedate.md) , ou la définition de l’élément [Status](status.md) sur **Completed**.</span><span class="sxs-lookup"><span data-stu-id="e1020-120">Setting **PercentComplete** to 100 has the same effect as setting the [CompleteDate](completedate.md) element or setting the [Status](status.md) element to **Completed**.</span></span> <span data-ttu-id="e1020-121">Dans une demande qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="e1020-121">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="e1020-122">Par exemple, si **PercentComplete** a la valeur 100, [recompleted](completedate.md) est le 1er janvier 2007 et [Status](status.md) is NotStarted, et que les propriétés sont diffusées dans cet ordre, l’effet est de définir l' [État](status.md) de la tâche sur NotStarted, le paramètre [Completed](completedate.md) sur **null**et le **PourcentageAchevé** sur 0.</span><span class="sxs-lookup"><span data-stu-id="e1020-122">For example, if **PercentComplete** is 100, [CompleteDate](completedate.md) is January 1, 2007, and [Status](status.md) is NotStarted, and the properties are streamed in this order, the effect will be to set the [Status](status.md) of the task to NotStarted, the [CompleteDate](completedate.md) to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="e1020-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="e1020-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1020-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e1020-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1020-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e1020-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1020-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e1020-126">Schema Name</span></span>  <br/> |<span data-ttu-id="e1020-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e1020-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1020-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e1020-128">Validation File</span></span>  <br/> |<span data-ttu-id="e1020-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e1020-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1020-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e1020-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1020-131">False</span><span class="sxs-lookup"><span data-stu-id="e1020-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1020-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e1020-132">See also</span></span>



- [<span data-ttu-id="e1020-133">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e1020-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="e1020-134">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="e1020-134">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="e1020-135">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="e1020-135">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

