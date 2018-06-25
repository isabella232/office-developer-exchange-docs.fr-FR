---
title: (Service web de messagerie unifiée) de l’opération de déconnexion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: L’opération de déconnexion met fin à l’appel est identifié par l’ID d’appel (service web de messagerie unifiée) spécifié.
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755960"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="8ee6e-103">(Service web de messagerie unifiée) de l’opération de déconnexion</span><span class="sxs-lookup"><span data-stu-id="8ee6e-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="8ee6e-104">L’opération de déconnexion met fin à l’appel est identifié par [l’ID d’appel (service web de messagerie unifiée)](callid-um-web-service.md)de spécifié.</span><span class="sxs-lookup"><span data-stu-id="8ee6e-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="8ee6e-105">Exemple de requête de déconnexion</span><span class="sxs-lookup"><span data-stu-id="8ee6e-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="8ee6e-106">Description</span><span class="sxs-lookup"><span data-stu-id="8ee6e-106">Description</span></span>

<span data-ttu-id="8ee6e-107">Une demande de déconnexion l’exemple suivant montre comment former une demande de déconnexion d’un appel.</span><span class="sxs-lookup"><span data-stu-id="8ee6e-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="8ee6e-108">Code</span><span class="sxs-lookup"><span data-stu-id="8ee6e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="8ee6e-109">Exemple de réponse de déconnexion réussie</span><span class="sxs-lookup"><span data-stu-id="8ee6e-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="8ee6e-110">Description</span><span class="sxs-lookup"><span data-stu-id="8ee6e-110">Description</span></span>

<span data-ttu-id="8ee6e-111">L’exemple suivant d’une réponse de déconnexion montre une réponse à la demande de déconnexion.</span><span class="sxs-lookup"><span data-stu-id="8ee6e-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8ee6e-112">Code</span><span class="sxs-lookup"><span data-stu-id="8ee6e-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8ee6e-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8ee6e-113">See also</span></span>

- [<span data-ttu-id="8ee6e-114">Déconnecter (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8ee6e-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="8ee6e-115">DisconnectResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8ee6e-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="8ee6e-116">ID d’appel (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="8ee6e-116">CallId (UM web service)</span></span>](callid-um-web-service.md)

