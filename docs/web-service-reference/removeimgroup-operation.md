---
title: Opération RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Opération de recherche plus d’informations sur la RemoveImGroup EWS.
ms.openlocfilehash: 85b312f0b156125a2d5395658ccea06d831abdde
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829097"
---
# <a name="removeimgroup-operation"></a>Opération RemoveImGroup

Trouvez des informations sur l’opération EWS **RemoveImGroup** . 
  
L’opération **RemoveImGroup** supprime un groupe (IM) de messagerie instantané à partir d’une boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-removeimgroup-operation"></a>Utilisation de l’opération RemoveImGroup

L’opération **RemoveImGroup** prend uniquement un argument d’identificateur de groupe unique. 
  
### <a name="removeimgroup-operation-soap-headers"></a>En-têtes SOAP RemoveImGroup opération

L’opération **RemoveImGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a>Exemple de requête d’opération RemoveImGroup

Une demande d’opération **RemoveImGroup** l’exemple suivant montre comment supprimer un groupe de messagerie instantanée. 
  
> [!NOTE]
> L’ID de groupe a été raccourcie afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

La demande SOAP body contient les éléments suivants :
  
- [RemoveImGroup](removeimgroup.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a>Réponse d’opération RemoveImGroup réussie

L’exemple suivant montre une réponse positive à une demande d’opération **RemoveImGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a>Opération RemoveImGroup ErrorInvalidImGroupId réponse d’erreur

L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImGroup** . La réponse d’erreur se produit lorsqu’une tentative est effectuée pour supprimer un groupe qui n’existe pas dans la boîte aux lettres. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a>Opération RemoveImGroup ErrorInvalidIdMalformed réponse d’erreur

L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImGroup** . La réponse d’erreur se produit lorsqu’une tentative est effectuée pour supprimer un groupe avec un identificateur de groupe au format incorrect. 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [RemoveImGroupResponse](removeimgroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Personnes et contacts dans EWS dans Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Opération AddImGroup](addimgroup-operation.md)
    
- [Opération SetImGroup](setimgroup-operation.md)
    

