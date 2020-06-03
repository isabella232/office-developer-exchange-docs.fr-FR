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
ms.openlocfilehash: 5d022827990b96fd8790ae9566ef49028ebe404c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459958"
---
# <a name="status"></a><span data-ttu-id="f4f21-103">État</span><span class="sxs-lookup"><span data-stu-id="f4f21-103">Status</span></span>

<span data-ttu-id="f4f21-104">L’élément **Status** représente l’état d’un élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="f4f21-104">The **Status** element represents the status of a task item.</span></span> 
  
```xml
<Status/>
```

 <span data-ttu-id="f4f21-105">**TaskStatusType**</span><span class="sxs-lookup"><span data-stu-id="f4f21-105">**TaskStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f4f21-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f4f21-106">Attributes and elements</span></span>

<span data-ttu-id="f4f21-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f4f21-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f4f21-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f4f21-108">Attributes</span></span>

<span data-ttu-id="f4f21-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f4f21-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f4f21-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f4f21-110">Child elements</span></span>

<span data-ttu-id="f4f21-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f4f21-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f4f21-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f4f21-112">Parent elements</span></span>

|<span data-ttu-id="f4f21-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f4f21-113">**Element**</span></span>|<span data-ttu-id="f4f21-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f4f21-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f4f21-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="f4f21-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="f4f21-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="f4f21-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f4f21-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f4f21-117">Text value</span></span>

<span data-ttu-id="f4f21-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="f4f21-118">A text value is required.</span></span> <span data-ttu-id="f4f21-119">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="f4f21-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="f4f21-120">NotStarted</span><span class="sxs-lookup"><span data-stu-id="f4f21-120">NotStarted</span></span>
    
- <span data-ttu-id="f4f21-121">InProgress</span><span class="sxs-lookup"><span data-stu-id="f4f21-121">InProgress</span></span>
    
- <span data-ttu-id="f4f21-122">Achevé</span><span class="sxs-lookup"><span data-stu-id="f4f21-122">Completed</span></span>
    
- <span data-ttu-id="f4f21-123">WaitingOnOthers</span><span class="sxs-lookup"><span data-stu-id="f4f21-123">WaitingOnOthers</span></span>
    
- <span data-ttu-id="f4f21-124">Différé</span><span class="sxs-lookup"><span data-stu-id="f4f21-124">Deferred</span></span>
    
## <a name="remarks"></a><span data-ttu-id="f4f21-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="f4f21-125">Remarks</span></span>

<span data-ttu-id="f4f21-126">La définition de l’option [Completed](completedate.md) a le même effet que celle de la valeur de [PourcentageAchevé](percentcomplete.md) sur 100 ou l' **État** **terminé**.</span><span class="sxs-lookup"><span data-stu-id="f4f21-126">Setting [CompleteDate](completedate.md) has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or **Status** to **Completed**.</span></span> <span data-ttu-id="f4f21-127">Dans une demande qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="f4f21-127">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="f4f21-128">Par exemple, si **le PourcentageAchevé** est 100 **, si** la valeur de l' **État** est 1/1/2007, si l’État est NotStarted et si les propriétés sont diffusées en continu dans cet ordre, l’effet est de définir l’état de la tâche sur NotStarted, l' **État** **terminé** sur **null**et le **PourcentageAchevé** sur 0.</span><span class="sxs-lookup"><span data-stu-id="f4f21-128">For example, if **PercentComplete** is 100, **CompleteDate** is 1/1/2007, and **Status** is NotStarted, and the properties are streamed in this order, the effect will be to set the **Status** of the task to NotStarted, the **CompleteDate** to **null**, and the **PercentComplete** to 0.</span></span> 
  
<span data-ttu-id="f4f21-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f4f21-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f4f21-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f4f21-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f4f21-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f4f21-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f4f21-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f4f21-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f4f21-133">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f4f21-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f4f21-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f4f21-134">Validation File</span></span>  <br/> |<span data-ttu-id="f4f21-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f4f21-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f4f21-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f4f21-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f4f21-137">False</span><span class="sxs-lookup"><span data-stu-id="f4f21-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f4f21-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f4f21-138">See also</span></span>



- [<span data-ttu-id="f4f21-139">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f4f21-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f4f21-140">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="f4f21-140">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="f4f21-141">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="f4f21-141">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

