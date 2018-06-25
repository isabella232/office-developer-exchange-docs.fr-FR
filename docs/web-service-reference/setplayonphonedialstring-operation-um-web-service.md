---
title: Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser en tant que la valeur par défaut pour l’opération PlayOnPhone (service web de messagerie unifiée) et l’opération PlayOnPhoneGreeting (service web de messagerie unifiée).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="91964-103">Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="91964-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="91964-104">L’opération SetPlayOnPhoneDialString définit la chaîne de numérotation à utiliser en tant que la valeur par défaut pour l' [opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et l' [opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="91964-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="91964-105">Exemple de requête SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="91964-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="91964-106">Description</span><span class="sxs-lookup"><span data-stu-id="91964-106">Description</span></span>

<span data-ttu-id="91964-107">Une demande de SetPlayOnPhoneDialString l’exemple suivant montre comment créer une requête pour définir la chaîne de numérotation par défaut pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="91964-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="91964-108">Code</span><span class="sxs-lookup"><span data-stu-id="91964-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="91964-109">Exemple de réponse SetPlayOnPhoneDialString réussie</span><span class="sxs-lookup"><span data-stu-id="91964-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="91964-110">Description</span><span class="sxs-lookup"><span data-stu-id="91964-110">Description</span></span>

<span data-ttu-id="91964-111">Une réponse SetPlayOnePhoneDialString l’exemple suivant montre une réponse à la demande SetPlayOnPhoneDialString.</span><span class="sxs-lookup"><span data-stu-id="91964-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="91964-112">Code</span><span class="sxs-lookup"><span data-stu-id="91964-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="91964-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="91964-113">See also</span></span>



[<span data-ttu-id="91964-114">SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="91964-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="91964-115">SetPlayOnPhoneDialStringResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="91964-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
[<span data-ttu-id="91964-116">dialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="91964-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

