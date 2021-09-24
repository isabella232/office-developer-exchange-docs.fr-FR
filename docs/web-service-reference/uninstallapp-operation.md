---
title: Opération UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Trouvez des informations sur l’opération EWS UninstallApp.
ms.openlocfilehash: 8a301360b2b4c38d85e8c5be2e80c79378d0fd97
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527145"
---
# <a name="uninstallapp-operation"></a>Opération UninstallApp

Trouvez des informations sur l’opération EWS **UninstallApp.** 
  
**L’opération UninstallApp** désinstalle une application de messagerie pour Outlook. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-uninstallapp-operation"></a>Utilisation de l’opération UninstallApp

**L’opération UninstallApp** prend un argument dans la demande qui identifie l’application de messagerie à désinstaller. 
  
### <a name="uninstallapp-operation-soap-headers"></a>En-têtes SOAP de l’opération UninstallApp

**L’opération UninstallApp** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a>Exemple de demande d’opération UninstallApp : Désinstaller une application de messagerie dans une boîte aux lettres

L’exemple suivant **d’une demande d’opération UninstallApp** montre comment désinstaller une application de messagerie à l’aide de l’identificateur d’application. L’identificateur d’application se trouve dans le manifeste de l’application qui est renvoyé par [l’opération GetAppManifests](getappmanifests-operation.md).
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

Le corps SOAP de la requête contient les éléments suivants :
  
- [UninstallApp](uninstallapp.md)
    
- [ID (String)](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a>Réponse de l’opération UninstallApp réussie

L’exemple suivant montre une réponse réussie à **une demande d’opération UninstallApp** pour désinstaller une application de messagerie. 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de la réponse contient les éléments suivants :
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a>Réponse d’erreur d’opération UninstallApp

L’exemple suivant montre une réponse d’erreur à **une demande d’opération UninstallApp.** Il s’agit d’une réponse à une demande de désinstallation d’une application de messagerie qui a déjà été désinstallée. 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse d’erreur contient les éléments suivants :
  
- [UninstallAppResponse](uninstallappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour obtenir des codes d’erreur supplémentaires génériques pour EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération InstallApp](installapp-operation.md)
    
- [Opération DisableApp](disableapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Opération GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

