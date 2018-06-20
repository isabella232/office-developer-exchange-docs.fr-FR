---
title: Opération GetCallInfo (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: L’opération GetCallInfo renvoie l’état de l’appel sortant qui est spécifiée par l’ID d’appel (service web de messagerie unifiée).
ms.openlocfilehash: 36f9cba3690520ebb457a4cb2bfbcde3fea4b8dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756533"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="67d0a-103">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="67d0a-104">L’opération GetCallInfo renvoie l’état de l’appel sortant qui est spécifiée par [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="67d0a-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="67d0a-105">Exemple de requête GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="67d0a-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="67d0a-106">Description</span><span class="sxs-lookup"><span data-stu-id="67d0a-106">Description</span></span>

<span data-ttu-id="67d0a-107">L’exemple suivant d’une demande GetCallInfo montre comment former une demande pour obtenir des informations relatives à un appel sortant spécifié.</span><span class="sxs-lookup"><span data-stu-id="67d0a-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="67d0a-108">Code</span><span class="sxs-lookup"><span data-stu-id="67d0a-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="67d0a-109">Exemple de réponse GetCallInfo réussie</span><span class="sxs-lookup"><span data-stu-id="67d0a-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="67d0a-110">Description</span><span class="sxs-lookup"><span data-stu-id="67d0a-110">Description</span></span>

<span data-ttu-id="67d0a-111">Une réponse GetCallInfo l’exemple suivant montre une réponse à une demande de GetCallInfo.</span><span class="sxs-lookup"><span data-stu-id="67d0a-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="67d0a-112">Code</span><span class="sxs-lookup"><span data-stu-id="67d0a-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="67d0a-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67d0a-113">See also</span></span>



[<span data-ttu-id="67d0a-114">GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="67d0a-115">GetCallInfoResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="67d0a-116">ID d’appel (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="67d0a-117">CallState (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="67d0a-118">EventCause (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="67d0a-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

