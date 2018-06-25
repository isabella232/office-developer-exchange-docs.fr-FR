---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: L’élément RetentionAction Spécifie l’action effectuée sur les éléments avec la balise de rétention.
ms.openlocfilehash: 54a1038f2e56aad66f89522423ccfbd69dc44a80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829215"
---
# <a name="retentionaction"></a><span data-ttu-id="e212d-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="e212d-103">RetentionAction</span></span>

<span data-ttu-id="e212d-104">L’élément **RetentionAction** Spécifie l’action effectuée sur les éléments avec la balise de rétention.</span><span class="sxs-lookup"><span data-stu-id="e212d-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="e212d-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="e212d-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e212d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e212d-106">Attributes and elements</span></span>

<span data-ttu-id="e212d-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e212d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e212d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e212d-108">Attributes</span></span>

<span data-ttu-id="e212d-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e212d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e212d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e212d-110">Child elements</span></span>

<span data-ttu-id="e212d-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e212d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e212d-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e212d-112">Parent elements</span></span>

[<span data-ttu-id="e212d-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="e212d-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="e212d-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e212d-114">Text value</span></span>

<span data-ttu-id="e212d-115">La valeur de texte de l’élément **RetentionAction** est l’action exécutée sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="e212d-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="e212d-116">La liste suivante contient les valeurs de texte de l’élément **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="e212d-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="e212d-117">**Aucun** - aucune action n’est effectuée sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="e212d-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="e212d-118">**MoveToDeletedItems** - l’élément est déplacé vers le dossier éléments supprimés par défaut.</span><span class="sxs-lookup"><span data-stu-id="e212d-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="e212d-119">**MoveToFolder** - l’élément est déplacé vers un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="e212d-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="e212d-120">**DeleteAndAllowRecovery** - l’élément est supprimé et placer dans la benne.</span><span class="sxs-lookup"><span data-stu-id="e212d-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="e212d-121">**PermanentlyDelete** - l’élément est définitivement supprimé de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e212d-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="e212d-122">**MarkAsPastRetentionLimit** - l’élément est marqué comme ayant dépassé la limite de temps de rétention.</span><span class="sxs-lookup"><span data-stu-id="e212d-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="e212d-123">**MoveToArchive** - l’élément est déplacé vers la boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="e212d-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="e212d-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="e212d-124">Remarks</span></span>

<span data-ttu-id="e212d-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e212d-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e212d-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e212d-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e212d-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e212d-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e212d-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e212d-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e212d-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e212d-129">Schema name</span></span>  <br/> |<span data-ttu-id="e212d-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e212d-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e212d-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e212d-131">Validation file</span></span>  <br/> |<span data-ttu-id="e212d-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e212d-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e212d-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e212d-133">Can be empty</span></span>  <br/> ||
   

