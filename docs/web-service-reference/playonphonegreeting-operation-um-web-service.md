---
title: Opération PlayOnPhoneGreeting (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhoneGreeting
api_type:
- schema
ms.assetid: 6deafc40-290b-4bce-9914-b6bcc529f38a
description: L’opération PlayOnPhoneGreeting un appel sortant et la lecture d’un des messages deux message d’accueil sur le téléphone.
ms.openlocfilehash: 85ba76c7638911678c1ef1aef88f47fdab2c6a4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828828"
---
# <a name="playonphonegreeting-operation-um-web-service"></a><span data-ttu-id="ff765-103">Opération PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ff765-103">PlayOnPhoneGreeting operation (UM web service)</span></span>

<span data-ttu-id="ff765-104">L’opération PlayOnPhoneGreeting un appel sortant et la lecture d’un des messages deux message d’accueil sur le téléphone.</span><span class="sxs-lookup"><span data-stu-id="ff765-104">The PlayOnPhoneGreeting operation makes an outbound call and plays one of the two greeting messages on the telephone.</span></span>
  
## <a name="playonphonegreeting-request-example"></a><span data-ttu-id="ff765-105">Exemple de requête PlayOnPhoneGreeting</span><span class="sxs-lookup"><span data-stu-id="ff765-105">PlayOnPhoneGreeting request example</span></span>

### <a name="description"></a><span data-ttu-id="ff765-106">Description</span><span class="sxs-lookup"><span data-stu-id="ff765-106">Description</span></span>

<span data-ttu-id="ff765-107">L’exemple suivant d’une demande PlayOnPhoneGreeting montre comment former une demande pour émettre un appel et lire le message d’accueil normal sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="ff765-107">The following example of a PlayOnPhoneGreeting request shows how to form a request to make an outbound call and play the normal greeting message on a telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="ff765-108">Code</span><span class="sxs-lookup"><span data-stu-id="ff765-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a><span data-ttu-id="ff765-109">Exemple de réponse PlayOnPhoneGreeting réussie</span><span class="sxs-lookup"><span data-stu-id="ff765-109">Successful PlayOnPhoneGreeting response example</span></span>

### <a name="description"></a><span data-ttu-id="ff765-110">Description</span><span class="sxs-lookup"><span data-stu-id="ff765-110">Description</span></span>

<span data-ttu-id="ff765-111">Une réponse PlayOnPhoneGreeting l’exemple suivant montre une réponse à la demande PlayOnPhoneGreeting.</span><span class="sxs-lookup"><span data-stu-id="ff765-111">The following example of a PlayOnPhoneGreeting response shows a response to the PlayOnPhoneGreeting request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ff765-112">Code</span><span class="sxs-lookup"><span data-stu-id="ff765-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ff765-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff765-113">See also</span></span>



[<span data-ttu-id="ff765-114">PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ff765-114">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
[<span data-ttu-id="ff765-115">PlayOnPhoneGreetingResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ff765-115">PlayOnPhoneGreetingResponse (UM web service)</span></span>](playonphonegreetingresponse-um-web-service.md)
  
[<span data-ttu-id="ff765-116">GreetingType (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ff765-116">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md)
  
[<span data-ttu-id="ff765-117">dialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ff765-117">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

