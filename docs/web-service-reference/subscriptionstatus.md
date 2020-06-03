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
description: L’élément SubscriptionStatus décrit l’état d’un abonnement envoyé.
ms.openlocfilehash: 195ab229380f4386b39e5c3fd48208cf66e224f0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530943"
---
# <a name="subscriptionstatus"></a><span data-ttu-id="ca98f-103">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="ca98f-103">SubscriptionStatus</span></span>

<span data-ttu-id="ca98f-104">L’élément **SubscriptionStatus** décrit l’état d’un abonnement envoyé.</span><span class="sxs-lookup"><span data-stu-id="ca98f-104">The **SubscriptionStatus** element describes the status of a push subscription.</span></span> 
  
```xml
<SubscriptionStatus>OK or Unsubscribe</SubscriptionStatus>
```

 <span data-ttu-id="ca98f-105">**SubscriptionStatusType**</span><span class="sxs-lookup"><span data-stu-id="ca98f-105">**SubscriptionStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca98f-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca98f-106">Attributes and elements</span></span>

<span data-ttu-id="ca98f-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca98f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca98f-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca98f-108">Attributes</span></span>

<span data-ttu-id="ca98f-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ca98f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca98f-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca98f-110">Child elements</span></span>

<span data-ttu-id="ca98f-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca98f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ca98f-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca98f-112">Parent elements</span></span>

|<span data-ttu-id="ca98f-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca98f-113">**Element**</span></span>|<span data-ttu-id="ca98f-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca98f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca98f-115">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="ca98f-115">SendNotificationResult</span></span>](sendnotificationresult.md) <br/> |<span data-ttu-id="ca98f-116">Contient la réponse de l’application cliente à une notification de type transmission.</span><span class="sxs-lookup"><span data-stu-id="ca98f-116">Contains the response of the client application' to a push notification.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ca98f-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="ca98f-117">Text value</span></span>

<span data-ttu-id="ca98f-118">Une valeur de texte est requise.</span><span class="sxs-lookup"><span data-stu-id="ca98f-118">A text value is required.</span></span> <span data-ttu-id="ca98f-119">Voici les valeurs de texte possibles pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="ca98f-119">The following are the possible text values for this element:</span></span>
  
- <span data-ttu-id="ca98f-120">OK</span><span class="sxs-lookup"><span data-stu-id="ca98f-120">OK</span></span>
    
- <span data-ttu-id="ca98f-121">Se désinscrire</span><span class="sxs-lookup"><span data-stu-id="ca98f-121">Unsubscribe</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ca98f-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca98f-122">Remarks</span></span>

<span data-ttu-id="ca98f-123">Cet élément décrit l’état de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca98f-123">This element describes the status of the subscription.</span></span> <span data-ttu-id="ca98f-124">L’application cliente d’abonnement poussé renvoie l’État à l’ordinateur qui exécute Exchange 2007 sur lequel le rôle de serveur d’accès au client est installé après chaque notification de transmission.</span><span class="sxs-lookup"><span data-stu-id="ca98f-124">The push subscription client application sends the status back to the computer that is running Exchange 2007 that has the Client Access server role installed after each push notification.</span></span> <span data-ttu-id="ca98f-125">Si la valeur **SubscriptionStatus** est **unsubscribe**, le serveur d’accès au client cesse d’envoyer des notifications et met fin à l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="ca98f-125">If the **SubscriptionStatus** value equals **Unsubscribe**, the Client Access server will stop sending notifications and end the subscription.</span></span> <span data-ttu-id="ca98f-126">Si la valeur **SubscriptionStatus** est définie sur **OK**, le serveur d’accès au client continuera à envoyer des notifications.</span><span class="sxs-lookup"><span data-stu-id="ca98f-126">If the **SubscriptionStatus** value equals **OK**, the Client Access server will continue to send notifications.</span></span>
  
<span data-ttu-id="ca98f-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ca98f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca98f-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ca98f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca98f-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ca98f-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ca98f-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ca98f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="ca98f-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ca98f-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ca98f-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ca98f-132">Validation File</span></span>  <br/> |<span data-ttu-id="ca98f-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ca98f-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ca98f-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ca98f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca98f-135">False</span><span class="sxs-lookup"><span data-stu-id="ca98f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca98f-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca98f-136">See also</span></span>



- [<span data-ttu-id="ca98f-137">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ca98f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

