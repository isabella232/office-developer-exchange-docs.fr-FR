---
title: SendNotificationResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResult
api_type:
- schema
ms.assetid: fa9d6202-fa66-4f10-9858-53f4f1ce14bc
description: L’élément SendNotificationResult contient la réponse d’une application client à une notification push.
ms.openlocfilehash: 9acaa396430cf4e06a9c996834874d19dcab50ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829350"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="39a6f-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="39a6f-103">SendNotificationResult</span></span>

<span data-ttu-id="39a6f-104">L’élément **SendNotificationResult** contient la réponse d’une application client à une notification push.</span><span class="sxs-lookup"><span data-stu-id="39a6f-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="39a6f-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="39a6f-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39a6f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="39a6f-106">Attributes and elements</span></span>

<span data-ttu-id="39a6f-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="39a6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39a6f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="39a6f-108">Attributes</span></span>

<span data-ttu-id="39a6f-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="39a6f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39a6f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="39a6f-110">Child elements</span></span>

|<span data-ttu-id="39a6f-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="39a6f-111">**Element**</span></span>|<span data-ttu-id="39a6f-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="39a6f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39a6f-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="39a6f-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="39a6f-114">Décrit l’état d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="39a6f-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39a6f-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="39a6f-115">Parent elements</span></span>

<span data-ttu-id="39a6f-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="39a6f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="39a6f-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="39a6f-117">Remarks</span></span>

<span data-ttu-id="39a6f-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="39a6f-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39a6f-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="39a6f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39a6f-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="39a6f-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39a6f-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="39a6f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="39a6f-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="39a6f-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39a6f-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="39a6f-123">Validation File</span></span>  <br/> |<span data-ttu-id="39a6f-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="39a6f-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39a6f-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="39a6f-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="39a6f-126">False</span><span class="sxs-lookup"><span data-stu-id="39a6f-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39a6f-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="39a6f-127">See also</span></span>



- [<span data-ttu-id="39a6f-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="39a6f-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

