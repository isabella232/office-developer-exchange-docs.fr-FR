---
title: ServerReplyWithMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerReplyWithMessage
api_type:
- schema
ms.assetid: 113c6ff2-9592-44f0-b542-54e4d5122ccb
description: L’élément ServerReplyWithMessage indique l’ID de modèle de message qui doit être envoyé en réponse aux messages entrants.
ms.openlocfilehash: f2d927ae18ac68523d4cdd173f0474fbbeb36c98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829390"
---
# <a name="serverreplywithmessage"></a><span data-ttu-id="d0d29-103">ServerReplyWithMessage</span><span class="sxs-lookup"><span data-stu-id="d0d29-103">ServerReplyWithMessage</span></span>

<span data-ttu-id="d0d29-104">L’élément **ServerReplyWithMessage** indique l’ID de modèle de message qui doit être envoyé en réponse aux messages entrants.</span><span class="sxs-lookup"><span data-stu-id="d0d29-104">The **ServerReplyWithMessage** element indicates the ID of the template message that is to be sent as a reply to incoming messages.</span></span> 
  
```XML
<ServerReplyWithMessage>
    <ItemId>
</ServerReplyWithMessage>
```

 <span data-ttu-id="d0d29-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="d0d29-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0d29-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d0d29-106">Attributes and elements</span></span>

<span data-ttu-id="d0d29-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d0d29-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0d29-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d0d29-108">Attributes</span></span>

<span data-ttu-id="d0d29-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0d29-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0d29-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d0d29-110">Child elements</span></span>

|<span data-ttu-id="d0d29-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0d29-111">**Element**</span></span>|<span data-ttu-id="d0d29-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0d29-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0d29-113">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="d0d29-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d0d29-114">Représente la clé unique identificateur et modification d’un élément dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0d29-114">Represents the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0d29-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d0d29-115">Parent elements</span></span>

|<span data-ttu-id="d0d29-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d0d29-116">**Element**</span></span>|<span data-ttu-id="d0d29-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d0d29-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0d29-118">Actions</span><span class="sxs-lookup"><span data-stu-id="d0d29-118">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="d0d29-119">Représente l'ensemble des actions qui sont disponibles pour être effectuées sur un message lorsque les conditions sont remplies.</span><span class="sxs-lookup"><span data-stu-id="d0d29-119">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0d29-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d0d29-120">Text value</span></span>

<span data-ttu-id="d0d29-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d0d29-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0d29-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="d0d29-122">Remarks</span></span>

<span data-ttu-id="d0d29-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d0d29-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0d29-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d0d29-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0d29-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d0d29-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d0d29-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d0d29-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d0d29-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d0d29-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d0d29-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d0d29-128">Validation File</span></span>  <br/> |<span data-ttu-id="d0d29-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d0d29-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d0d29-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d0d29-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0d29-131">True</span><span class="sxs-lookup"><span data-stu-id="d0d29-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0d29-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d0d29-132">See also</span></span>



- [<span data-ttu-id="d0d29-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d0d29-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

