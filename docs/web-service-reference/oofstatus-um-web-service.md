---
title: OofStatus (service Web de messagerie unifiée)
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
description: L’élément OofStatus contient une valeur qui indicaties l’état de la messagerie unifiée pour l’utilisateur qui effectue une opération GetUMProperties (service Web de messagerie unifiée).
ms.openlocfilehash: 80b1d5aa508579eec14637ed10c322b5fbb670da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460574"
---
# <a name="oofstatus-um-web-service"></a><span data-ttu-id="4b6ed-103">OofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-103">OofStatus (UM web service)</span></span>

<span data-ttu-id="4b6ed-104">L’élément **OofStatus** contient une valeur qui indicaties l’état de la messagerie unifiée pour l’utilisateur qui effectue une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="4b6ed-104">The **OofStatus** element contains a value that indicaties the Unified Messaging Out of Office status for the user who is making a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="4b6ed-105">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
[<span data-ttu-id="4b6ed-106">OofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-106">OofStatus (UM web service)</span></span>](oofstatus-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
    <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="4b6ed-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4b6ed-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b6ed-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4b6ed-108">Attributes and elements</span></span>

<span data-ttu-id="4b6ed-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4b6ed-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b6ed-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="4b6ed-110">Attributes</span></span>

<span data-ttu-id="4b6ed-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4b6ed-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b6ed-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4b6ed-112">Child elements</span></span>

<span data-ttu-id="4b6ed-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4b6ed-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b6ed-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4b6ed-114">Parent elements</span></span>

|<span data-ttu-id="4b6ed-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4b6ed-115">**Element**</span></span>|<span data-ttu-id="4b6ed-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="4b6ed-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b6ed-117">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-117">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md) <br/> |<span data-ttu-id="4b6ed-118">Définit une réponse à une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="4b6ed-118">Defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4b6ed-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4b6ed-119">Text value</span></span>

<span data-ttu-id="4b6ed-120">Une valeur de texte Boolean est requise.</span><span class="sxs-lookup"><span data-stu-id="4b6ed-120">A Boolean text value is required.</span></span> <span data-ttu-id="4b6ed-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="4b6ed-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="4b6ed-122">Vrai</span><span class="sxs-lookup"><span data-stu-id="4b6ed-122">True</span></span>
    
- <span data-ttu-id="4b6ed-123">Faux</span><span class="sxs-lookup"><span data-stu-id="4b6ed-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="4b6ed-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4b6ed-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b6ed-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4b6ed-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4b6ed-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4b6ed-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4b6ed-127">Messages</span><span class="sxs-lookup"><span data-stu-id="4b6ed-127">Messages</span></span>  <br/> |
|<span data-ttu-id="4b6ed-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4b6ed-128">Validation File</span></span>  <br/> |<span data-ttu-id="4b6ed-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4b6ed-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4b6ed-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4b6ed-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b6ed-131">False</span><span class="sxs-lookup"><span data-stu-id="4b6ed-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b6ed-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4b6ed-132">See also</span></span>



[<span data-ttu-id="4b6ed-133">Opération GetUMProperties (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-133">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
  
[<span data-ttu-id="4b6ed-134">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="4b6ed-134">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

