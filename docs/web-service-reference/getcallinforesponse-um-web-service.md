---
title: GetCallInfoResponse (service Web de messagerie unifiée)
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
description: L’élément GetCallInfoResponse définit une réponse à une opération GetCallInfo (service Web de messagerie unifiée).
ms.openlocfilehash: 6e54ec61a9a5ebecd96bbd39dad68f8cc011b8a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461204"
---
# <a name="getcallinforesponse-um-web-service"></a><span data-ttu-id="87753-103">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="87753-103">GetCallInfoResponse (UM web service)</span></span>

<span data-ttu-id="87753-104">L’élément **GetCallInfoResponse** définit une réponse à une [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="87753-104">The **GetCallInfoResponse** element defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="87753-105">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="87753-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <CallState/>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="87753-106">**UMCallInfo**</span><span class="sxs-lookup"><span data-stu-id="87753-106">**UMCallInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87753-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="87753-107">Attributes and elements</span></span>

<span data-ttu-id="87753-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="87753-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87753-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="87753-109">Attributes</span></span>

<span data-ttu-id="87753-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="87753-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87753-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="87753-111">Child elements</span></span>

|<span data-ttu-id="87753-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="87753-112">**Element**</span></span>|<span data-ttu-id="87753-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="87753-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="87753-114">CallState</span><span class="sxs-lookup"><span data-stu-id="87753-114">CallState</span></span>  <br/> |<span data-ttu-id="87753-115">Contient une valeur qui indique l’état d’un appel pour lequel l' [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) a demandé des informations.</span><span class="sxs-lookup"><span data-stu-id="87753-115">Contains a value that indicates the status of a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
|<span data-ttu-id="87753-116">EventCause</span><span class="sxs-lookup"><span data-stu-id="87753-116">EventCause</span></span>  <br/> |<span data-ttu-id="87753-117">Contient une valeur qui indique la cause d’un événement pour un appel pour lequel l' [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) a demandé des informations.</span><span class="sxs-lookup"><span data-stu-id="87753-117">Contains a value that indicates the cause of an event for a call for which the [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) requested information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87753-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="87753-118">Parent elements</span></span>

<span data-ttu-id="87753-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="87753-119">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="87753-120">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="87753-120">Text value</span></span>

<span data-ttu-id="87753-121">Aucune.</span><span class="sxs-lookup"><span data-stu-id="87753-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87753-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="87753-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87753-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="87753-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87753-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="87753-124">Schema Name</span></span>  <br/> |<span data-ttu-id="87753-125">Messages</span><span class="sxs-lookup"><span data-stu-id="87753-125">Messages</span></span>  <br/> |
|<span data-ttu-id="87753-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="87753-126">Validation File</span></span>  <br/> |<span data-ttu-id="87753-127">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="87753-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87753-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="87753-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="87753-129">False</span><span class="sxs-lookup"><span data-stu-id="87753-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87753-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="87753-130">See also</span></span>



[<span data-ttu-id="87753-131">Opération GetCallInfo (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="87753-131">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="87753-132">CallState (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="87753-132">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="87753-133">EventCause (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="87753-133">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

