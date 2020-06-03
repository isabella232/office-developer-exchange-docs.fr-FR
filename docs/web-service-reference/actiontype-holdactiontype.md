---
title: ActionType (HoldActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f50449b9-e73b-43c5-af96-6433bf434dce
description: L’élément ActionType indique le type d’action pour la suspension.
ms.openlocfilehash: 8f2796df818dac2bd285b055aa44fbcecd0de5e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457857"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="647ae-103">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="647ae-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="647ae-104">L’élément **ActionType** indique le type d’action pour la suspension.</span><span class="sxs-lookup"><span data-stu-id="647ae-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="647ae-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="647ae-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="647ae-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="647ae-106">Attributes and elements</span></span>

<span data-ttu-id="647ae-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="647ae-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="647ae-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="647ae-108">Attributes</span></span>

<span data-ttu-id="647ae-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="647ae-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="647ae-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="647ae-110">Child elements</span></span>

<span data-ttu-id="647ae-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="647ae-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="647ae-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="647ae-112">Parent elements</span></span>

[<span data-ttu-id="647ae-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="647ae-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="647ae-114">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="647ae-114">Text value</span></span>

<span data-ttu-id="647ae-115">La valeur de texte de l’élément **ActionType** correspond au type de suspension défini dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="647ae-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="647ae-116">Une valeur de texte de **Create** indique qu’une conservation de boîte aux lettres est créée.</span><span class="sxs-lookup"><span data-stu-id="647ae-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="647ae-117">Une valeur de texte de **mise à jour** indique qu’une conservation de boîte aux lettres est mise à jour.</span><span class="sxs-lookup"><span data-stu-id="647ae-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="647ae-118">Une valeur de texte de **suppression** indique qu’une conservation de boîte aux lettres est supprimée.</span><span class="sxs-lookup"><span data-stu-id="647ae-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="647ae-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="647ae-119">Remarks</span></span>

<span data-ttu-id="647ae-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="647ae-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="647ae-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="647ae-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="647ae-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="647ae-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="647ae-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="647ae-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="647ae-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="647ae-124">Schema name</span></span>  <br/> |<span data-ttu-id="647ae-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="647ae-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="647ae-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="647ae-126">Validation file</span></span>  <br/> |<span data-ttu-id="647ae-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="647ae-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="647ae-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="647ae-128">Can be empty</span></span>  <br/> |<span data-ttu-id="647ae-129">false</span><span class="sxs-lookup"><span data-stu-id="647ae-129">false</span></span>  <br/> |
   

