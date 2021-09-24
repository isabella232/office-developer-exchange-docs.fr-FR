---
title: Opération GetFederationInformation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: L’opération GetFederationInformation fournit des informations sur l’état de fédération de l’organisation, telles que l’URI cible à utiliser lors de la demande de jetons destinés à cette organisation, ainsi que les autres domaines que l’organisation a également fédérés.
ms.openlocfilehash: 915498440e4bc3d7262ed3a55350f7d3723d47d8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529953"
---
# <a name="getfederationinformation-operation-soap"></a>Opération GetFederationInformation (SOAP)

L’opération **GetFederationInformation** fournit des informations sur l’état de fédération de l’organisation, telles que l’URI cible à utiliser lors de la demande de jetons destinés à cette organisation, ainsi que les autres domaines que l’organisation a également fédérés. 
  
Seules les organisations fédérées peuvent partager des calendriers, des contacts et des messages à des utilisateurs externes.
  
## <a name="getfederationinformation-request-example"></a>Exemple de requête GetFederationInformation

### <a name="description"></a>Description

L’exemple suivant **d’une demande GetFederationInformation** affiche une demande pour les informations de fédération d’un utilisateur. Le client envoie cette demande au serveur. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="https://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="https://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">https://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [GetFederationInformationRequestMessage (SOAP)](getfederationinformationrequestmessage-soap.md)
    
- [Request (SOAP)](request-soap.md)
    
- [Domaine (SOAP)](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a>Exemple de réponse GetFederationInformation

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la **demande GetFederationInformation** que le serveur envoie au client. 
  
### <a name="code"></a>Code

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="https://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a>Éléments de réponse

Les éléments suivants sont utilisés dans la réponse :
  
- [GetFederationInformationResponseMessage (SOAP)](getfederationinformationresponsemessage-soap.md)
    
- [Response (SOAP)](response-soap.md)
    
- [ErrorCode (SOAP)](errorcode-soap.md)
    
- [ErrorMessage (SOAP)](errormessage-soap.md)
    
- [ApplicationUri (SOAP)](applicationuri-soap.md)
    
- [Domaines (SOAP)](domains-soap.md)
    
- [Domaine (SOAP)](domain-soap.md)
    
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

