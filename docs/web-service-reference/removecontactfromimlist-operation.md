---
title: Opération RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Trouvez des informations sur l’opération RemoveContactFromImList EWS.
ms.openlocfilehash: cc72dc1b0abf9032fabafbaac53d29f41968dafb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523585"
---
# <a name="removecontactfromimlist-operation"></a>Opération RemoveContactFromImList

Trouvez des informations sur **l’opération RemoveContactFromImList** EWS. 
  
**L’opération RemoveContactFromImList** supprime les contacts de la liste de messagerie instantanée Lync lorsque Lync utilise Exchange pour le magasin de contacts. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Utilisation de l’opération RemoveContactFromImList

**L’opération RemoveContactFromImList** accepte un seul argument qui identifie un contact à supprimer de la liste de contacts Lync stockée sur un Exchange serveur. La liste des contacts que cette opération cible est appelée **Contacts Lync** Outlook 2013. 
  
> [!CAUTION]
> N’utilisez pas [l’opération DeleteItem](deleteitem-operation.md) pour supprimer des contacts d’une liste de contacts. Un traitement côté serveur supplémentaire peut être dû à la prise en charge de la suppression d’un contact de la **liste des contacts Lync.** Notez que la **liste de contacts Lync** est l’équivalent conceptuel du dossier de boîte aux lettres **de contacts Lync** par défaut. 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>En-têtes SOAP d’opération RemoveContactFromImList

**L’opération RemoveContactFromImList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la RFC 3066, « Balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemple de demande d’opération RemoveContactFromImList : supprimer un contact de la liste des contacts Lync

L’exemple suivant **d’une demande d’opération RemoveContactFromImList** montre comment supprimer un contact de la liste **des contacts Lync.** **L’opération RemoveContactFromImList** accepte un identificateur de contact unique unique pour identifier le contact supprimé de la liste des **contacts Lync.** 
  
> [!NOTE]
> Tous les identificateurs d’élément et les touches de modification de cet article ont été raccourcis pour préserver la lisibilité. 
  
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

Les éléments suivants sont utilisés dans le corps SOAP de la requête :
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Réponse de l’opération RemoveContactFromImList réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveContactFromImList** pour supprimer un contact de la liste des **contacts Lync.** 
  
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

Les éléments suivants sont utilisés dans le corps SOAP de la réponse :
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Réponse d’erreur d’opération RemoveContactFromImList

L’exemple suivant montre une réponse d’erreur à **une demande d’opération RemoveContactFromImList.** Il s’agit d’une réponse à une demande de suppression d’un contact de la liste des **contacts Lync** lorsque le contact n’existe plus dans la liste. 
  
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

Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetImItemList](getimitemlist-operation.md)
    

