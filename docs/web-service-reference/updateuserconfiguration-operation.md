---
title: Opération UpdateUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfiguration
api_type:
- schema
ms.assetid: eda73b62-6a3a-43ae-8fd9-f30892811f27
description: L’opération UpdateUserConfiguration met à jour un objet de configuration utilisateur sur un dossier.
ms.openlocfilehash: 95fe6518fa30104463ec7f0aec8f786183eb513b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468543"
---
# <a name="updateuserconfiguration-operation"></a><span data-ttu-id="b63f9-103">Opération UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63f9-103">UpdateUserConfiguration operation</span></span>

<span data-ttu-id="b63f9-104">L’opération **UpdateUserConfiguration** met à jour un objet de configuration utilisateur sur un dossier.</span><span class="sxs-lookup"><span data-stu-id="b63f9-104">The **UpdateUserConfiguration** operation updates a user configuration object on a folder.</span></span> 
  
## <a name="updateuserconfiguration-request-example"></a><span data-ttu-id="b63f9-105">Exemple de requête UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63f9-105">UpdateUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="b63f9-106">Description</span><span class="sxs-lookup"><span data-stu-id="b63f9-106">Description</span></span>

<span data-ttu-id="b63f9-107">L’exemple de requête **UpdateUserConfiguration** suivant montre comment créer une demande de mise à jour d’un objet de configuration utilisateur dans le dossier Brouillons.</span><span class="sxs-lookup"><span data-stu-id="b63f9-107">The following example of an **UpdateUserConfiguration** request shows how to form a request to update a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b63f9-108">Code</span><span class="sxs-lookup"><span data-stu-id="b63f9-108">Code</span></span>

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
    <m:UpdateUserConfiguration>
      <m:UserConfiguration>
        <t:UserConfigurationName Name="TestConfig">
          <t:DistinguishedFolderId Id="drafts"/>
        </t:UserConfigurationName>
        <t:Dictionary>
          <t:DictionaryEntry>
            <t:DictionaryKey>
              <t:Type>String</t:Type>
              <t:Value>PhoneNumber</t:Value>
            </t:DictionaryKey>
            <t:DictionaryValue>
              <t:Type>String</t:Type>
              <t:Value>111-111-5555</t:Value>
            </t:DictionaryValue>
          </t:DictionaryEntry>
        </t:Dictionary>
      </m:UserConfiguration>
    </m:UpdateUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="updateuserconfiguration-response-example"></a><span data-ttu-id="b63f9-109">Exemple de réponse UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="b63f9-109">UpdateUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="b63f9-110">Description</span><span class="sxs-lookup"><span data-stu-id="b63f9-110">Description</span></span>

<span data-ttu-id="b63f9-111">L’exemple suivant montre une réponse réussie à la demande **UpdateUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="b63f9-111">The following example shows a successful response to the **UpdateUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="b63f9-112">Code</span><span class="sxs-lookup"><span data-stu-id="b63f9-112">Code</span></span>

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
    <m:UpdateUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UpdateUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UpdateUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:UpdateUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b63f9-113">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b63f9-113">See also</span></span>



[<span data-ttu-id="b63f9-114">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b63f9-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="b63f9-115">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b63f9-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

