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
description: L’élément HasBeenProcessed indique si un élément de message de réunion a été traité.
ms.openlocfilehash: 7251ca86e07a0b72c186c65094b6469331dfd12e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462892"
---
# <a name="hasbeenprocessed"></a><span data-ttu-id="05da6-103">HasBeenProcessed</span><span class="sxs-lookup"><span data-stu-id="05da6-103">HasBeenProcessed</span></span>

<span data-ttu-id="05da6-104">L’élément **HasBeenProcessed** indique si un élément de message de réunion a été traité.</span><span class="sxs-lookup"><span data-stu-id="05da6-104">The **HasBeenProcessed** element indicates whether a meeting message item has been processed.</span></span> 
  
```xml
<HasBeenProcessed/>
```

 <span data-ttu-id="05da6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="05da6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="05da6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="05da6-106">Attributes and elements</span></span>

<span data-ttu-id="05da6-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="05da6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="05da6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="05da6-108">Attributes</span></span>

<span data-ttu-id="05da6-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="05da6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="05da6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="05da6-110">Child elements</span></span>

<span data-ttu-id="05da6-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="05da6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="05da6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="05da6-112">Parent elements</span></span>

|<span data-ttu-id="05da6-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="05da6-113">**Element**</span></span>|<span data-ttu-id="05da6-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="05da6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="05da6-115">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="05da6-115">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="05da6-116">Représente une annulation de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05da6-116">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05da6-117">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="05da6-117">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="05da6-118">Représente une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05da6-118">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05da6-119">Propriété meetingrequest</span><span class="sxs-lookup"><span data-stu-id="05da6-119">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="05da6-120">Représente une demande de réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05da6-120">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="05da6-121">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="05da6-121">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="05da6-122">Représente une réponse à une réunion dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="05da6-122">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="05da6-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="05da6-123">Text value</span></span>

<span data-ttu-id="05da6-124">Une valeur de texte **true** indique que le message de réunion a été traité.</span><span class="sxs-lookup"><span data-stu-id="05da6-124">A text value of **true** indicates that the meeting message has been processed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="05da6-125">Remarques</span><span class="sxs-lookup"><span data-stu-id="05da6-125">Remarks</span></span>

<span data-ttu-id="05da6-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="05da6-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="05da6-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="05da6-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="05da6-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="05da6-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="05da6-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="05da6-129">Schema Name</span></span>  <br/> |<span data-ttu-id="05da6-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="05da6-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="05da6-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="05da6-131">Validation File</span></span>  <br/> |<span data-ttu-id="05da6-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="05da6-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="05da6-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="05da6-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="05da6-134">False</span><span class="sxs-lookup"><span data-stu-id="05da6-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="05da6-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="05da6-135">See also</span></span>



- [<span data-ttu-id="05da6-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="05da6-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

