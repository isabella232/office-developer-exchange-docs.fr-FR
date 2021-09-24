---
title: Opération GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Trouvez des informations sur l’opération EWS GetAppManifests.
ms.openlocfilehash: 979a09d24d0c9365a92e589aa169bebf2340411b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509916"
---
# <a name="getappmanifests-operation"></a>Opération GetAppManifests

Trouvez des informations sur l’opération EWS **GetAppManifests.** 
  
**L’opération GetAppManifests récupère** les manifestes d’application. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getappmanifests-operation"></a>Utilisation de l’opération GetAppManifests

**L’opération GetAppManifests ne** prend aucun argument pour demander les manifestes d’application pour une boîte aux lettres. La réponse contient des fichiers manifeste XML codés en base 64 pour chaque application installée dans une boîte aux lettres. 
  
### <a name="getappmanifests-operation-soap-headers"></a>En-têtes SOAP de l’opération GetAppManifests

**L’opération GetAppManifests peut** utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a>Exemple de demande d’opération GetAppManifests : obtenir les manifestes d’application pour une boîte aux lettres

L’exemple suivant **d’une demande d’opération GetAppManifests** montre comment obtenir les manifestes d’application pour une boîte aux lettres. [L’élément ApiVersionSupported](apiversionsupported.md) et l’élément [SchemaVersionSupported](schemaversionsupported.md) sont facultatifs. 
  
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

Le corps SOAP de la requête contient l’élément suivant :
  
- [GetAppManifests](getappmanifests.md)
    
- [ApiVersionSupported](apiversionsupported.md)
    
- [SchemaVersionSupported](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a>Réponse de l’opération GetAppManifests réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetAppManifests** pour obtenir les manifestes d’application d’une boîte aux lettres. 
  
> [!NOTE]
> Tous les manifestes d’application base64 ont été arbitrairement tronqués pour préserver la lisibilité. 
  
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

Le corps SOAP de la réponse contient les éléments suivants :
  
- [GetAppManifestsResponse](getappmanifestsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Applications](apps.md)
    
- [Application](app.md)
    
- [Manifeste](manifest.md)
    
Le corps SOAP de la réponse peut également contenir l’élément suivant :
  
- [Manifestes](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a>Réponse d’erreur de l’opération GetAppManifests

Les erreurs renvoyées pour cette opération sont liées à un format non valide des paramètres d’entrée ou sont des erreurs EWS génériques. Pour les codes d’erreur qui sont génériques pour EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
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
    

