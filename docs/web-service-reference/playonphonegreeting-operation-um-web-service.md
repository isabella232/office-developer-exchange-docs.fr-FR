---
title: Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)
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
description: L’opération PlayOnPhoneGreeting effectue un appel sortant et joue l’un des deux messages de salutation sur le téléphone.
ms.openlocfilehash: 3af120b9ac8d7a368742fad2850c924228488662
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528894"
---
# <a name="playonphonegreeting-operation-um-web-service"></a><span data-ttu-id="96915-103">Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="96915-103">PlayOnPhoneGreeting operation (UM web service)</span></span>

<span data-ttu-id="96915-104">L’opération PlayOnPhoneGreeting effectue un appel sortant et joue l’un des deux messages de salutation sur le téléphone.</span><span class="sxs-lookup"><span data-stu-id="96915-104">The PlayOnPhoneGreeting operation makes an outbound call and plays one of the two greeting messages on the telephone.</span></span>
  
## <a name="playonphonegreeting-request-example"></a><span data-ttu-id="96915-105">Exemple de requête PlayOnPhoneGreeting</span><span class="sxs-lookup"><span data-stu-id="96915-105">PlayOnPhoneGreeting request example</span></span>

### <a name="description"></a><span data-ttu-id="96915-106">Description</span><span class="sxs-lookup"><span data-stu-id="96915-106">Description</span></span>

<span data-ttu-id="96915-107">L’exemple de requête PlayOnPhoneGreeting suivant montre comment créer une demande d’émission d’un appel sortant et lire le message d’accueil normal sur un téléphone.</span><span class="sxs-lookup"><span data-stu-id="96915-107">The following example of a PlayOnPhoneGreeting request shows how to form a request to make an outbound call and play the normal greeting message on a telephone.</span></span>
  
### <a name="code"></a><span data-ttu-id="96915-108">Code</span><span class="sxs-lookup"><span data-stu-id="96915-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhoneGreeting xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GreetingType>NormalCustom</GreetingType>
      <DialString>12345</DialString>
    </PlayOnPhoneGreeting>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphonegreeting-response-example"></a><span data-ttu-id="96915-109">Exemple de réponse PlayOnPhoneGreeting réussi</span><span class="sxs-lookup"><span data-stu-id="96915-109">Successful PlayOnPhoneGreeting response example</span></span>

### <a name="description"></a><span data-ttu-id="96915-110">Description</span><span class="sxs-lookup"><span data-stu-id="96915-110">Description</span></span>

<span data-ttu-id="96915-111">L’exemple suivant de réponse PlayOnPhoneGreeting indique une réponse à la demande PlayOnPhoneGreeting.</span><span class="sxs-lookup"><span data-stu-id="96915-111">The following example of a PlayOnPhoneGreeting response shows a response to the PlayOnPhoneGreeting request.</span></span>
  
### <a name="code"></a><span data-ttu-id="96915-112">Code</span><span class="sxs-lookup"><span data-stu-id="96915-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneGreetingResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <PlayOnPhoneGreetingResponse>MjA4MTQ5MmItMTBmZC00ZGFmLThiMzEtNDllNDJjM2Y3MjIxQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneGreetingResponse> 
    </PlayOnPhoneGreetingResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="96915-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="96915-113">See also</span></span>



[<span data-ttu-id="96915-114">PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="96915-114">PlayOnPhoneGreeting (UM web service)</span></span>](playonphonegreeting-um-web-service.md)
  
[<span data-ttu-id="96915-115">PlayOnPhoneGreetingResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="96915-115">PlayOnPhoneGreetingResponse (UM web service)</span></span>](playonphonegreetingresponse-um-web-service.md)
  
[<span data-ttu-id="96915-116">GreetingType (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="96915-116">GreetingType (UM web service)</span></span>](greetingtype-um-web-service.md)
  
[<span data-ttu-id="96915-117">dialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="96915-117">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

