---
title: Opération GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Trouvez des informations sur l’opération EWS GetUserPhoto.
ms.openlocfilehash: 6769842d31519f0aac2cf9bda10c1cab70558301
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461813"
---
# <a name="getuserphoto-operation"></a>Opération GetUserPhoto

Trouvez des informations sur l’opération EWS **GetUserPhoto** . 
  
L’opération **GetUserPhoto** obtient une photo de l’utilisateur à partir des services de domaine Active Directory (AD DS). 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getuserphoto-operation"></a>Utilisation de l’opération GetUserPhoto

L’opération **RemoveContactFromImList** est une opération simple qui accepte l’adresse de messagerie d’un utilisateur et la taille de photo demandée et renvoie le flux de photos dans la réponse. 
  
> [!NOTE]
> EWS a une opération SOAP et une opération REST pour obtenir des photos de l’utilisateur. Pour plus d’informations sur l’interface REST, consultez la rubrique obtenir des photos de l' [utilisateur à l’aide d’EWS dans Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx). 
  
### <a name="getuserphoto-operation-soap-headers"></a>En-têtes SOAP d’opération GetUserPhoto

L’opération **GetUserPhoto** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a>Exemple de requête d’opération GetUserPhoto : obtenir la photo d’un utilisateur

L’exemple suivant de demande d’opération **GetUserPhoto** montre comment obtenir la photo d’un utilisateur. Cet exemple demande une photo d’utilisateur de 48 x 48 pixels. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Les éléments suivants sont utilisés dans le corps SOAP de la demande :
  
- [GetUserPhoto](getuserphoto.md)
    
- [E-mail (chaîne)](email-string.md)
    
- [SizeRequested](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a>Réponse de l’opération GetUserPhoto réussie

L’exemple suivant montre une réponse réussie à une opération **GetUserPhoto** pour obtenir la photo d’un utilisateur. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

Les éléments suivants sont utilisés dans le corps SOAP de réponse :
  
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [HasChanged](haschanged.md)
    
- [GetUserPhotoResponse](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a>Réponse d’erreur d’opération GetUserPhoto

L’enveloppe SOAP ne renvoie pas de code d’erreur si vous tentez d’obtenir une photo d’utilisateur pour une adresse de messagerie qui n’existe pas dans l’organisation. Un code d’état HTTP 500 sera renvoyé dans la réponse pour indiquer que la demande a échoué. 
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)   
- [Obtenir des photos de l’utilisateur à l’aide d’EWS dans Exchange](https://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

