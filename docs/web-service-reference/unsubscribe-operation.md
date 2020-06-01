---
title: Opération de résiliation d’abonnement
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
description: L’opération de désinscription est utilisée pour mettre fin à un abonnement de notification par extraction. Utilisez cette opération au lieu de laisser un délai d’expiration d’abonnement. Cette opération est valide uniquement pour les notifications de type pull.
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468025"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="4ff84-105">Opération de résiliation d’abonnement</span><span class="sxs-lookup"><span data-stu-id="4ff84-105">Unsubscribe operation</span></span>

<span data-ttu-id="4ff84-106">L’opération de désinscription est utilisée pour mettre fin à un abonnement de notification par extraction.</span><span class="sxs-lookup"><span data-stu-id="4ff84-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="4ff84-107">Utilisez cette opération au lieu de laisser un délai d’expiration d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="4ff84-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="4ff84-108">Cette opération est valide uniquement pour les notifications de type pull.</span><span class="sxs-lookup"><span data-stu-id="4ff84-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="4ff84-109">Exemple de requête de désinscription</span><span class="sxs-lookup"><span data-stu-id="4ff84-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="4ff84-110">Description</span><span class="sxs-lookup"><span data-stu-id="4ff84-110">Description</span></span>

<span data-ttu-id="4ff84-111">L’exemple suivant montre le message XML SOAP qui est envoyé pour annuler l’abonnement d’un client à partir du service de notification.</span><span class="sxs-lookup"><span data-stu-id="4ff84-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="4ff84-112">Code</span><span class="sxs-lookup"><span data-stu-id="4ff84-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="4ff84-113">Éléments de requête de désinscription</span><span class="sxs-lookup"><span data-stu-id="4ff84-113">Unsubscribe request elements</span></span>

<span data-ttu-id="4ff84-114">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="4ff84-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="4ff84-115">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="4ff84-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="4ff84-116">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="4ff84-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="4ff84-117">Exemple de réponse de désinscription réussie</span><span class="sxs-lookup"><span data-stu-id="4ff84-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="4ff84-118">Description</span><span class="sxs-lookup"><span data-stu-id="4ff84-118">Description</span></span>

<span data-ttu-id="4ff84-119">L’exemple suivant montre une réponse réussie à une demande d’annulation d’abonnement.</span><span class="sxs-lookup"><span data-stu-id="4ff84-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="4ff84-120">Code</span><span class="sxs-lookup"><span data-stu-id="4ff84-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="4ff84-121">Éléments de réponse de désinscription</span><span class="sxs-lookup"><span data-stu-id="4ff84-121">Unsubscribe response elements</span></span>

<span data-ttu-id="4ff84-122">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="4ff84-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="4ff84-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4ff84-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4ff84-124">Se désabonner</span><span class="sxs-lookup"><span data-stu-id="4ff84-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="4ff84-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4ff84-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4ff84-126">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4ff84-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="4ff84-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4ff84-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="4ff84-128">Exemple de réponse d’erreur d’annulation d’abonnement</span><span class="sxs-lookup"><span data-stu-id="4ff84-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="4ff84-129">Description</span><span class="sxs-lookup"><span data-stu-id="4ff84-129">Description</span></span>

<span data-ttu-id="4ff84-130">L’exemple suivant de réponse à une erreur d’annulation d’abonnement se produit en réponse à une tentative d’annulation d’abonnement à l’aide d’un identificateur d’abonnement introuvable dans la Banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="4ff84-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="4ff84-131">Code</span><span class="sxs-lookup"><span data-stu-id="4ff84-131">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="4ff84-132">Éléments de réponse d’erreur d’annulation d’abonnement</span><span class="sxs-lookup"><span data-stu-id="4ff84-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="4ff84-133">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="4ff84-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="4ff84-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4ff84-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="4ff84-135">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="4ff84-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="4ff84-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4ff84-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4ff84-137">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4ff84-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="4ff84-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="4ff84-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4ff84-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4ff84-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4ff84-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4ff84-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="4ff84-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4ff84-141">See also</span></span>

- [<span data-ttu-id="4ff84-142">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="4ff84-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="4ff84-143">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="4ff84-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="4ff84-144">Utilisation des abonnements extraits</span><span class="sxs-lookup"><span data-stu-id="4ff84-144">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

