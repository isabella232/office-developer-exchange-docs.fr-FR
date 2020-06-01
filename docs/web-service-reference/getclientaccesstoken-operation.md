---
title: Opération GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Trouvez des informations sur l’opération EWS GetClientAccessToken.
ms.openlocfilehash: 2d49d675fcedb0e7e8312a9715f095c47fcf3d77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462037"
---
# <a name="getclientaccesstoken-operation"></a>Opération GetClientAccessToken

Trouvez des informations sur l’opération EWS **GetClientAccessToken** . 
  
L’opération **GetClientAccessToken** obtient un jeton d’accès client pour une application de messagerie pour Outlook. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getclientaccesstoken-operation"></a>Utilisation de l’opération GetClientAccessToken

La demande d’opération **GetClientAccessToken** prend deux arguments obligatoires : l’identificateur de l’application et le type de jeton. Vous pouvez utiliser l' [opération GetAppManifests](getappmanifests-operation.md) pour demander l’identificateur de l’application. 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a>En-têtes SOAP d’opération GetClientAccessToken

L’opération **GetClientAccessToken** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a>Exemple de requête d’opération GetClientAccessToken : obtenir un jeton d’identité de l’appelant

L’exemple suivant de demande d’opération **GetClientAccessToken** montre comment obtenir un jeton d’identité de l’appelant pour une application. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la demande contient les éléments suivants :
  
- [GetClientAccessToken](getclientaccesstoken.md)
    
- [TokenRequests](tokenrequests.md)
    
- [TokenRequest](tokenrequest.md)
    
- [ID (chaîne)](id-string.md)
    
- [TokenType](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a>Réponse de l’opération GetClientAccessToken réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetClientAccessToken** pour obtenir un jeton d’identité de l’appelant pour une application. 
  
> [!NOTE]
> Les valeurs de jeton de cet article ont été raccourcies afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Jeton (ClientAccessTokenType)](token-clientaccesstokentype.md)
    
- [ID (chaîne)](id-string.md)
    
- [TokenType (ClientAccessTokenType)](tokentype-clientaccesstokentype.md)
    
- [TokenValue](tokenvalue.md)
    
- [TTL (ClientAccessTokenTypeType)](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a>Réponse d’erreur d’opération GetClientAccessToken

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetClientAccessToken** . Il s’agit d’une réponse à une demande d’obtention d’un jeton de rappel d’extension sans les autorisations appropriées. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [GetClientAccessTokenResponse](getclientaccesstokenresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetClientAccessTokenResponseMessage](getclientaccesstokenresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetAppManifests](getappmanifests-operation.md)
    
- [Compléments Outlook](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

