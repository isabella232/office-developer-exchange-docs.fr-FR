---
title: Opération DeleteUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 93e44690-be2d-4fdb-96a8-4ded3c193aed
description: L’opération DeleteUserConfiguration supprime un objet de configuration utilisateur sur un dossier.
ms.openlocfilehash: 064e1ace2c2f51783431ce42670b2a4fd8146b54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44451466"
---
# <a name="deleteuserconfiguration-operation"></a><span data-ttu-id="628dd-103">Opération DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="628dd-103">DeleteUserConfiguration operation</span></span>

<span data-ttu-id="628dd-104">L’opération **DeleteUserConfiguration** supprime un objet de configuration utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="628dd-104">The **DeleteUserConfiguration** operation deletes a user configuration object on a folder.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="628dd-105">L’opération **DeleteUserConfiguration** déclenchera un événement Move pour le système de notification d’événements.</span><span class="sxs-lookup"><span data-stu-id="628dd-105">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="628dd-106">L’objet de configuration utilisateur est déplacé vers la benne.</span><span class="sxs-lookup"><span data-stu-id="628dd-106">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="deleteuserconfiguration-request-example"></a><span data-ttu-id="628dd-107">Exemple de requête DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="628dd-107">DeleteUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="628dd-108">Description</span><span class="sxs-lookup"><span data-stu-id="628dd-108">Description</span></span>

<span data-ttu-id="628dd-109">L’exemple de requête **DeleteUserConfiguration** suivant montre comment créer une demande de suppression d’un objet de configuration utilisateur dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="628dd-109">The following example of a **DeleteUserConfiguration** request shows how to form a request to delete a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="628dd-110">Code</span><span class="sxs-lookup"><span data-stu-id="628dd-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:DeleteUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
    </m:DeleteUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="deleteuserconfiguration-response-example"></a><span data-ttu-id="628dd-111">Exemple de réponse DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="628dd-111">DeleteUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="628dd-112">Description</span><span class="sxs-lookup"><span data-stu-id="628dd-112">Description</span></span>

<span data-ttu-id="628dd-113">L’exemple suivant montre une réponse réussie à la demande **DeleteUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="628dd-113">The following example shows a successful response to the **DeleteUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="628dd-114">Code</span><span class="sxs-lookup"><span data-stu-id="628dd-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:DeleteUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="628dd-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="628dd-115">See also</span></span>

- [<span data-ttu-id="628dd-116">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="628dd-116">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="628dd-117">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="628dd-117">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

