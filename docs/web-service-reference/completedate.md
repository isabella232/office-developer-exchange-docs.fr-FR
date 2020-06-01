---
title: Terminé
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteDate
api_type:
- schema
ms.assetid: b2b53b87-6a0b-4a55-bcfc-3bf67d3c1700
description: L’élément Completed représente la date à laquelle un élément a été terminé.
ms.openlocfilehash: fff3d5d3105bf63c9cdd34cbcf828d57ca287b86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461421"
---
# <a name="completedate"></a><span data-ttu-id="17796-103">Terminé</span><span class="sxs-lookup"><span data-stu-id="17796-103">CompleteDate</span></span>

<span data-ttu-id="17796-104">L’élément **Completed** représente la date à laquelle un élément a été terminé.</span><span class="sxs-lookup"><span data-stu-id="17796-104">The **CompleteDate** element represents the date on which an item was completed.</span></span> 
  
```xml
<CompleteDate/>
```

 <span data-ttu-id="17796-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="17796-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17796-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="17796-106">Attributes and elements</span></span>

<span data-ttu-id="17796-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="17796-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17796-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="17796-108">Attributes</span></span>

<span data-ttu-id="17796-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="17796-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="17796-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="17796-110">Child elements</span></span>

<span data-ttu-id="17796-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="17796-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17796-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="17796-112">Parent elements</span></span>

|<span data-ttu-id="17796-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="17796-113">**Element**</span></span>|<span data-ttu-id="17796-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="17796-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17796-115">Tâche</span><span class="sxs-lookup"><span data-stu-id="17796-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="17796-116">Représente une tâche dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="17796-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17796-117">Indicateur</span><span class="sxs-lookup"><span data-stu-id="17796-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="17796-118">Spécifie un indicateur sur un élément de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="17796-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17796-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="17796-119">Text value</span></span>

<span data-ttu-id="17796-120">Une valeur de texte qui représente la date et l’heure est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="17796-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17796-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="17796-121">Remarks</span></span>

<span data-ttu-id="17796-122">La définition de l’option **Completed** a le même effet que celle de la valeur de [PourcentageAchevé](percentcomplete.md) sur 100 ou l' [État](status.md) **terminé**.</span><span class="sxs-lookup"><span data-stu-id="17796-122">Setting **CompleteDate** has the same effect as setting [PercentComplete](percentcomplete.md) to 100 or [Status](status.md) to **Completed**.</span></span> <span data-ttu-id="17796-123">Dans une demande qui définit au moins deux de ces propriétés, la dernière propriété traitée détermine la valeur définie pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="17796-123">In a request that sets at least two of these properties, the last processed property will determine the value that is set for these elements.</span></span> <span data-ttu-id="17796-124">Par exemple, si [PercentComplete](percentcomplete.md) est 100, **recompleted** est le 1er janvier 2007 et [Status](status.md) est **NotStarted**, et que les propriétés sont diffusées dans cet ordre, l’effet est de définir l' [État](status.md) de la tâche sur **NotStarted**, la valeur de la propriété [Completed](completedate.md) sur **null**et [PercentComplete](percentcomplete.md) sur 0.</span><span class="sxs-lookup"><span data-stu-id="17796-124">For example, if [PercentComplete](percentcomplete.md) is 100, **CompleteDate** is January 1, 2007, and [Status](status.md) is **NotStarted**, and the properties are streamed in that order, the effect will be to set the [Status](status.md) of the task to **NotStarted**, the [CompleteDate](completedate.md) to **null**, and [PercentComplete](percentcomplete.md) to 0.</span></span> 
  
<span data-ttu-id="17796-125">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="17796-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17796-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="17796-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17796-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="17796-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17796-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="17796-128">Schema Name</span></span>  <br/> |<span data-ttu-id="17796-129">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="17796-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="17796-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="17796-130">Validation File</span></span>  <br/> |<span data-ttu-id="17796-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="17796-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17796-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="17796-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="17796-133">False</span><span class="sxs-lookup"><span data-stu-id="17796-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17796-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="17796-134">See also</span></span>



- [<span data-ttu-id="17796-135">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="17796-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="17796-136">Création de tâches</span><span class="sxs-lookup"><span data-stu-id="17796-136">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="17796-137">Suppression de tâches</span><span class="sxs-lookup"><span data-stu-id="17796-137">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

