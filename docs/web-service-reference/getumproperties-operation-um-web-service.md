---
title: Opération GetUMProperties (service Web de messagerie unifiée)
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
description: L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.
ms.openlocfilehash: 42176d9cd0288af6515aeea616a4f216a419410c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462471"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="85ef2-103">Opération GetUMProperties (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="85ef2-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="85ef2-104">L’opération GetUMProperties obtient toutes les propriétés de messagerie unifiée pour la boîte aux lettres de l’utilisateur qui effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="85ef2-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="85ef2-105">Exemple de requête GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="85ef2-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="85ef2-106">Description</span><span class="sxs-lookup"><span data-stu-id="85ef2-106">Description</span></span>

<span data-ttu-id="85ef2-107">L’exemple de requête GetUMProperties suivant montre comment créer une demande pour obtenir les propriétés de messagerie unifiée d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="85ef2-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="85ef2-108">Code</span><span class="sxs-lookup"><span data-stu-id="85ef2-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="85ef2-109">Exemple de réponse GetUMProperties réussi</span><span class="sxs-lookup"><span data-stu-id="85ef2-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="85ef2-110">Description</span><span class="sxs-lookup"><span data-stu-id="85ef2-110">Description</span></span>

<span data-ttu-id="85ef2-111">L’exemple suivant de réponse GetUMProperties indique une réponse à la demande GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="85ef2-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="85ef2-112">Code</span><span class="sxs-lookup"><span data-stu-id="85ef2-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a><span data-ttu-id="85ef2-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85ef2-113">See also</span></span>



[<span data-ttu-id="85ef2-114">GetUMProperties (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="85ef2-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="85ef2-115">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="85ef2-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

