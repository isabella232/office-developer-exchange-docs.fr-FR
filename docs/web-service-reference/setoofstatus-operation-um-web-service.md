---
title: Opération SetOofStatus (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du bureau (OOF) doit être lu de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829445"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="b6140-103">Opération SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b6140-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="b6140-104">L’opération SetOofStatus définit une valeur qui indique si le message d’accueil d’absence du bureau (OOF) doit être lu de l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="b6140-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="b6140-105">Exemple de requête SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="b6140-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="b6140-106">Description</span><span class="sxs-lookup"><span data-stu-id="b6140-106">Description</span></span>

<span data-ttu-id="b6140-107">Une demande de SetOofStatus l’exemple suivant montre comment créer une requête pour activer le message d’accueil d’absence du bureau pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b6140-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="b6140-108">Code</span><span class="sxs-lookup"><span data-stu-id="b6140-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="b6140-109">Exemple de réponse SetOofStatus réussie</span><span class="sxs-lookup"><span data-stu-id="b6140-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="b6140-110">Description</span><span class="sxs-lookup"><span data-stu-id="b6140-110">Description</span></span>

<span data-ttu-id="b6140-111">Une réponse SetOofStatus l’exemple suivant montre une réponse à la demande SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="b6140-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b6140-112">Code</span><span class="sxs-lookup"><span data-stu-id="b6140-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b6140-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b6140-113">See also</span></span>



[<span data-ttu-id="b6140-114">SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b6140-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="b6140-115">SetOofStatusResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b6140-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="b6140-116">État (service web de messagerie unifiée - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="b6140-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

