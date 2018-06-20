---
title: EventCause (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- EventCause
api_type:
- schema
ms.assetid: 7b3c1db8-cad4-4050-a50d-b06f065db530
description: L’élément EventCause contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une demande de (service web de messagerie unifiée) opération GetCallInfo.
ms.openlocfilehash: dd73d93527bebb3b522ad0a6cdae5b9faee1a6a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756219"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="19b6c-103">EventCause (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-103">EventCause (UM web service)</span></span>

<span data-ttu-id="19b6c-104">L’élément **EventCause** contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="19b6c-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="19b6c-105">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="19b6c-106">EventCause (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="19b6c-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="19b6c-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19b6c-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="19b6c-108">Attributes and elements</span></span>

<span data-ttu-id="19b6c-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="19b6c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19b6c-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="19b6c-110">Attributes</span></span>

<span data-ttu-id="19b6c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19b6c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19b6c-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="19b6c-112">Child elements</span></span>

<span data-ttu-id="19b6c-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="19b6c-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="19b6c-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="19b6c-114">Parent elements</span></span>

|<span data-ttu-id="19b6c-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="19b6c-115">**Element**</span></span>|<span data-ttu-id="19b6c-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="19b6c-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19b6c-117">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="19b6c-118">Définit une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="19b6c-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="19b6c-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="19b6c-119">Text value</span></span>

<span data-ttu-id="19b6c-120">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="19b6c-120">A text value is required.</span></span> <span data-ttu-id="19b6c-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="19b6c-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="19b6c-122">Aucun</span><span class="sxs-lookup"><span data-stu-id="19b6c-122">None</span></span>
    
- <span data-ttu-id="19b6c-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="19b6c-123">UserBusy</span></span>
    
- <span data-ttu-id="19b6c-124">NoAnswer</span><span class="sxs-lookup"><span data-stu-id="19b6c-124">NoAnswer</span></span>
    
- <span data-ttu-id="19b6c-125">Other</span><span class="sxs-lookup"><span data-stu-id="19b6c-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="19b6c-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="19b6c-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19b6c-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="19b6c-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19b6c-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="19b6c-128">Schema Name</span></span>  <br/> |<span data-ttu-id="19b6c-129">Messages</span><span class="sxs-lookup"><span data-stu-id="19b6c-129">Messages</span></span>  <br/> |
|<span data-ttu-id="19b6c-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="19b6c-130">Validation File</span></span>  <br/> |<span data-ttu-id="19b6c-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="19b6c-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19b6c-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="19b6c-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="19b6c-133">False</span><span class="sxs-lookup"><span data-stu-id="19b6c-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19b6c-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="19b6c-134">See also</span></span>



[<span data-ttu-id="19b6c-135">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="19b6c-136">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="19b6c-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

