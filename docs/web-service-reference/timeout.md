---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: L’élément Timeout représente la durée, en minutes, pendant laquelle l’abonnement peut rester inactif sans demande GetEvents du client.
ms.openlocfilehash: 6f3228cd480bf0eaf259c4f321bc74d0845b9bba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459895"
---
# <a name="timeout"></a><span data-ttu-id="32aa9-103">Timeout</span><span class="sxs-lookup"><span data-stu-id="32aa9-103">Timeout</span></span>

<span data-ttu-id="32aa9-104">L’élément **timeout** représente la durée, en minutes, pendant laquelle l’abonnement peut rester inactif sans demande GetEvents du client.</span><span class="sxs-lookup"><span data-stu-id="32aa9-104">The **Timeout** element represents the duration, in minutes, that the subscription can remain idle without a GetEvents request from the client.</span></span> 
  
```xml
<Timeout/>
```

 <span data-ttu-id="32aa9-105">**int**</span><span class="sxs-lookup"><span data-stu-id="32aa9-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32aa9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="32aa9-106">Attributes and elements</span></span>

<span data-ttu-id="32aa9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="32aa9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32aa9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="32aa9-108">Attributes</span></span>

<span data-ttu-id="32aa9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="32aa9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32aa9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="32aa9-110">Child elements</span></span>

<span data-ttu-id="32aa9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="32aa9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32aa9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="32aa9-112">Parent elements</span></span>

|<span data-ttu-id="32aa9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="32aa9-113">**Element**</span></span>|<span data-ttu-id="32aa9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="32aa9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32aa9-115">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="32aa9-115">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md) <br/> |<span data-ttu-id="32aa9-116">Représente un abonnement à un abonnement de notification d’événement basé sur l’extraction.</span><span class="sxs-lookup"><span data-stu-id="32aa9-116">Represents a subscription to a pull-based event notification subscription.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32aa9-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="32aa9-117">Text value</span></span>

<span data-ttu-id="32aa9-118">Une valeur de texte qui représente un entier est requise si cet élément est utilisé.</span><span class="sxs-lookup"><span data-stu-id="32aa9-118">A text value that represents an integer is required if this element is used.</span></span> <span data-ttu-id="32aa9-119">Les valeurs possibles de cet élément sont comprises entre 1 et 1440 inclus.</span><span class="sxs-lookup"><span data-stu-id="32aa9-119">The possible values for this element are 1 to 1440, inclusive.</span></span> <span data-ttu-id="32aa9-120">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="32aa9-120">This element is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32aa9-121">Remarques</span><span class="sxs-lookup"><span data-stu-id="32aa9-121">Remarks</span></span>

<span data-ttu-id="32aa9-122">Le délai d’expiration de l’abonnement est réinitialisé par une demande GetEvents réussie.</span><span class="sxs-lookup"><span data-stu-id="32aa9-122">The timeout timer for the subscription is reset by a successful GetEvents request.</span></span>
  
<span data-ttu-id="32aa9-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="32aa9-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="32aa9-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="32aa9-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32aa9-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="32aa9-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32aa9-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="32aa9-126">Schema name</span></span>  <br/> |<span data-ttu-id="32aa9-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="32aa9-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="32aa9-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="32aa9-128">Validation file</span></span>  <br/> |<span data-ttu-id="32aa9-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="32aa9-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32aa9-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="32aa9-130">Can be empty</span></span>  <br/> |<span data-ttu-id="32aa9-131">False</span><span class="sxs-lookup"><span data-stu-id="32aa9-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32aa9-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="32aa9-132">See also</span></span>



[<span data-ttu-id="32aa9-133">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="32aa9-133">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="32aa9-134">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="32aa9-134">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="32aa9-135">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="32aa9-135">Unsubscribe operation</span></span>](unsubscribe-operation.md)

