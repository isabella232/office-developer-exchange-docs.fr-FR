---
title: Opération GetHoldOnMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9157f329-80b4-4cd0-a158-378064966ae6
description: Trouvez des informations sur l’opération EWS GetHoldOnMailboxes.
ms.openlocfilehash: 3e87aed618b98cbaf556b31f59365f5ed97bec85
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516992"
---
# <a name="getholdonmailboxes-operation"></a>Opération GetHoldOnMailboxes

> [!IMPORTANT]
> À compter du 1er avril 2020, l’opération GetHoldOnMailboxes ne sera plus disponible dans Exchange Online. Cette opération ne sera pas affectée dans les versions sur site de Exchange Server. Pour plus d’informations, [voir Retrait des outils eDiscovery hérités dans Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Trouvez des informations sur l’opération EWS **GetHoldOnMailboxes.** 
  
**L’opération GetHoldOnMailboxes** obtient les boîtes aux lettres qui sont placées dans une attente spécifique et la requête de hold associée. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getholdonmailboxes-operation"></a>Utilisation de l’opération GetHoldOnMailboxes

L’opération **GetHoldOnMailboxes** fournit au client des informations sur les boîtes aux lettres placées sous une mise en attente spécifique, des informations sur la requête de mise en attente associée à chaque mise en attente, le cas échéant, et des informations sur l’état de la mise en attente pour chaque boîte aux lettres. Pour plus d’informations sur les boîtes aux lettres en attente, y compris les attentes basées sur des requêtes, voir [In-Place Hold](https://technet.microsoft.com/library/ff637980%28v=exchg.150%29) on TechNet. 
  
### <a name="getholdonmailboxes-operation-soap-headers"></a>En-têtes SOAP d’opération GetHoldOnMailboxes

**L’opération GetHoldOnMailboxes peut** utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifie les rôles serveur nécessaires pour permettre à l’appelant d’effectuer la demande. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getholdonmailboxes-operation-request-example-get-mailbox-hold-information"></a>Exemple de demande d’opération GetHoldOnMailboxes : obtenir les informations de la boîte aux lettres

L’exemple suivant d’une demande d’opération **GetHoldOnMailboxes** montre comment obtenir les informations de la boîte aux lettres en attente pour la boîte aux lettres HoldId2. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetHoldOnMailboxes>
         <m:HoldId>HoldId2</m:HoldId>
      </m:GetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la requête contient les éléments suivants :
  
- [GetHoldOnMailboxes](getholdonmailboxes.md)
    
- [HoldId](holdid.md)
    
## <a name="successful-getholdonmailboxes-operation-response"></a>Réponse de l’opération GetHoldOnMailboxes réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetHoldOnMailboxes** pour obtenir les informations de la boîte aux lettres de la boîte aux lettres holdId2. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="https://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=ecc0fd98c2cadf-Willi</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First Organization/ou=Exchange Administrative Group (FYDIBPDLT)/cn=Recipients/cn=dasdat341q8de95-Micha</Mailbox>
                  <Status>OnHold</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse contient les éléments suivants :
  
- [GetHoldOnMailboxesResponse](getholdonmailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [MailboxHoldResult](mailboxholdresult.md)
    
- [HoldId](holdid.md)
    
- [Query](query.md)
    
- [MailboxHoldStatuses](mailboxholdstatuses.md)
    
- [MailboxHoldStatus](mailboxholdstatus.md)
    
- [Mailbox (String)](mailbox-string.md)
    
- [Status (HoldStatusType)](status-holdstatustype.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="getholdonmailboxes-operation-error-response"></a>Réponse d’erreur d’opération GetHoldOnMailboxes

L’exemple suivant montre une réponse d’erreur à **une demande d’opération GetHoldOnMailboxes.** Il s’agit d’une réponse à une demande d’obtenir une attente qui a été supprimée. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specific query-based hold is not found.</MessageText>
         <ResponseCode>ErrorMailboxHoldNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de réponse d’erreur contient les éléments suivants :
  
- [GetHoldOnMailboxesResponse](getholdonmailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour obtenir des codes d’erreur supplémentaires génériques pour EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Opération SearchMailboxes](searchmailboxes-operation.md)
    
- [Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

