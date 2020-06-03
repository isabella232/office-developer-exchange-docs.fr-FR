---
title: Se désinscrire
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
description: L’élément unsubscribe contient les propriétés utilisées pour annuler l’abonnement à un abonnement.
ms.openlocfilehash: d3d9c3bf9ad97cc0fdabf574c6505c797583838a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467213"
---
# <a name="unsubscribe"></a><span data-ttu-id="69abe-103">Se désinscrire</span><span class="sxs-lookup"><span data-stu-id="69abe-103">Unsubscribe</span></span>

<span data-ttu-id="69abe-104">L’élément **unsubscribe** contient les propriétés utilisées pour annuler l’abonnement à un abonnement.</span><span class="sxs-lookup"><span data-stu-id="69abe-104">The **Unsubscribe** element contains the properties used to unsubscribe from a subscription.</span></span> 
  
[<span data-ttu-id="69abe-105">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="69abe-105">Unsubscribe</span></span>](unsubscribe.md)
  
```xml
<Unsubscribe>
   <SubscriptionId/>
</Unsubscribe>
```

 <span data-ttu-id="69abe-106">**UnsubscribeType**</span><span class="sxs-lookup"><span data-stu-id="69abe-106">**UnsubscribeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69abe-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="69abe-107">Attributes and elements</span></span>

<span data-ttu-id="69abe-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="69abe-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69abe-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="69abe-109">Attributes</span></span>

<span data-ttu-id="69abe-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="69abe-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69abe-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="69abe-111">Child elements</span></span>

|<span data-ttu-id="69abe-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="69abe-112">**Element**</span></span>|<span data-ttu-id="69abe-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="69abe-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69abe-114">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="69abe-114">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="69abe-115">Représente l’identificateur d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="69abe-115">Represents the identifier for a subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69abe-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="69abe-116">Parent elements</span></span>

<span data-ttu-id="69abe-117">Aucun.</span><span class="sxs-lookup"><span data-stu-id="69abe-117">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69abe-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="69abe-118">Remarks</span></span>

<span data-ttu-id="69abe-119">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="69abe-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69abe-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="69abe-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69abe-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="69abe-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="69abe-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="69abe-122">Schema name</span></span>  <br/> |<span data-ttu-id="69abe-123">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="69abe-123">Messages schema</span></span>  <br/> |
|<span data-ttu-id="69abe-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="69abe-124">Validation file</span></span>  <br/> |<span data-ttu-id="69abe-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="69abe-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="69abe-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="69abe-126">Can be empty</span></span>  <br/> |<span data-ttu-id="69abe-127">False</span><span class="sxs-lookup"><span data-stu-id="69abe-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69abe-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="69abe-128">See also</span></span>



[<span data-ttu-id="69abe-129">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="69abe-129">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="69abe-130">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="69abe-130">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="69abe-131">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="69abe-131">Unsubscribe operation</span></span>](unsubscribe-operation.md)

