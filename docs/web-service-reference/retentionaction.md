---
title: RetentionAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3bdf5955-1212-48a1-b3b5-743086866c91
description: L’élément RetentionAction spécifie l’action effectuée sur les éléments à l’aide de la balise de rétention.
ms.openlocfilehash: c16988413e732ddc3cd6ebc355cb73c4d96550c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465232"
---
# <a name="retentionaction"></a><span data-ttu-id="f3645-103">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="f3645-103">RetentionAction</span></span>

<span data-ttu-id="f3645-104">L’élément **RetentionAction** spécifie l’action effectuée sur les éléments à l’aide de la balise de rétention.</span><span class="sxs-lookup"><span data-stu-id="f3645-104">The **RetentionAction** element specifies the action performed on items with the retention tag.</span></span> 
  
```XML
<RetentionAction> None | MoveToDeletedItems | MoveToFolder | DeleteAndAllowRecovery | PermanentlyDelete | MarkAsPastRetentionLimit | MoveToArchive <RetentionAction>
```

 <span data-ttu-id="f3645-105">**RetentionActionType**</span><span class="sxs-lookup"><span data-stu-id="f3645-105">**RetentionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3645-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f3645-106">Attributes and elements</span></span>

<span data-ttu-id="f3645-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f3645-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3645-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f3645-108">Attributes</span></span>

<span data-ttu-id="f3645-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f3645-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3645-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f3645-110">Child elements</span></span>

<span data-ttu-id="f3645-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f3645-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f3645-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f3645-112">Parent elements</span></span>

[<span data-ttu-id="f3645-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="f3645-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="f3645-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f3645-114">Text value</span></span>

<span data-ttu-id="f3645-115">La valeur de texte de l’élément **RetentionAction** est l’action effectuée sur les éléments.</span><span class="sxs-lookup"><span data-stu-id="f3645-115">The text value of the **RetentionAction** element is the action performed on items.</span></span> <span data-ttu-id="f3645-116">La liste suivante contient les valeurs de texte de l’élément **RetentionAction** .</span><span class="sxs-lookup"><span data-stu-id="f3645-116">The following list contains the text values for the **RetentionAction** element.</span></span> 
  
> <span data-ttu-id="f3645-117">**None** : aucune action n’est effectuée sur l’élément.</span><span class="sxs-lookup"><span data-stu-id="f3645-117">**None** - No action is performed on the item.</span></span> 
    
> <span data-ttu-id="f3645-118">**MoveToDeletedItems** -l’élément est déplacé vers le dossier éléments supprimés par défaut.</span><span class="sxs-lookup"><span data-stu-id="f3645-118">**MoveToDeletedItems** - The item is moved to the default Deleted Items folder.</span></span> 
    
> <span data-ttu-id="f3645-119">**MoveToFolder** : l’élément est déplacé vers un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="f3645-119">**MoveToFolder** - The item is moved to a specified folder.</span></span> 
    
> <span data-ttu-id="f3645-120">**DeleteAndAllowRecovery** : l’élément est supprimé et placé dans la benne.</span><span class="sxs-lookup"><span data-stu-id="f3645-120">**DeleteAndAllowRecovery** - The item is deleted and put into the Dumpster.</span></span> 
    
> <span data-ttu-id="f3645-121">**PermanentlyDelete** : l’élément est définitivement supprimé de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f3645-121">**PermanentlyDelete** - The item is permanently deleted from the mailbox.</span></span> 
    
> <span data-ttu-id="f3645-122">**MarkAsPastRetentionLimit** -l’élément est marqué comme ayant dépassé la limite de temps de rétention.</span><span class="sxs-lookup"><span data-stu-id="f3645-122">**MarkAsPastRetentionLimit** - The item is marked as having exceeded the retention time limit.</span></span> 
    
> <span data-ttu-id="f3645-123">**MoveToArchive** : l’élément est déplacé vers la boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="f3645-123">**MoveToArchive** - The item is moved to the archive mailbox.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="f3645-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="f3645-124">Remarks</span></span>

<span data-ttu-id="f3645-125">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f3645-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f3645-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3645-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3645-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f3645-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3645-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f3645-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f3645-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f3645-129">Schema name</span></span>  <br/> |<span data-ttu-id="f3645-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f3645-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f3645-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f3645-131">Validation file</span></span>  <br/> |<span data-ttu-id="f3645-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f3645-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f3645-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f3645-133">Can be empty</span></span>  <br/> ||
   

