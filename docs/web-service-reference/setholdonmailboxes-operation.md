---
title: Opération SetHoldOnMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9015a0d8-3495-461b-aa79-797d23169585
description: Opération de recherche plus d’informations sur la SetHoldOnMailboxes EWS.
ms.openlocfilehash: 1091ed14ceb25dfd275499b9db47ae4e41b5f1a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829412"
---
# <a name="setholdonmailboxes-operation"></a>Opération SetHoldOnMailboxes

Trouvez des informations sur l’opération EWS **SetHoldOnMailboxes** . 
  
L’opération **SetHoldOnMailboxes** définit une stratégie de blocage de boîtes aux lettres sur les boîtes aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-setholdonmailboxes-operation"></a>Utilisation de l’opération SetHoldOnMailboxes

L’opération **SetHoldOnMailboxes** définit un blocage de boîtes aux lettres sur un ou plusieurs boîtes aux lettres. 
  
### <a name="setholdonmailboxes-operation-soap-headers"></a>En-têtes SOAP SetHoldOnMailboxes opération

L’opération **SetHoldOnMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="setholdonmailboxes-operation-request-example-apply-a-hold-on-a-mailbox"></a>Exemple de requête d’opération SetHoldOnMailboxes : appliquer un blocage sur une boîte aux lettres

Une demande d’opération **SetHoldOnMailboxes** l’exemple suivant montre comment appliquer un blocage sur deux boîtes aux lettres. La suspension de la boîte aux lettres a été créée à l’aide de la commande [New-MailboxSearch](http://technet.microsoft.com/en-us/library/dd298064.aspx) . 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:SetHoldOnMailboxes>
         <m:ActionType>Create</m:ActionType>
         <m:HoldId>HoldId2</m:HoldId>
         <m:Query>test</m:Query>
         <m:Mailboxes>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</t:String>
            <t:String>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</t:String>
         </m:Mailboxes>
         <m:Language>English</m:Language>
         <m:IncludeNonIndexableItems>false</m:IncludeNonIndexableItems>
         <m:Deduplication>true</m:Deduplication>
      </m:SetHoldOnMailboxes>
   </soap:Body>
</soap:Envelope>

```

La demande SOAP body contient les éléments suivants :
  
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [ActionType (HoldActionType)](actiontype-holdactiontype.md)
    
- [HoldId](holdid.md)
    
- [Query](query.md)
    
- [Boîtes aux lettres (ArrayOfStringsType)](mailboxes-arrayofstringstype.md)
    
- [Chaîne](string.md)
    
- [Language](language.md)
    
- [IncludeNonIndexableItems](includenonindexableitems.md)
    
- [Déduplication](deduplication.md)
    
## <a name="successful-setholdonmailboxes-operation-response"></a>Réponse d’opération SetHoldOnMailboxes réussie

L’exemple suivant montre une réponse positive à une demande d’opération **SetHoldOnMailboxes** pour mettre les deux boîtes aux lettres en attente. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <SetHoldOnMailboxesResponse ResponseClass="Success" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <MailboxHoldResult>
            <HoldId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">HoldId2</HoldId>
            <Query xmlns="http://schemas.microsoft.com/exchange/services/2006/types">test</Query>
            <MailboxHoldStatuses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <MailboxHoldStatus>
                  <Mailbox>o=First/ou=Exchange(DLT)/cn=Recipients/cn=1fa441ff5e4749ba43ecc0fd94c21adf-Willi</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
               <MailboxHoldStatus>
                  <Mailbox>/o=First/ou=Exchange(DLT)/cn=Recipients/cn=aed2346adaa34ffc9f0f339917e8de95-Micha</Mailbox>
                  <Status>Pending</Status>
                  <AdditionalInfo/>
               </MailboxHoldStatus>
            </MailboxHoldStatuses>
         </MailboxHoldResult>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

La réponse SOAP body contient les éléments suivants :
  
- [SetHoldOnMailboxesResponse](setholdonmailboxesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [MailboxHoldResult](mailboxholdresult.md)
    
- [HoldId](holdid.md)
    
- [Query](query.md)
    
- [MailboxHoldStatuses](mailboxholdstatuses.md)
    
- [MailboxHoldStatus](mailboxholdstatus.md)
    
- [Boîte aux lettres (chaîne)](mailbox-string.md)
    
- [État (HoldStatusType)](status-holdstatustype.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="setholdonmailboxes-operation-error-response"></a>Réponse d’erreur d’opération SetHoldOnMailboxes

L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetHoldOnMailboxes** . Il s’agit d’une réponse à une demande qui contient un identificateur de boîte aux lettres spécifiée est incorrecte. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <SetHoldOnMailboxesResponse ResponseClass="Error" 
                                  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox is specified for hold operation. If specified in the request, then it could be the object does not exist in AD or is a Distribution Group.</MessageText>
         <ResponseCode>ErrorInvalidOperation</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetHoldOnMailboxesResponse>
   </s:Body>
</s:Envelope>

```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [SetHoldOnMailboxesResponse](setholdonmailboxesresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Opération SearchMailboxes](searchmailboxes-operation.md)
    
- [Opération GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)
    
- [Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

