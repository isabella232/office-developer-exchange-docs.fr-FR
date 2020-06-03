---
title: EventCause (service Web de messagerie unifiée)
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
description: L’élément EventCause contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une opération GetCallInfo (service Web de messagerie unifiée).
ms.openlocfilehash: 9d49fd4b16236d0dd87889fbbd039f2e271a5968
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458676"
---
# <a name="eventcause-um-web-service"></a><span data-ttu-id="50829-103">EventCause (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-103">EventCause (UM web service)</span></span>

<span data-ttu-id="50829-104">L’élément **EventCause** contient une valeur qui indique la cause d’un événement d’appel dans une réponse à une [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="50829-104">The **EventCause** element contains a value that indicates the cause for a call event in a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="50829-105">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-105">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="50829-106">EventCause (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-106">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)
  
```xml
<GetCallInfoResponse>
  <EventCause/>
</GetCallInfoResponse>
```

 <span data-ttu-id="50829-107">**UMEventCause**</span><span class="sxs-lookup"><span data-stu-id="50829-107">**UMEventCause**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="50829-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="50829-108">Attributes and elements</span></span>

<span data-ttu-id="50829-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="50829-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50829-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="50829-110">Attributes</span></span>

<span data-ttu-id="50829-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="50829-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50829-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="50829-112">Child elements</span></span>

<span data-ttu-id="50829-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="50829-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="50829-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="50829-114">Parent elements</span></span>

|<span data-ttu-id="50829-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50829-115">**Element**</span></span>|<span data-ttu-id="50829-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="50829-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50829-117">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-117">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md) <br/> |<span data-ttu-id="50829-118">Définit une réponse à une [opération GetCallInfo (service Web de messagerie unifiée)](getcallinfo-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="50829-118">Defines a response to a [GetCallInfo operation (UM web service)](getcallinfo-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="50829-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="50829-119">Text value</span></span>

<span data-ttu-id="50829-120">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="50829-120">A text value is required.</span></span> <span data-ttu-id="50829-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="50829-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="50829-122">Aucun</span><span class="sxs-lookup"><span data-stu-id="50829-122">None</span></span>
    
- <span data-ttu-id="50829-123">UserBusy</span><span class="sxs-lookup"><span data-stu-id="50829-123">UserBusy</span></span>
    
- <span data-ttu-id="50829-124">Noanswer</span><span class="sxs-lookup"><span data-stu-id="50829-124">NoAnswer</span></span>
    
- <span data-ttu-id="50829-125">Autres</span><span class="sxs-lookup"><span data-stu-id="50829-125">Other</span></span>
    
## <a name="element-information"></a><span data-ttu-id="50829-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="50829-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="50829-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="50829-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="50829-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="50829-128">Schema Name</span></span>  <br/> |<span data-ttu-id="50829-129">Messages</span><span class="sxs-lookup"><span data-stu-id="50829-129">Messages</span></span>  <br/> |
|<span data-ttu-id="50829-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="50829-130">Validation File</span></span>  <br/> |<span data-ttu-id="50829-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="50829-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="50829-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="50829-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="50829-133">False</span><span class="sxs-lookup"><span data-stu-id="50829-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="50829-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50829-134">See also</span></span>



[<span data-ttu-id="50829-135">Opération GetCallInfo (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-135">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
  
[<span data-ttu-id="50829-136">GetCallInfoResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="50829-136">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)

