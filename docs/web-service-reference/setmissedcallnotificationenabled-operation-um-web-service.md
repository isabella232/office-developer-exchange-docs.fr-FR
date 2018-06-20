---
title: Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: L’opération SetMissedCallNotificationEnabled Active ou désactive les notifications d’appels manqués.
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="7058a-103">Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7058a-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="7058a-104">L’opération SetMissedCallNotificationEnabled Active ou désactive les notifications d’appels manqués.</span><span class="sxs-lookup"><span data-stu-id="7058a-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="7058a-105">Exemple de requête SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="7058a-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="7058a-106">Description</span><span class="sxs-lookup"><span data-stu-id="7058a-106">Description</span></span>

<span data-ttu-id="7058a-107">L’exemple suivant d’une demande SetMissedCallNotificationEnabled montre comment former une demande pour activer les notifications d’appels manqués.</span><span class="sxs-lookup"><span data-stu-id="7058a-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="7058a-108">Code</span><span class="sxs-lookup"><span data-stu-id="7058a-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="7058a-109">Exemple de réponse SetMissedCallNotificationEnabled réussie</span><span class="sxs-lookup"><span data-stu-id="7058a-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="7058a-110">Description</span><span class="sxs-lookup"><span data-stu-id="7058a-110">Description</span></span>

<span data-ttu-id="7058a-111">Une réponse PlayOnPhoneGreeting l’exemple suivant montre une réponse à la demande SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="7058a-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7058a-112">Code</span><span class="sxs-lookup"><span data-stu-id="7058a-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="7058a-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7058a-113">See also</span></span>



[<span data-ttu-id="7058a-114">SetMissedCallNotificationEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7058a-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="7058a-115">SetMissedCallNotificationEnabledResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7058a-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="7058a-116">État (service web de messagerie unifiée - SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="7058a-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

