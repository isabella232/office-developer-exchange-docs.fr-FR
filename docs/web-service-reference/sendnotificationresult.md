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
description: L’élément SendNotificationResult contient la réponse d’une application client à une notification de type transmission.
ms.openlocfilehash: 4ee9a0dda3d887f8fbfa2c2b34a9a077e7af37ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464888"
---
# <a name="sendnotificationresult"></a><span data-ttu-id="00584-103">SendNotificationResult</span><span class="sxs-lookup"><span data-stu-id="00584-103">SendNotificationResult</span></span>

<span data-ttu-id="00584-104">L’élément **SendNotificationResult** contient la réponse d’une application client à une notification de type transmission.</span><span class="sxs-lookup"><span data-stu-id="00584-104">The **SendNotificationResult** element contains the response of a client application to a push notification.</span></span> 
  
```xml
<SendNotificationResult>
   <SubscriptionStatus/>
</SendNotificationResult>
```

 <span data-ttu-id="00584-105">**SendNotificationResultType**</span><span class="sxs-lookup"><span data-stu-id="00584-105">**SendNotificationResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00584-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="00584-106">Attributes and elements</span></span>

<span data-ttu-id="00584-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="00584-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00584-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="00584-108">Attributes</span></span>

<span data-ttu-id="00584-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="00584-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00584-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="00584-110">Child elements</span></span>

|<span data-ttu-id="00584-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="00584-111">**Element**</span></span>|<span data-ttu-id="00584-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="00584-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00584-113">SubscriptionStatus</span><span class="sxs-lookup"><span data-stu-id="00584-113">SubscriptionStatus</span></span>](subscriptionstatus.md) <br/> |<span data-ttu-id="00584-114">Décrit l’état d’un abonnement envoyé.</span><span class="sxs-lookup"><span data-stu-id="00584-114">Describes the status of a push subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="00584-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="00584-115">Parent elements</span></span>

<span data-ttu-id="00584-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="00584-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="00584-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="00584-117">Remarks</span></span>

<span data-ttu-id="00584-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="00584-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00584-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="00584-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00584-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="00584-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00584-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="00584-121">Schema Name</span></span>  <br/> |<span data-ttu-id="00584-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="00584-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00584-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="00584-123">Validation File</span></span>  <br/> |<span data-ttu-id="00584-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="00584-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00584-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="00584-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="00584-126">False</span><span class="sxs-lookup"><span data-stu-id="00584-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00584-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="00584-127">See also</span></span>



- [<span data-ttu-id="00584-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="00584-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

