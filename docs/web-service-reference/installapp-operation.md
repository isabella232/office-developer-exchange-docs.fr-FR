---
title: Opération InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Trouvez des informations sur l’opération EWS InstallApp.
ms.openlocfilehash: ae6aab7f7176aa827bafa9abf1aa67d458d309d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465687"
---
# <a name="installapp-operation"></a>Opération InstallApp

Trouvez des informations sur l’opération EWS **InstallApp** . 
  
L’opération **InstallApp** installe une application de messagerie pour Outlook dans une boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-installapp-operation"></a>Utilisation de l’opération InstallApp

L’opération **InstallApp** prend un seul argument qui identifie une application de messagerie à installer. L’argument contient le manifeste encodé en base64 pour une application de messagerie. 
  
### <a name="installapp-operation-soap-headers"></a>En-têtes SOAP d’opération InstallApp

L’opération **InstallApp** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>Exemple de requête d’opération InstallApp : installer une application de messagerie dans une boîte aux lettres

L’exemple suivant de demande d’opération **InstallApp** indique comment installer une application de messagerie pour Outlook. Le manifeste de l’application peut être trouvé à l’aide de l' [opération GetAppManifests](getappmanifests-operation.md).
  
> [!NOTE]
> Le manifeste d’application encodé en base64 a été tronqué de manière arbitraire afin de préserver la lisibilité et ne représente pas un manifeste valide. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la demande contient les éléments suivants :
  
- [InstallApp](installapp.md)
    
- [Manifeste](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>Réponse de l’opération InstallApp réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **InstallApp** pour installer une application de messagerie. 
  
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
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>Réponse d’erreur d’opération InstallApp

L’exemple suivant montre une réponse d’erreur à une demande d’opération **InstallApp** . Il s’agit d’une réponse à une demande contenant un manifeste non valide. 
  
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
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [InstallAppResponse](installappresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération DisableApp](disableapp-operation.md)
    
- [Opération UninstallApp](uninstallapp-operation.md)
    
- [GetAppManifests](getappmanifests.md)
    
- [Opération GetAppMarketplaceUrl](getappmarketplaceurl-operation.md)
    

