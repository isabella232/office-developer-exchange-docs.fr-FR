---
title: Opération GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Trouvez des informations sur l’opération EWS GetAppMarketplaceUrl.
ms.openlocfilehash: f9dd41a43b92910ec596b95a0ce1e99a239ba01e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530089"
---
# <a name="getappmarketplaceurl-operation"></a>Opération GetAppMarketplaceUrl

Trouvez des informations sur l’opération EWS **GetAppMarketplaceUrl.** 
  
**L’opération GetAppMarketplaceUrl** récupère l’URL de l’app marketplace qu’un client peut visiter pour acquérir des applications à installer dans une boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getappmarketplaceurl-operation"></a>Utilisation de l’opération GetAppMarketplaceUrl

**L’opération GetAppMarketplaceUrl** ne prend aucun argument pour demander l’URL de la place de marché à partir de laquelle un client peut installer des applications. La réponse contient une URL vers le marketplace de l’application. 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a>En-têtes SOAP de l’opération GetAppMarketplaceUrl

**L’opération GetAppMarketplaceUrl** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a>Exemple de demande d’opération GetAppMarketplaceUrl : obtenir l’URL du marketplace d’application pour une boîte aux lettres

L’exemple suivant **d’une demande d’opération GetAppMarketplaceUrl** montre comment obtenir l’URL de l’application Marketplace pour une boîte aux lettres. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la requête contient les éléments suivants :
  
- [GetAppMarketplaceUrl](getappmarketplaceurl.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a>Réponse de l’opération GetAppMarketplaceUrl réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetAppMarketplaceUrl** pour obtenir l’URL du marketplace d’application pour une boîte aux lettres. 
  
> [!NOTE]
> L’URL du marketplace de l’application a été modifiée pour préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse contient les éléments suivants :
  
- [GetAppMarketplaceUrlResponse](getappmarketplaceurlresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [AppMarketplaceUrl](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a>Réponse d’erreur d’opération GetAppMarketPlaceUrl

Les erreurs renvoyées pour cette opération sont liées à une configuration de service incorrecte ou sont des erreurs EWS génériques. Pour les codes d’erreur qui sont génériques pour EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md). 
  
L’exemple suivant montre une réponse d’erreur qui est renvoyée lorsque le Exchange de configuration externe (ECP) n’est pas configuré.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse d’erreur contient les éléments suivants :
  
- [GetAppMarketplaceUrlResponse](getappmarketplaceurlresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération DisableApp](disableapp-operation.md)
    
- [Opération InstallApp](installapp-operation.md)
    
- [Opération UninstallApp](uninstallapp-operation.md)
    
- [Opération GetAppManifests](getappmanifests-operation.md)
    

