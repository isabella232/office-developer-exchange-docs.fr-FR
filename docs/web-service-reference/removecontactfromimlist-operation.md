---
title: Opération RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Opération de recherche plus d’informations sur la RemoveContactFromImList EWS.
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829080"
---
# <a name="removecontactfromimlist-operation"></a>Opération RemoveContactFromImList

Trouvez des informations sur l’opération EWS **RemoveContactFromImList** . 
  
L’opération **RemoveContactFromImList** supprime les contacts de la liste de la messagerie instantanée (MI) de Lync lorsque Lync utilise Exchange pour le magasin de contacts. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Utilisation de l’opération RemoveContactFromImList

L’opération **RemoveContactFromImList** accepte un argument unique qui identifie un contact à supprimer de la liste des contacts Lync stockée sur un serveur Exchange. La liste des contacts que les objectifs de cette opération est appelée **Contacts Lync** dans Outlook 2013. 
  
> [!CAUTION]
> N’utilisez pas l' [opération DeleteItem](deleteitem-operation.md) pour supprimer des contacts à partir d’une liste de contacts. Traitement côté serveur supplémentaire devront se produisent pour prendre en charge la suppression d’un contact dans la liste de **Contacts Lync** . Notez que la liste de **Contacts Lync** est l’équivalent conceptuelle du dossier par défaut **Contacts Lync** boîte aux lettres. 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>En-têtes SOAP RemoveContactFromImList opération

L’opération **RemoveContactFromImList** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Exemple de requête d’opération RemoveContactFromImList : supprimer un contact de la liste de Contacts Lync

Une demande d’opération **RemoveContactFromImList** l’exemple suivant montre comment supprimer un contact de la liste de **Contacts Lync** . L’opération **RemoveContactFromImList** accepte un identificateur contact unique pour identifier le contact est supprimé de la liste de **Contacts Lync** . 
  
> [!NOTE]
> Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

Les éléments suivants sont utilisés dans la demande SOAP body :
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Réponse d’opération RemoveContactFromImList réussie

L’exemple suivant montre une réponse positive à une demande d’opération **RemoveContactFromImList** pour supprimer un contact dans la liste de **Contacts Lync** . 
  
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
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

Les éléments suivants sont utilisés dans la réponse SOAP body :
  
- [RemoveContactFromImListResponse](removecontactfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Réponse d’erreur d’opération RemoveContactFromImList

L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveContactFromImList** . Il s’agit d’une réponse à une demande pour supprimer un contact dans la liste de **Contacts Lync** lorsque le contact n’existe plus dans la liste. 
  
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
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    

