---
title: OofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- OofStatus
api_type:
- schema
ms.assetid: 0ba4225a-784e-4e6e-bd20-be45f0f7597c
description: L’élément OofStatus contient une valeur que l’état Unified Messaging d’absence du bureau de l’utilisateur qui effectue une demande de (service web de messagerie unifiée) opération GetUMProperties indicaties.
ms.openlocfilehash: 1fe358a8bfea3c509220d6705a238ae832de37e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828650"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="d8118-103">OofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="d8118-104">L’élément **OofStatus** contient une valeur qui indicaties l’état Unified Messaging d’absence du bureau de l’utilisateur qui effectue une demande [d’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d8118-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="d8118-105">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="d8118-106">OofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="d8118-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d8118-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d8118-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d8118-108">Attributes and elements</span></span>

<span data-ttu-id="d8118-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d8118-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d8118-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="d8118-110">Attributes</span></span>

<span data-ttu-id="d8118-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d8118-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d8118-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d8118-112">Child elements</span></span>

<span data-ttu-id="d8118-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d8118-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d8118-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d8118-114">Parent elements</span></span>

|<span data-ttu-id="d8118-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d8118-115">**Element**</span></span>|<span data-ttu-id="d8118-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d8118-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d8118-117">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="d8118-118">Définit une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="d8118-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d8118-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="d8118-119">Text value</span></span>

<span data-ttu-id="d8118-120">Une valeur de type Boolean texte est requise.</span><span class="sxs-lookup"><span data-stu-id="d8118-120">A Boolean text value is required.</span></span> <span data-ttu-id="d8118-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="d8118-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="d8118-122">True</span><span class="sxs-lookup"><span data-stu-id="d8118-122">True</span></span>
    
- <span data-ttu-id="d8118-123">Faux</span><span class="sxs-lookup"><span data-stu-id="d8118-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="d8118-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d8118-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d8118-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d8118-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d8118-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d8118-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d8118-127">Messages</span><span class="sxs-lookup"><span data-stu-id="d8118-127">Messages</span></span>  <br/> |
|<span data-ttu-id="d8118-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d8118-128">Validation File</span></span>  <br/> |<span data-ttu-id="d8118-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d8118-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d8118-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d8118-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d8118-131">False</span><span class="sxs-lookup"><span data-stu-id="d8118-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d8118-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d8118-132">See also</span></span>



[<span data-ttu-id="d8118-133">Opération GetUMProperties (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="d8118-134">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="d8118-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

