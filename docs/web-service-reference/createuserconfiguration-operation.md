---
title: Opération CreateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfiguration
api_type:
- schema
ms.assetid: eb5b8ab6-9743-481c-aac9-f9aa889bd353
description: L’opération CreateUserConfiguration crée un objet de configuration utilisateur sur un dossier.
ms.openlocfilehash: 5f0eb7d18736008af39199cbc52cc3a6e6abda09
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755739"
---
# <a name="createuserconfiguration-operation"></a><span data-ttu-id="81cbe-103">Opération CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="81cbe-103">CreateUserConfiguration operation</span></span>

<span data-ttu-id="81cbe-104">L’opération **CreateUserConfiguration** crée un objet de configuration utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="81cbe-104">The **CreateUserConfiguration** operation creates a user configuration object on a folder.</span></span> 
  
## <a name="createuserconfiguration-request-example"></a><span data-ttu-id="81cbe-105">Exemple de requête CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="81cbe-105">CreateUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="81cbe-106">Description</span><span class="sxs-lookup"><span data-stu-id="81cbe-106">Description</span></span>

<span data-ttu-id="81cbe-107">L’exemple suivant d’une demande **CreateUserConfiguration** montre comment former une demande pour créer un objet de configuration utilisateur dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="81cbe-107">The following example of a **CreateUserConfiguration** request shows how to form a request to create a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="81cbe-108">Code</span><span class="sxs-lookup"><span data-stu-id="81cbe-108">Code</span></span>

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
    <m:CreateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts">
          </t:DistinguishedFolderId>
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>555-555-1111</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>  
    </m:CreateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="createuserconfiguration-response-example"></a><span data-ttu-id="81cbe-109">Exemple de réponse CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="81cbe-109">CreateUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="81cbe-110">Description</span><span class="sxs-lookup"><span data-stu-id="81cbe-110">Description</span></span>

<span data-ttu-id="81cbe-111">L’exemple suivant montre une réponse positive à la demande **CreateUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="81cbe-111">The following example shows a successful response to the **CreateUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="81cbe-112">Code</span><span class="sxs-lookup"><span data-stu-id="81cbe-112">Code</span></span>

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
    <m:CreateUserConfigurationResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:CreateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:CreateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="81cbe-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="81cbe-113">See also</span></span>



[<span data-ttu-id="81cbe-114">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="81cbe-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="81cbe-115">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="81cbe-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

