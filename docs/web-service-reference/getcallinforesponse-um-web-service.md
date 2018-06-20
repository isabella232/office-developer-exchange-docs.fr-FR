---
title: GetCallInfoResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfoResponse
api_type:
- schema
ms.assetid: aa5196bf-f5f3-455c-94ea-304fb7920c79
description: L’élément GetCallInfoResponse définit une réponse à une demande de (service web de messagerie unifiée) opération GetCallInfo.
ms.openlocfilehash: d9658dd9cb47f925e05dc21a8651c98dce1f0a2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756537"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="4d94f-103">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d94f-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="4d94f-104">L’élément **GetCallInfoResponse** définit une réponse à une demande de [l’opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="4d94f-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="4d94f-105">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d94f-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="4d94f-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="4d94f-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d94f-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4d94f-107">Attributes and elements</span></span>

<span data-ttu-id="4d94f-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4d94f-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d94f-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="4d94f-109">Attributes</span></span>

<span data-ttu-id="4d94f-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d94f-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d94f-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4d94f-111">Child elements</span></span>

|<span data-ttu-id="4d94f-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4d94f-112">**Element**</span></span>|<span data-ttu-id="4d94f-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="4d94f-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4d94f-114">CallState</span><span class="sxs-lookup"><span data-stu-id="4d94f-114">CallState</span></span>  <br/> |<span data-ttu-id="4d94f-115">Contient une valeur qui indique l’état d’un appel pour lequel l' [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) les informations demandées.</span><span class="sxs-lookup"><span data-stu-id="4d94f-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="4d94f-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="4d94f-116">EventCause</span></span>  <br/> |<span data-ttu-id="4d94f-117">Contient une valeur qui indique la cause d’un événement pour un appel pour lequel l' [opération GetCallInfo (service web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) les informations demandées.</span><span class="sxs-lookup"><span data-stu-id="4d94f-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d94f-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4d94f-118">Parent elements</span></span>

<span data-ttu-id="4d94f-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d94f-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4d94f-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4d94f-120">Text value</span></span>

<span data-ttu-id="4d94f-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4d94f-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d94f-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4d94f-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d94f-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4d94f-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4d94f-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4d94f-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4d94f-125">Messages</span><span class="sxs-lookup"><span data-stu-id="4d94f-125">Messages</span></span>  <br/> |
|<span data-ttu-id="4d94f-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4d94f-126">Validation File</span></span>  <br/> |<span data-ttu-id="4d94f-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4d94f-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4d94f-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4d94f-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d94f-129">False</span><span class="sxs-lookup"><span data-stu-id="4d94f-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d94f-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4d94f-130">See also</span></span>



[<span data-ttu-id="4d94f-131">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d94f-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="4d94f-132">CallState (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d94f-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="4d94f-133">EventCause (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4d94f-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

