---
title: État (service web de messagerie unifiée - SetOofStatus)
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
description: L’élément Status définit la valeur à utiliser dans une requête (service web de messagerie unifiée) d’opération SetOofStatus.
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829583"
---
# <a name="status-um-web-service---setoofstatus"></a><span data-ttu-id="ceb21-103">État (service web de messagerie unifiée - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="ceb21-103">Status (UM web service - SetOofStatus)</span></span>

<span data-ttu-id="ceb21-104">L’élément **Status** définit la valeur à utiliser dans une requête [d’opération SetOofStatus (service web de messagerie unifiée)](setoofstatus-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="ceb21-104">The **Status** element defines the value to use in a [SetOofStatus operation (UM web service)](setoofstatus-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="ceb21-105">SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ceb21-105">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="ceb21-106">État (service web de messagerie unifiée - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="ceb21-106">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 <span data-ttu-id="ceb21-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ceb21-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ceb21-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ceb21-108">Attributes and elements</span></span>

<span data-ttu-id="ceb21-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ceb21-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ceb21-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ceb21-110">Attributes</span></span>

<span data-ttu-id="ceb21-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ceb21-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ceb21-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ceb21-112">Child elements</span></span>

<span data-ttu-id="ceb21-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ceb21-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ceb21-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ceb21-114">Parent elements</span></span>

|<span data-ttu-id="ceb21-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ceb21-115">**Element**</span></span>|<span data-ttu-id="ceb21-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="ceb21-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ceb21-117">SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ceb21-117">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md) <br/> |<span data-ttu-id="ceb21-118">Définit une demande pour définir l’état Unified Messaging d’absence du bureau Office (OOF) de l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="ceb21-118">Defines a request to set the Unified Messaging Out of Office (OOF) status for the user who makes the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ceb21-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ceb21-119">Text value</span></span>

<span data-ttu-id="ceb21-120">Une valeur booléenne est requise.</span><span class="sxs-lookup"><span data-stu-id="ceb21-120">A Boolean value is required.</span></span> <span data-ttu-id="ceb21-121">Les valeurs possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="ceb21-121">The following are the possible values:</span></span>
  
- <span data-ttu-id="ceb21-122">True</span><span class="sxs-lookup"><span data-stu-id="ceb21-122">True</span></span>
    
- <span data-ttu-id="ceb21-123">Faux</span><span class="sxs-lookup"><span data-stu-id="ceb21-123">False</span></span>
    
## <a name="element-information"></a><span data-ttu-id="ceb21-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ceb21-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ceb21-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ceb21-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ceb21-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ceb21-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ceb21-127">Messages</span><span class="sxs-lookup"><span data-stu-id="ceb21-127">Messages</span></span>  <br/> |
|<span data-ttu-id="ceb21-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ceb21-128">Validation File</span></span>  <br/> |<span data-ttu-id="ceb21-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ceb21-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ceb21-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ceb21-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ceb21-131">False</span><span class="sxs-lookup"><span data-stu-id="ceb21-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ceb21-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ceb21-132">See also</span></span>



[<span data-ttu-id="ceb21-133">Opération SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ceb21-133">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)

