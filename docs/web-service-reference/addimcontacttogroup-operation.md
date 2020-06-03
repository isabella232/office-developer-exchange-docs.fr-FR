---
title: Opération AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Trouvez des informations sur l’opération EWS AddImContactToGroup.
ms.openlocfilehash: a69ee0b355e78e1249383cab612a75bcda8d9e8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458410"
---
# <a name="addimcontacttogroup-operation"></a>Opération AddImContactToGroup

Trouvez des informations sur l’opération EWS **AddImContactToGroup** . 
  
L’opération **AddImContactToGroup** les services Web Exchange (EWS) ajoute un contact de messagerie instantanée à un groupe. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-addimcontacttogroup-operation"></a>Utilisation de l’opération AddImContactToGroup

L’opération **AddImContactToGroup** peut accepter uniquement les contacts de messagerie instantanée. Si vous souhaitez ajouter un nouveau contact de messagerie instantanée au magasin de contacts unifié, utilisez l’opération [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) . 
  
L’opération **AddImContactToGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
**Tableau 1. En-têtes SOAP d’opération AddImContactToGroup**

|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a>Exemple de requête d’opération AddImContactToGroup : ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantanée

L’exemple suivant de demande d’opération **AddImContactToGroup** indique comment ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantanée. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

Le corps SOAP de la demande contient les éléments suivants :
  
- [AddImContactToGroup](addimcontacttogroup.md)
    
- [Mettez](contactid.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a>Réponse de l’opération AddImContactToGroup réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **AddImContactToGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a>AddImContactToGroup Operation ErrorInvalidImContactId Error Response

L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddImContactToGroup** . La réponse d’erreur suivante se produit lors d’une tentative d’ajout d’un contact qui n’est pas un contact de messagerie instantanée. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opération AddImGroup](addimgroup-operation.md)
    
- [Opération AddNewImContactToGroup](addnewimcontacttogroup-operation.md)
    
- [Opération SetImGroup](setimgroup-operation.md)
    
- [Opération RemoveImGroup](removeimgroup-operation.md)
    
- [Opération GetImItemList](getimitemlist-operation.md)
    
- [Personnes et contacts dans EWS dans Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

