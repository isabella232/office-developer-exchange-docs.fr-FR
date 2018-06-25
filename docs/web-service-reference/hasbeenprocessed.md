---
title: HasBeenProcessed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasBeenProcessed
api_type:
- schema
ms.assetid: 46d4af8e-0f11-4a74-9365-1d983731fed8
description: L’élément HasBeenProcessed indique si un message de réunion élément a été traité.
ms.openlocfilehash: cccd3b2258490fcbe902bcd391f25b0be2fe7c26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827796"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="1dd7a-103">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="1dd7a-103">HasBeenProcessed</span></span>

<span data-ttu-id="1dd7a-104">L’élément **HasBeenProcessed** indique si un message de réunion élément a été traité.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="1dd7a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="1dd7a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1dd7a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1dd7a-106">Attributes and elements</span></span>

<span data-ttu-id="1dd7a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1dd7a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1dd7a-108">Attributes</span></span>

<span data-ttu-id="1dd7a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1dd7a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1dd7a-110">Child elements</span></span>

<span data-ttu-id="1dd7a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1dd7a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1dd7a-112">Parent elements</span></span>

|<span data-ttu-id="1dd7a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1dd7a-113">**Element**</span></span>|<span data-ttu-id="1dd7a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1dd7a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1dd7a-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="1dd7a-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="1dd7a-116">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1dd7a-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="1dd7a-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="1dd7a-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1dd7a-119">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1dd7a-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="1dd7a-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="1dd7a-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="1dd7a-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="1dd7a-122">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1dd7a-123">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1dd7a-123">Text value</span></span>

<span data-ttu-id="1dd7a-124">Une valeur de texte de **la valeur true** indique que le message de réunion a été traité.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1dd7a-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="1dd7a-125">Remarks</span></span>

<span data-ttu-id="1dd7a-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1dd7a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1dd7a-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1dd7a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1dd7a-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1dd7a-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1dd7a-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1dd7a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1dd7a-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="1dd7a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="1dd7a-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1dd7a-131">Validation File</span></span>  <br/> |<span data-ttu-id="1dd7a-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1dd7a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1dd7a-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1dd7a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1dd7a-134">False</span><span class="sxs-lookup"><span data-stu-id="1dd7a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1dd7a-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1dd7a-135">See also</span></span>



- [<span data-ttu-id="1dd7a-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1dd7a-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

