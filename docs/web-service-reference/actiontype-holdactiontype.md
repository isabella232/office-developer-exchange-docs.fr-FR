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
ms.openlocfilehash: cb1cfa8a1306c4a6cacf5c82824d19cab57e7941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755152"
---
# <a name="actiontype-holdactiontype"></a><span data-ttu-id="82279-103">ActionType (HoldActionType)</span><span class="sxs-lookup"><span data-stu-id="82279-103">ActionType (HoldActionType)</span></span>

<span data-ttu-id="82279-104">L’élément **ActionType** indique le type d’action pour la suspension.</span><span class="sxs-lookup"><span data-stu-id="82279-104">The **ActionType** element indicates the type of action for the hold.</span></span> 
  
```XML
<ActionType> Create | Update | Remove </ActionType>
```

 <span data-ttu-id="82279-105">**HoldActionType**</span><span class="sxs-lookup"><span data-stu-id="82279-105">**HoldActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82279-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="82279-106">Attributes and elements</span></span>

<span data-ttu-id="82279-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="82279-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82279-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="82279-108">Attributes</span></span>

<span data-ttu-id="82279-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="82279-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82279-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="82279-110">Child elements</span></span>

<span data-ttu-id="82279-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="82279-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82279-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="82279-112">Parent elements</span></span>

[<span data-ttu-id="82279-113">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="82279-113">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
  
## <a name="text-value"></a><span data-ttu-id="82279-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="82279-114">Text value</span></span>

<span data-ttu-id="82279-115">La valeur de texte de l’élément **ActionType** est le type de suspension définir une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="82279-115">The text value of the **ActionType** element is the type of hold set on a mailbox.</span></span> <span data-ttu-id="82279-116">**Créer** la valeur texte indique qu’une suspension de boîte aux lettres sera créée.</span><span class="sxs-lookup"><span data-stu-id="82279-116">A text value of **Create** indicates that a mailbox hold will be created.</span></span> <span data-ttu-id="82279-117">Une valeur de texte de **mise à jour** indique qu’une boîte aux lettres de suspension est mis à jour.</span><span class="sxs-lookup"><span data-stu-id="82279-117">A text value of **Update** indicates that a mailbox hold will be updated.</span></span> <span data-ttu-id="82279-118">**Supprimer** la valeur texte indique qu’une boîte aux lettres de suspension est supprimée.</span><span class="sxs-lookup"><span data-stu-id="82279-118">A text value of **Remove** indicates that a mailbox hold will be removed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="82279-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="82279-119">Remarks</span></span>

<span data-ttu-id="82279-120">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="82279-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="82279-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="82279-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82279-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="82279-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82279-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="82279-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82279-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="82279-124">Schema name</span></span>  <br/> |<span data-ttu-id="82279-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="82279-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="82279-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="82279-126">Validation file</span></span>  <br/> |<span data-ttu-id="82279-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="82279-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82279-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="82279-128">Can be empty</span></span>  <br/> |<span data-ttu-id="82279-129">false</span><span class="sxs-lookup"><span data-stu-id="82279-129">false</span></span>  <br/> |
   

