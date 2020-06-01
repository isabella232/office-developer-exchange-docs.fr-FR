---
title: Opération GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: 070cbfe5-325a-4955-8e4a-8230ea0459a7
description: L’opération GetServiceConfiguration obtient des informations de configuration pour le type de service spécifié. Cette opération peut retourner des paramètres de configuration pour la messagerie unifiée, les règles de protection et les services de messagerie.
ms.openlocfilehash: b8ea2cef366a52765850dddcc8c1ef1e8fa68b22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460910"
---
# <a name="getserviceconfiguration-operation"></a><span data-ttu-id="abe2b-104">Opération GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="abe2b-104">GetServiceConfiguration operation</span></span>

<span data-ttu-id="abe2b-105">L’opération **GetServiceConfiguration** obtient des informations de configuration pour le type de service spécifié.</span><span class="sxs-lookup"><span data-stu-id="abe2b-105">The **GetServiceConfiguration** operation gets configuration information for the specified type of service.</span></span> <span data-ttu-id="abe2b-106">Cette opération peut retourner des paramètres de configuration pour la messagerie unifiée, les règles de protection et les services de messagerie.</span><span class="sxs-lookup"><span data-stu-id="abe2b-106">This operation can return configuration settings for the Unified Messaging, Protection Rules, and Mail Tips services.</span></span> 
  
## <a name="getserviceconfiguration-request-example"></a><span data-ttu-id="abe2b-107">Exemple de requête GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="abe2b-107">GetServiceConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="abe2b-108">Description</span><span class="sxs-lookup"><span data-stu-id="abe2b-108">Description</span></span>

<span data-ttu-id="abe2b-109">L’exemple de requête **GetServiceConfiguration** suivant montre comment créer une demande pour obtenir des informations de configuration pour le service de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="abe2b-109">The following example of a **GetServiceConfiguration** request shows how to form a request to get configuration information for the Unified Messaging service.</span></span> 
  
### <a name="code"></a><span data-ttu-id="abe2b-110">Code</span><span class="sxs-lookup"><span data-stu-id="abe2b-110">Code</span></span>

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
    <m:GetServiceConfiguration>
      <m:RequestedConfiguration>
        <m:ConfigurationName>UnifiedMessagingConfiguration</m:ConfigurationName>
      </m:RequestedConfiguration>
    </m:GetServiceConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getserviceconfiguration-response-example"></a><span data-ttu-id="abe2b-111">Exemple de réponse GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="abe2b-111">GetServiceConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="abe2b-112">Description</span><span class="sxs-lookup"><span data-stu-id="abe2b-112">Description</span></span>

<span data-ttu-id="abe2b-113">L’exemple suivant montre une réponse réussie à la demande **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="abe2b-113">The following example shows a successful response to the **GetServiceConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="abe2b-114">Code</span><span class="sxs-lookup"><span data-stu-id="abe2b-114">Code</span></span>

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
    <GetServiceConfigurationResponse ResponseClass="Success" 
                                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <ResponseMessages>
        <ServiceConfigurationResponseMessageType ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <m:UnifiedMessagingConfiguration xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
            <t:UmEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:UmEnabled>
            <t:PlayOnPhoneDialString xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">user@contoso.com</t:PlayOnPhoneDialString>
            <t:PlayOnPhoneEnabled xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">true</t:PlayOnPhoneEnabled>
          </m:UnifiedMessagingConfiguration>
        </ServiceConfigurationResponseMessageType>
      </ResponseMessages>
    </GetServiceConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="getserviceconfiguration-error-response-example"></a><span data-ttu-id="abe2b-115">Exemple de réponse d’erreur GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="abe2b-115">GetServiceConfiguration Error response example</span></span>

### <a name="description"></a><span data-ttu-id="abe2b-116">Description</span><span class="sxs-lookup"><span data-stu-id="abe2b-116">Description</span></span>

<span data-ttu-id="abe2b-117">L’exemple suivant montre une réponse d’erreur à la demande **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="abe2b-117">The following example shows an error response to the **GetServiceConfiguration** request.</span></span> <span data-ttu-id="abe2b-118">Cette erreur est due à un nom de configuration incorrect.</span><span class="sxs-lookup"><span data-stu-id="abe2b-118">This error was caused by an incorrect configuration name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="abe2b-119">Code</span><span class="sxs-lookup"><span data-stu-id="abe2b-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: 
      The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
      is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
      datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType' 
      - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>13</t:LineNumber>
          <t:LinePosition>62</t:LinePosition>
          <t:Violation>The 'https://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
          is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
          datatype 'https://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType'
          - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="abe2b-120">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="abe2b-120">See also</span></span>



[<span data-ttu-id="abe2b-121">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="abe2b-121">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="abe2b-122">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="abe2b-122">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

