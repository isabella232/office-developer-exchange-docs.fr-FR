---
title: Opération IsUMEnabled (service Web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: L’opération IsUMEnabled détermine si une boîte aux lettres est activée pour la messagerie unifiée.
ms.openlocfilehash: b1478f5a113059251fe1b036ac7d77e5a4ab4f50
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458235"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="ef4d8-103">Opération IsUMEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ef4d8-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="ef4d8-104">L’opération IsUMEnabled détermine si une boîte aux lettres est activée pour la messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="ef4d8-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="ef4d8-105">Exemple de requête IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="ef4d8-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="ef4d8-106">Description</span><span class="sxs-lookup"><span data-stu-id="ef4d8-106">Description</span></span>

<span data-ttu-id="ef4d8-107">L’exemple de requête IsUMEnabled suivant montre comment créer une demande pour déterminer si une boîte aux lettres est activée pour la messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="ef4d8-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef4d8-108">Code</span><span class="sxs-lookup"><span data-stu-id="ef4d8-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="ef4d8-109">Exemple de réponse IsUMEnabled réussi</span><span class="sxs-lookup"><span data-stu-id="ef4d8-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="ef4d8-110">Description</span><span class="sxs-lookup"><span data-stu-id="ef4d8-110">Description</span></span>

<span data-ttu-id="ef4d8-111">L’exemple suivant montre une réponse réussie à une demande IsUMEnabled.</span><span class="sxs-lookup"><span data-stu-id="ef4d8-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef4d8-112">Code</span><span class="sxs-lookup"><span data-stu-id="ef4d8-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ef4d8-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ef4d8-113">See also</span></span>



[<span data-ttu-id="ef4d8-114">IsUMEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ef4d8-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="ef4d8-115">IsUMEnabledResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="ef4d8-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="ef4d8-116">Éléments XML de service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ef4d8-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

