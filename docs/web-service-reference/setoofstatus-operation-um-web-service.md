---
title: Opération SetOofStatus (service Web de messagerie unifiée)
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
description: L’opération SetOofStatus définit une valeur qui indique si le message d’accueil de l’absence du Bureau doit être lu pour l’utilisateur qui effectue la demande.
ms.openlocfilehash: 2311b6137ac25d15ad3d06668450c1d0f7ec1fad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467353"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="b3aa6-103">Opération SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b3aa6-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="b3aa6-104">L’opération SetOofStatus définit une valeur qui indique si le message d’accueil de l’absence du Bureau doit être lu pour l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="b3aa6-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="b3aa6-105">Exemple de requête SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="b3aa6-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="b3aa6-106">Description</span><span class="sxs-lookup"><span data-stu-id="b3aa6-106">Description</span></span>

<span data-ttu-id="b3aa6-107">L’exemple de requête SetOofStatus suivant montre comment créer une demande pour activer le message d’accueil d’absence du Bureau pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="b3aa6-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="b3aa6-108">Code</span><span class="sxs-lookup"><span data-stu-id="b3aa6-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="b3aa6-109">Exemple de réponse SetOofStatus réussi</span><span class="sxs-lookup"><span data-stu-id="b3aa6-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="b3aa6-110">Description</span><span class="sxs-lookup"><span data-stu-id="b3aa6-110">Description</span></span>

<span data-ttu-id="b3aa6-111">L’exemple suivant de réponse SetOofStatus indique une réponse à la demande SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="b3aa6-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b3aa6-112">Code</span><span class="sxs-lookup"><span data-stu-id="b3aa6-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b3aa6-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b3aa6-113">See also</span></span>



[<span data-ttu-id="b3aa6-114">SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b3aa6-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="b3aa6-115">SetOofStatusResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="b3aa6-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="b3aa6-116">État (service Web de messagerie unifiée-SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="b3aa6-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

