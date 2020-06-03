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
description: L’élément MarkAsRead indique si les messages doivent être marqués comme lus.
ms.openlocfilehash: 691409a4eace8885d36f4b30b8eef1aca8c332a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461764"
---
# <a name="markasread"></a><span data-ttu-id="3a32b-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="3a32b-103">MarkAsRead</span></span>

<span data-ttu-id="3a32b-104">L’élément **MarkAsRead** indique si les messages doivent être marqués comme lus.</span><span class="sxs-lookup"><span data-stu-id="3a32b-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="3a32b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3a32b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a32b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="3a32b-106">Attributes and elements</span></span>

<span data-ttu-id="3a32b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="3a32b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a32b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="3a32b-108">Attributes</span></span>

<span data-ttu-id="3a32b-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="3a32b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a32b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="3a32b-110">Child elements</span></span>

<span data-ttu-id="3a32b-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="3a32b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3a32b-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="3a32b-112">Parent elements</span></span>

|<span data-ttu-id="3a32b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3a32b-113">**Element**</span></span>|<span data-ttu-id="3a32b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="3a32b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a32b-115">Actions</span><span class="sxs-lookup"><span data-stu-id="3a32b-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="3a32b-116">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="3a32b-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a32b-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="3a32b-117">Text value</span></span>

<span data-ttu-id="3a32b-118">Une valeur de texte **true** indique que le message doit être marqué comme lu.</span><span class="sxs-lookup"><span data-stu-id="3a32b-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="3a32b-119">La valeur **false** indique que les messages ne doivent pas être marqués comme lus.</span><span class="sxs-lookup"><span data-stu-id="3a32b-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3a32b-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="3a32b-120">Remarks</span></span>

<span data-ttu-id="3a32b-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="3a32b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a32b-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="3a32b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a32b-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="3a32b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3a32b-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="3a32b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="3a32b-125">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="3a32b-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3a32b-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="3a32b-126">Validation File</span></span>  <br/> |<span data-ttu-id="3a32b-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="3a32b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3a32b-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="3a32b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="3a32b-129">True</span><span class="sxs-lookup"><span data-stu-id="3a32b-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3a32b-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3a32b-130">See also</span></span>



- [<span data-ttu-id="3a32b-131">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3a32b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

