---
title: Opération GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Opération de recherche plus d’informations sur la GetUserPhoto EWS.
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827694"
---
# <a name="getuserphoto-operation"></a>Opération GetUserPhoto

Trouvez des informations sur l’opération EWS **GetUserPhoto** . 
  
L’opération **GetUserPhoto** Obtient une photo de l’utilisateur des Services de domaine Active Directory (AD DS). 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Utilisation de l’opération GetUserPhoto

L’opération **RemoveContactFromImList** est une opération simple qui accepte une adresse de messagerie d’un utilisateur et la taille de photo demandé et retourne le flux de photos dans la réponse. 
  
> [!NOTE]
> EWS dispose d’un SOAP et une opération basée sur REST pour obtenir les photos de l’utilisateur. Pour plus d’informations sur l’interface REST, voir [obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx). 
  
### <a name="getuserphoto-operation-soap-headers"></a>En-têtes SOAP GetUserPhoto opération

L’opération **GetUserPhoto** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Exemple de requête d’opération GetUserPhoto : obtenir la photo d’un utilisateur

Une demande d’opération **GetUserPhoto** l’exemple suivant montre comment obtenir la photo d’un utilisateur. Cet exemple demande une photo de l’utilisateur qui est de 48 x 48 pixels. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

Les éléments suivants sont utilisés dans la demande SOAP body :
  
- [GetUserPhoto](getuserphoto.md)
    
- [Courrier électronique (chaîne)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Réponse d’opération GetUserPhoto réussie

L’exemple suivant montre une réponse positive à une opération **GetUserPhoto** pour obtenir la photo d’un utilisateur. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

Les éléments suivants sont utilisés dans la réponse SOAP body :
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Réponse d’erreur d’opération GetUserPhoto

L’enveloppe SOAP ne renvoie un code d’erreur si une tentative est effectuée pour obtenir une photo de l’utilisateur pour une adresse de messagerie qui n’existe pas dans l’organisation. Un code d’état HTTP 500 s’afficheront dans la réponse pour indiquer que la demande a échoué. 
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)   
- [Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

