---
title: Opération GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Trouvez des informations sur l’opération EWS GetAppManifests.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463005"
---
# <a name="getappmanifests-operation"></a>Opération GetAppManifests

Trouvez des informations sur l’opération EWS **GetAppManifests** . 
  
L’opération **GetAppManifests** récupère les manifestes d’application. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getappmanifests-operation"></a>Utilisation de l’opération GetAppManifests

L’opération **GetAppManifests** ne prend aucun argument pour demander les manifestes d’application pour une boîte aux lettres. La réponse contient des fichiers manifeste XML codés en base64 pour chaque application installée dans une boîte aux lettres. 
  
### <a name="getappmanifests-operation-soap-headers"></a>En-têtes SOAP d’opération GetAppManifests

L’opération **GetAppManifests** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>Exemple de requête d’opération GetAppManifests : obtenir les manifestes d’application pour une boîte aux lettres

L’exemple suivant de demande d’opération **GetAppManifests** indique comment obtenir les manifestes d’application pour une boîte aux lettres. L’élément [ApiVersionSupported](apiversionsupported.md) et l’élément [SchemaVersionSupported](schemaversionsupported.md) sont facultatifs. 
  
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
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la demande contient l’élément suivant :
  
- [GetAppManifests](getappmanifests.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>Réponse de l’opération GetAppManifests réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetAppManifests** pour obtenir les manifestes d’application pour une boîte aux lettres. 
  
> [!NOTE]
> Tous les manifestes d’application base64 ont été tronqués de manière arbitraire afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetAppManifestsResponse](getappmanifestsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Applications](apps.md)
    
- [App](app.md)
    
- [Manifeste](manifest.md)
    
Le corps SOAP de la réponse peut également contenir l’élément suivant :
  
- [Manifestes](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>Réponse d’erreur d’opération GetAppManifests

Les erreurs renvoyées pour cette opération sont liées à un format non valide des paramètres d’entrée ou sont des erreurs EWS génériques. Pour les codes d’erreur génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération DisableApp](disableapp-operation.md)
    
- [Opération InstallApp](installapp-operation.md)
    
- [Opération UninstallApp](uninstallapp-operation.md)
    
- [Opération GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

