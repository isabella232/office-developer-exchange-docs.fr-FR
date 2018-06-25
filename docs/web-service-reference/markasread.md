---
title: MarkAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkAsRead
api_type:
- schema
ms.assetid: 404842e1-fbdb-480d-a1d8-ba1ab2c9fb1e
description: L’élément MarkAsRead indique si les messages doivent être marqués comme étant en lecture.
ms.openlocfilehash: b453ad73912e99b6fd3aed84b03a7d2fc2b6a294
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828355"
---
# <a name="markasread"></a><span data-ttu-id="7d248-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="7d248-103">MarkAsRead</span></span>

<span data-ttu-id="7d248-104">L’élément **MarkAsRead** indique si les messages doivent être marqués comme étant en lecture.</span><span class="sxs-lookup"><span data-stu-id="7d248-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="7d248-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="7d248-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d248-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="7d248-106">Attributes and elements</span></span>

<span data-ttu-id="7d248-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="7d248-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d248-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="7d248-108">Attributes</span></span>

<span data-ttu-id="7d248-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d248-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d248-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="7d248-110">Child elements</span></span>

<span data-ttu-id="7d248-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="7d248-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7d248-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="7d248-112">Parent elements</span></span>

|<span data-ttu-id="7d248-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7d248-113">**Element**</span></span>|<span data-ttu-id="7d248-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="7d248-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d248-115">Actions</span><span class="sxs-lookup"><span data-stu-id="7d248-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="7d248-116">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="7d248-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7d248-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="7d248-117">Text value</span></span>

<span data-ttu-id="7d248-118">Une valeur de texte de **la valeur true** indique que le message doit être marqué comme lu.</span><span class="sxs-lookup"><span data-stu-id="7d248-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="7d248-119">La valeur **false** indique que les messages ne doivent pas être marqués comme lus.</span><span class="sxs-lookup"><span data-stu-id="7d248-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7d248-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="7d248-120">Remarks</span></span>

<span data-ttu-id="7d248-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d248-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d248-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="7d248-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d248-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="7d248-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7d248-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="7d248-124">Schema Name</span></span>  <br/> |<span data-ttu-id="7d248-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="7d248-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7d248-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="7d248-126">Validation File</span></span>  <br/> |<span data-ttu-id="7d248-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7d248-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7d248-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="7d248-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="7d248-129">True</span><span class="sxs-lookup"><span data-stu-id="7d248-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d248-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7d248-130">See also</span></span>



- [<span data-ttu-id="7d248-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7d248-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

