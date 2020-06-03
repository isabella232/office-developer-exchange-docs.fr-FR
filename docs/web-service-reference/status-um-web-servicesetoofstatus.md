---
title: État (service Web de messagerie unifiée-SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: L’élément Status définit la valeur à utiliser dans une demande d’opération SetOofStatus (service Web de messagerie unifiée).
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459979"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="48c2d-103">État (service Web de messagerie unifiée-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="48c2d-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="48c2d-104">L’élément **Status** définit la valeur à utiliser dans une demande d' [opération SetOofStatus (service Web de messagerie unifiée)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="48c2d-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="48c2d-105">SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="48c2d-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="48c2d-106">État (service Web de messagerie unifiée-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="48c2d-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="48c2d-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="48c2d-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="48c2d-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="48c2d-108">Attributes and elements</span></span>

<span data-ttu-id="48c2d-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="48c2d-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="48c2d-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="48c2d-110">Attributes</span></span>

<span data-ttu-id="48c2d-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="48c2d-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="48c2d-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="48c2d-112">Child elements</span></span>

<span data-ttu-id="48c2d-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="48c2d-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="48c2d-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="48c2d-114">Parent elements</span></span>

|<span data-ttu-id="48c2d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="48c2d-115">**Element**</span></span>|<span data-ttu-id="48c2d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="48c2d-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="48c2d-117">SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="48c2d-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="48c2d-118">Définit une demande de définition de l’état d’absence du Bureau de la messagerie unifiée pour l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="48c2d-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="48c2d-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="48c2d-119">Text value</span></span>

<span data-ttu-id="48c2d-120">Une valeur booléenne est requise.</span><span class="sxs-lookup"><span data-stu-id="48c2d-120">A Boolean value is required.</span></span> <span data-ttu-id="48c2d-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="48c2d-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="48c2d-122">Vrai</span><span class="sxs-lookup"><span data-stu-id="48c2d-122">True</span></span>
    
- <span data-ttu-id="48c2d-123">Faux</span><span class="sxs-lookup"><span data-stu-id="48c2d-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="48c2d-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="48c2d-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="48c2d-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="48c2d-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="48c2d-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="48c2d-126">Schema Name</span></span>  <br/> |<span data-ttu-id="48c2d-127">Messages</span><span class="sxs-lookup"><span data-stu-id="48c2d-127">Messages</span></span>  <br/> |
|<span data-ttu-id="48c2d-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="48c2d-128">Validation File</span></span>  <br/> |<span data-ttu-id="48c2d-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="48c2d-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="48c2d-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="48c2d-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="48c2d-131">False</span><span class="sxs-lookup"><span data-stu-id="48c2d-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="48c2d-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="48c2d-132">See also</span></span>



[<span data-ttu-id="48c2d-133">Opération SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="48c2d-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

