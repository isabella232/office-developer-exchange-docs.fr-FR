---
title: Se désabonner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 5584db5f-553a-47ce-85fb-f9902c9990ab
description: L’élément de désabonnement contient les propriétés utilisées pour annuler l’abonnement à partir d’un abonnement.
ms.openlocfilehash: bab797ff74a921e3e93c993229bc6d6d289e0c5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838843"
---
# <a name="unsubscribe"></a><span data-ttu-id="a82b9-103">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="a82b9-103">Unsubscribe</span></span>

<span data-ttu-id="a82b9-104">L’élément de **désabonnement** contient les propriétés utilisées pour annuler l’abonnement à partir d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="a82b9-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="a82b9-105">Annuler l’abonnement</span><span class="sxs-lookup"><span data-stu-id="a82b9-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="a82b9-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="a82b9-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a82b9-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a82b9-107">Attributes and elements</span></span>

<span data-ttu-id="a82b9-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a82b9-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a82b9-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="a82b9-109">Attributes</span></span>

<span data-ttu-id="a82b9-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a82b9-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a82b9-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a82b9-111">Child elements</span></span>

|<span data-ttu-id="a82b9-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a82b9-112">**Element**</span></span>|<span data-ttu-id="a82b9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="a82b9-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a82b9-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="a82b9-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="a82b9-115">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="a82b9-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a82b9-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a82b9-116">Parent elements</span></span>

<span data-ttu-id="a82b9-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a82b9-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a82b9-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="a82b9-118">Remarks</span></span>

<span data-ttu-id="a82b9-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a82b9-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a82b9-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a82b9-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a82b9-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a82b9-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a82b9-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a82b9-122">Schema name</span></span>  <br/> |<span data-ttu-id="a82b9-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a82b9-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a82b9-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a82b9-124">Validation file</span></span>  <br/> |<span data-ttu-id="a82b9-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a82b9-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a82b9-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a82b9-126">Can be empty</span></span>  <br/> |<span data-ttu-id="a82b9-127">False</span><span class="sxs-lookup"><span data-stu-id="a82b9-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a82b9-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a82b9-128">See also</span></span>



[<span data-ttu-id="a82b9-129">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a82b9-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="a82b9-130">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="a82b9-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="a82b9-131">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="a82b9-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

