---
title: Opération RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Trouvez des informations sur l’opération RemoveDistributionGroupFromImList EWS.
ms.openlocfilehash: 52b653008b7b14d2c2467cc9bb1f8f1475cee8f5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513394"
---
# <a name="removedistributiongroupfromimlist-operation"></a>Opération RemoveDistributionGroupFromImList

Trouvez des informations **sur l’opération RemoveDistributionGroupFromImList** EWS. 
  
**L’opération RemoveDistributionGroupFromImList** supprime un groupe de distribution de la liste de messagerie instantanée Lync lorsque Lync utilise Exchange pour le magasin de contacts. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a>Utilisation de l’opération RemoveDistributionGroupFromImList

**L’opération RemoveDistributionGroupFromImList** accepte un seul argument qui identifie un groupe de distribution à supprimer de la liste de messagerie instantanée Lync stockée sur un Exchange serveur. 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a>En-têtes SOAP d’opération RemoveDistributionGroupFromImList

**L’opération RemoveDistributionGroupFromImList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité. Cet en-tête s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la RFC 3066, « Balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a>Exemple de demande d’opération RemoveDistributionGroupFromImList : supprimer un groupe de distribution d’une liste de messagerie instantanée

L’exemple suivant **d’une demande d’opération RemoveDistributionGroupFromImList** montre comment supprimer un groupe de distribution d’un groupe de messagerie instantanée. **L’opération RemoveDistributionGroupFromImList** accepte l’identificateur de groupe unique pour identifier le groupe de distribution à supprimer de la liste de messagerie instantanée. [L’élément ExchangeStoreId](exchangestoreid.md) renvoyé dans la réponse pour l’opération [GetImItemList](getimitemlist-operation.md) et l’opération [AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) identifie les groupes de distribution qui peuvent être supprimés de la liste de messagerie instantanée. 
  
> [!NOTE]
> Tous les identificateurs d’élément et les touches de modification de cet article ont été raccourcis pour préserver la lisibilité. 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

Les éléments suivants sont utilisés dans le corps SOAP de la requête :
  
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a>Réponse de l’opération RemoveDistributionGroupFromImList réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveDistributionGroupFromImList** pour supprimer un groupe de distribution d’un groupe de messagerie instantanée. 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

Les éléments suivants sont utilisés dans le corps SOAP de la réponse :
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a>Exemple de réponse d’erreur d’opération RemoveDistributionGroupFromImList

L’exemple suivant montre une réponse d’erreur à **une demande d’opération RemoveDistributionGroupFromImList.** Il s’agit d’une réponse à une demande de suppression d’un groupe de distribution qui a déjà été supprimé de la boîte aux lettres. 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetImItemList](getimitemlist-operation.md)
    
- [Opération AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md)
    
- [Personnes et contacts dans EWS dans Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

