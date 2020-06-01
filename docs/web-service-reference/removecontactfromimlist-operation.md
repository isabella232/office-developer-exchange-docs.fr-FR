---
title: Opération RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Trouvez des informations sur l’opération EWS RemoveContactFromImList.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458466"
---
# <a name="removecontactfromimlist-operation"></a>Opération RemoveContactFromImList

Trouvez des informations sur l’opération EWS **RemoveContactFromImList** . 
  
L’opération **RemoveContactFromImList** supprime les contacts de la liste de messagerie instantanée Lync lorsque Lync utilise Exchange pour le magasin de contacts. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Utilisation de l’opération RemoveContactFromImList

L’opération **RemoveContactFromImList** accepte un seul argument qui identifie un contact à supprimer de la liste des contacts Lync stockée sur un serveur Exchange. La liste des contacts ciblés par cette opération est appelée **contacts Lync** dans Outlook 2013. 
  
> [!CAUTION]
> N’utilisez pas l' [opération DeleteItem](deleteitem-operation.md) pour supprimer des contacts d’une liste de contacts. Un traitement supplémentaire côté serveur peut être nécessaire pour prendre en charge la suppression d’un contact de la liste de **contacts Lync** . Notez que la liste de **contacts Lync** est l’équivalent conceptuel du dossier de boîte aux lettres **contacts Lync** par défaut. 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>En-têtes SOAP d’opération RemoveContactFromImList

L’opération **RemoveContactFromImList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemple de requête d’opération RemoveContactFromImList : supprimer un contact de la liste de contacts Lync

L’exemple suivant de demande d’opération **RemoveContactFromImList** montre comment supprimer un contact de la liste de **contacts Lync** . L’opération **RemoveContactFromImList** accepte un seul identificateur de contact unique pour identifier le contact qui est supprimé de la liste de **contacts Lync** . 
  
> [!NOTE]
> Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

Les éléments suivants sont utilisés dans le corps SOAP de la demande :
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [Mettez](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Réponse de l’opération RemoveContactFromImList réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveContactFromImList** pour supprimer un contact de la liste de **contacts Lync** . 
  
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
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

Les éléments suivants sont utilisés dans le corps SOAP de réponse :
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Réponse d’erreur d’opération RemoveContactFromImList

L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveContactFromImList** . Réponse à une demande de suppression d’un contact de la liste de **contacts Lync** lorsque le contact n’existe plus dans la liste. 
  
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
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetImItemList](getimitemlist-operation.md)
    

