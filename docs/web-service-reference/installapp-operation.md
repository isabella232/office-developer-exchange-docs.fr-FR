---
title: Opération InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Opération de recherche plus d’informations sur la InstallApp EWS.
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827951"
---
# <a name="installapp-operation"></a>Opération InstallApp

Trouvez des informations sur l’opération EWS **InstallApp** . 
  
L’opération **InstallApp** installe une application de messagerie pour Outlook dans une boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-installapp-operation"></a>Utilisation de l’opération InstallApp

L’opération **InstallApp** prend un argument unique qui identifie une application de messagerie à installer. L’argument contient le manifeste pour une application de messagerie codé en base64. 
  
### <a name="installapp-operation-soap-headers"></a>En-têtes SOAP InstallApp opération

L’opération **InstallApp** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a>Exemple de requête d’opération InstallApp : installer une application de messagerie dans une boîte aux lettres

Une requête d’opération **InstallApp** l’exemple suivant montre comment installer une application de messagerie pour Outlook. Vous trouverez le manifeste d’application à l’aide de l' [opération GetAppManifests](getappmanifests-operation.md).
  
> [!NOTE]
> Le manifeste d’application codé en base64 a été tronqué arbitrairement afin de préserver la lisibilité et ne représente pas un manifeste valid. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

La demande SOAP body contient les éléments suivants :
  
- [InstallApp](installapp.md)
    
- [Manifeste](manifest.md)
    
## <a name="successful-installapp-operation-response"></a>Réponse d’opération InstallApp réussie

L’exemple suivant montre une réponse positive à une demande d’opération **InstallApp** pour installer une application de messagerie. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [InstallAppResponse](installappresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="installapp-operation-error-response"></a>Réponse d’erreur d’opération InstallApp

L’exemple suivant montre une réponse d’erreur à une demande d’opération **InstallApp** . Il s’agit d’une réponse à une demande qui contient un manifeste non valide. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
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
    

