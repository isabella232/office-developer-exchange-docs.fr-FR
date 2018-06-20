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
description: L’opération DeleteUserConfiguration supprime un objet de configuration utilisateur dans un dossier.
ms.openlocfilehash: 033134a7e16aa8e7a3d6b928141012b646863a68
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755875"
---
# <a name="deleteuserconfiguration-operation"></a><span data-ttu-id="ee119-103">Opération DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee119-103">DeleteUserConfiguration operation</span></span>

<span data-ttu-id="ee119-104">L’opération **DeleteUserConfiguration** supprime un objet de configuration utilisateur dans un dossier.</span><span class="sxs-lookup"><span data-stu-id="ee119-104">The **DeleteUserConfiguration** operation deletes a user configuration object on a folder.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="ee119-105">L’opération **DeleteUserConfiguration** déclenche un événement de déplacement pour le système de notification d’événement.</span><span class="sxs-lookup"><span data-stu-id="ee119-105">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="ee119-106">L’objet de configuration utilisateur est déplacée vers la benne.</span><span class="sxs-lookup"><span data-stu-id="ee119-106">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="deleteuserconfiguration-request-example"></a><span data-ttu-id="ee119-107">Exemple de requête DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee119-107">DeleteUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="ee119-108">Description</span><span class="sxs-lookup"><span data-stu-id="ee119-108">Description</span></span>

<span data-ttu-id="ee119-109">L’exemple suivant d’une demande **DeleteUserConfiguration** montre comment former une demande pour supprimer un objet de configuration utilisateur dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="ee119-109">The following example of a **DeleteUserConfiguration** request shows how to form a request to delete a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee119-110">Code</span><span class="sxs-lookup"><span data-stu-id="ee119-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

## <a name="deleteuserconfiguration-response-example"></a><span data-ttu-id="ee119-111">Exemple de réponse DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ee119-111">DeleteUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="ee119-112">Description</span><span class="sxs-lookup"><span data-stu-id="ee119-112">Description</span></span>

<span data-ttu-id="ee119-113">L’exemple suivant montre une réponse positive à la demande **DeleteUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="ee119-113">The following example shows a successful response to the **DeleteUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee119-114">Code</span><span class="sxs-lookup"><span data-stu-id="ee119-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:DeleteUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="ee119-115">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ee119-115">See also</span></span>

- [<span data-ttu-id="ee119-116">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ee119-116">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="ee119-117">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ee119-117">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

