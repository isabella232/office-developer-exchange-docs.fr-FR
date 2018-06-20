---
title: SubscriptionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionStatus
api_type:
- schema
ms.assetid: 2d64ebb7-f26a-4d02-b7ef-d9d7da75f0c3
description: L’élément SubscriptionStatus décrit l’état d’un abonnement.
ms.openlocfilehash: 1f6de15f7a3b07714899aef2ff74a8d556f8ca1d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838643"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="1ae49-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="1ae49-103">SubscriptionStatus</span></span>

<span data-ttu-id="1ae49-104">L’élément **SubscriptionStatus** décrit l’état d’un abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae49-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="1ae49-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="1ae49-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ae49-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1ae49-106">Attributes and elements</span></span>

<span data-ttu-id="1ae49-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1ae49-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ae49-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1ae49-108">Attributes</span></span>

<span data-ttu-id="1ae49-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ae49-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ae49-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1ae49-110">Child elements</span></span>

<span data-ttu-id="1ae49-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1ae49-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ae49-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1ae49-112">Parent elements</span></span>

|<span data-ttu-id="1ae49-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1ae49-113">**Element**</span></span>|<span data-ttu-id="1ae49-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="1ae49-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ae49-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="1ae49-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="1ae49-116">Contient la réponse de l’application cliente » à une notification push.</span><span class="sxs-lookup"><span data-stu-id="1ae49-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ae49-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1ae49-117">Text value</span></span>

<span data-ttu-id="1ae49-118">Une valeur texte est requise.</span><span class="sxs-lookup"><span data-stu-id="1ae49-118">A text value is required.</span></span> <span data-ttu-id="1ae49-119">Les valeurs de texte possibles de cet élément sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="1ae49-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="1ae49-120">OK</span><span class="sxs-lookup"><span data-stu-id="1ae49-120">OK</span></span>
    
- <span data-ttu-id="1ae49-121">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="1ae49-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1ae49-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="1ae49-122">Remarks</span></span>

<span data-ttu-id="1ae49-123">Cet élément décrit l’état de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae49-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="1ae49-124">L’application cliente d’abonnement push envoie le statut sur l’ordinateur qui exécute Exchange 2007 qui a le rôle de serveur d’accès au Client installé après chaque notification push.</span><span class="sxs-lookup"><span data-stu-id="1ae49-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="1ae49-125">Si la valeur **SubscriptionStatus** est égale à **Annuler l’abonnement**, le serveur d’accès au Client arrêter l’envoi de notifications et mettre fin à l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="1ae49-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="1ae49-126">Si la valeur **SubscriptionStatus** est égale à **OK**, le serveur d’accès au Client continuera d’envoyer des notifications.</span><span class="sxs-lookup"><span data-stu-id="1ae49-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="1ae49-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="1ae49-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ae49-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1ae49-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ae49-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1ae49-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ae49-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1ae49-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1ae49-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1ae49-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ae49-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1ae49-132">Validation File</span></span>  <br/> |<span data-ttu-id="1ae49-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1ae49-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ae49-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1ae49-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ae49-135">False</span><span class="sxs-lookup"><span data-stu-id="1ae49-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ae49-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1ae49-136">See also</span></span>



- [<span data-ttu-id="1ae49-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1ae49-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

