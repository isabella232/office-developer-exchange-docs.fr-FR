---
title: Opération GetUMProperties (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: L’opération GetUMProperties Obtient toutes les propriétés de la messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827678"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="0eaa3-103">Opération GetUMProperties (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0eaa3-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="0eaa3-104">L’opération GetUMProperties Obtient toutes les propriétés de la messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="0eaa3-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="0eaa3-105">Exemple de requête GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="0eaa3-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="0eaa3-106">Description</span><span class="sxs-lookup"><span data-stu-id="0eaa3-106">Description</span></span>

<span data-ttu-id="0eaa3-107">L’exemple suivant d’une demande GetUMProperties montre comment former une demande pour obtenir les propriétés d’une boîte aux lettres de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="0eaa3-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="0eaa3-108">Code</span><span class="sxs-lookup"><span data-stu-id="0eaa3-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="0eaa3-109">Exemple de réponse GetUMProperties réussie</span><span class="sxs-lookup"><span data-stu-id="0eaa3-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="0eaa3-110">Description</span><span class="sxs-lookup"><span data-stu-id="0eaa3-110">Description</span></span>

<span data-ttu-id="0eaa3-111">Une réponse GetUMProperties l’exemple suivant montre une réponse à la demande GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="0eaa3-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="0eaa3-112">Code</span><span class="sxs-lookup"><span data-stu-id="0eaa3-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="0eaa3-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0eaa3-113">See also</span></span>



[<span data-ttu-id="0eaa3-114">GetUMProperties (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0eaa3-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="0eaa3-115">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="0eaa3-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

