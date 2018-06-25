---
title: PermanentDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: L’élément PermanentDelete indique si les messages doivent être définitivement supprimés et non enregistré dans le dossier éléments supprimés.
ms.openlocfilehash: 40cf80e054bb70a3f6d687e8d4361f1d4331a7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828724"
---
# <a name="permanentdelete"></a><span data-ttu-id="d1f41-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="d1f41-103">PermanentDelete</span></span>

<span data-ttu-id="d1f41-104">L’élément **PermanentDelete** indique si les messages doivent être définitivement supprimés et non enregistré dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="d1f41-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="d1f41-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d1f41-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1f41-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1f41-106">Attributes and elements</span></span>

<span data-ttu-id="d1f41-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1f41-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1f41-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1f41-108">Attributes</span></span>

<span data-ttu-id="d1f41-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1f41-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1f41-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1f41-110">Child elements</span></span>

<span data-ttu-id="d1f41-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d1f41-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1f41-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1f41-112">Parent elements</span></span>

|<span data-ttu-id="d1f41-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1f41-113">**Element**</span></span>|<span data-ttu-id="d1f41-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1f41-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1f41-115">Actions</span><span class="sxs-lookup"><span data-stu-id="d1f41-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="d1f41-116">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="d1f41-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1f41-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d1f41-117">Text value</span></span>

<span data-ttu-id="d1f41-118">Une valeur de texte de **la valeur true** indique que le message doit être marqué pour être définitivement supprimés.</span><span class="sxs-lookup"><span data-stu-id="d1f41-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="d1f41-119">La valeur **false** indique que le message ne doit pas être marqué pour être définitivement supprimés.</span><span class="sxs-lookup"><span data-stu-id="d1f41-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d1f41-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1f41-120">Remarks</span></span>

<span data-ttu-id="d1f41-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1f41-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1f41-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1f41-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1f41-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1f41-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1f41-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1f41-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d1f41-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d1f41-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1f41-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1f41-126">Validation File</span></span>  <br/> |<span data-ttu-id="d1f41-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d1f41-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1f41-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1f41-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1f41-129">True</span><span class="sxs-lookup"><span data-stu-id="d1f41-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1f41-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1f41-130">See also</span></span>



- [<span data-ttu-id="d1f41-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d1f41-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

