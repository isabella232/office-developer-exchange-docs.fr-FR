---
title: Annuler l’opération
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
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: L’opération Annuler l’abonnement est utilisée pour mettre fin à un abonnement de notification. Utilisez cette opération, plutôt que de laisser un délai d’expiration de l’abonnement. Cette opération est uniquement valide pour les notifications de type pull.
ms.openlocfilehash: 64514a718d473f0fd7d0320bd1ccecddb1940ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838845"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="5cb3d-105">Annuler l’opération</span><span class="sxs-lookup"><span data-stu-id="5cb3d-105">Unsubscribe operation</span></span>

<span data-ttu-id="5cb3d-106">L’opération Annuler l’abonnement est utilisée pour mettre fin à un abonnement de notification.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="5cb3d-107">Utilisez cette opération, plutôt que de laisser un délai d’expiration de l’abonnement.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="5cb3d-108">Cette opération est uniquement valide pour les notifications de type pull.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="5cb3d-109">Annuler l’abonnement d’exemple de requête</span><span class="sxs-lookup"><span data-stu-id="5cb3d-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="5cb3d-110">Description</span><span class="sxs-lookup"><span data-stu-id="5cb3d-110">Description</span></span>

<span data-ttu-id="5cb3d-111">L’exemple suivant montre le message SOAP XML qui est envoyé pour annuler l’abonnement d’un client à partir du service de Notification.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="5cb3d-112">Code</span><span class="sxs-lookup"><span data-stu-id="5cb3d-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="5cb3d-113">Annuler l’abonnement aux éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="5cb3d-113">Unsubscribe request elements</span></span>

<span data-ttu-id="5cb3d-114">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="5cb3d-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5cb3d-115">Annuler l’abonnement</span><span class="sxs-lookup"><span data-stu-id="5cb3d-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="5cb3d-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="5cb3d-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="5cb3d-117">Exemple de réponse de désabonnement réussi</span><span class="sxs-lookup"><span data-stu-id="5cb3d-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="5cb3d-118">Description</span><span class="sxs-lookup"><span data-stu-id="5cb3d-118">Description</span></span>

<span data-ttu-id="5cb3d-119">L’exemple suivant montre une réponse positive à une demande de désabonnement.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5cb3d-120">Code</span><span class="sxs-lookup"><span data-stu-id="5cb3d-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="5cb3d-121">Annuler l’abonnement aux éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="5cb3d-121">Unsubscribe response elements</span></span>

<span data-ttu-id="5cb3d-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="5cb3d-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5cb3d-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5cb3d-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5cb3d-124">Annuler l’abonnement</span><span class="sxs-lookup"><span data-stu-id="5cb3d-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="5cb3d-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5cb3d-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5cb3d-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5cb3d-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="5cb3d-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5cb3d-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="5cb3d-128">Annuler l’abonnement d’exemple de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="5cb3d-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="5cb3d-129">Description</span><span class="sxs-lookup"><span data-stu-id="5cb3d-129">Description</span></span>

<span data-ttu-id="5cb3d-130">L’exemple suivant d’une réponse d’erreur désabonnement se produit en réponse à une tentative d’annuler l’abonnement à l’aide d’un identificateur d’abonnement qui ne peut pas être situé dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cb3d-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="5cb3d-131">Code</span><span class="sxs-lookup"><span data-stu-id="5cb3d-131">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="5cb3d-132">Annuler l’abonnement aux éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="5cb3d-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="5cb3d-133">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="5cb3d-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5cb3d-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5cb3d-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5cb3d-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="5cb3d-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="5cb3d-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5cb3d-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5cb3d-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5cb3d-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="5cb3d-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="5cb3d-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5cb3d-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5cb3d-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5cb3d-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5cb3d-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="5cb3d-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5cb3d-141">See also</span></span>

- [<span data-ttu-id="5cb3d-142">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="5cb3d-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="5cb3d-143">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="5cb3d-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="5cb3d-144">À l’aide d’abonnement</span><span class="sxs-lookup"><span data-stu-id="5cb3d-144">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

