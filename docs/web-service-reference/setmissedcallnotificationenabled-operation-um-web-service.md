---
title: Opération SetMissedCallNotificationEnabled (service Web de messagerie unifiée)
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
description: L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467395"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="7de1b-103">Opération SetMissedCallNotificationEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7de1b-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="7de1b-104">L’opération SetMissedCallNotificationEnabled active ou désactive les notifications d’appels manqués.</span><span class="sxs-lookup"><span data-stu-id="7de1b-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="7de1b-105">Exemple de requête SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="7de1b-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="7de1b-106">Description</span><span class="sxs-lookup"><span data-stu-id="7de1b-106">Description</span></span>

<span data-ttu-id="7de1b-107">L’exemple de requête SetMissedCallNotificationEnabled suivant montre comment créer une demande pour activer les notifications d’appels manqués.</span><span class="sxs-lookup"><span data-stu-id="7de1b-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="7de1b-108">Code</span><span class="sxs-lookup"><span data-stu-id="7de1b-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="7de1b-109">Exemple de réponse SetMissedCallNotificationEnabled réussi</span><span class="sxs-lookup"><span data-stu-id="7de1b-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="7de1b-110">Description</span><span class="sxs-lookup"><span data-stu-id="7de1b-110">Description</span></span>

<span data-ttu-id="7de1b-111">L’exemple suivant de réponse PlayOnPhoneGreeting indique une réponse à la demande SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="7de1b-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7de1b-112">Code</span><span class="sxs-lookup"><span data-stu-id="7de1b-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="7de1b-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7de1b-113">See also</span></span>



[<span data-ttu-id="7de1b-114">SetMissedCallNotificationEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7de1b-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="7de1b-115">SetMissedCallNotificationEnabledResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7de1b-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="7de1b-116">État (service Web de messagerie unifiée-SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="7de1b-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

