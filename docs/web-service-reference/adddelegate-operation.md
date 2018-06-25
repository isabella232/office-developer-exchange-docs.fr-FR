---
title: Opération AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: L’opération AddDelegate ajoute un ou plusieurs délégués à la boîte aux lettres d’une entité de sécurité et définit les autorisations d’accès spécifiques.
ms.openlocfilehash: 28d4ded2625efc3d6eade44f5fafc06c2ffca7ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755159"
---
# <a name="adddelegate-operation"></a>Opération AddDelegate

L’opération **AddDelegate** ajoute un ou plusieurs délégués à la boîte aux lettres d’une entité de sécurité et définit les autorisations d’accès spécifiques. 
  
## <a name="soap-headers"></a>En-têtes SOAP

L’opération **AddDelegate** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
   
## <a name="adddelegate-request-example"></a>Exemple de requête AddDelegate

### <a name="description"></a>Description

L’exemple suivant d’une demande **AddDelegate** indique une tentative de donner user1 déléguer des autorisations sur les dossiers qui appartiennent à l’utilisateur 2. User1 bénéficie des autorisations au niveau de l’auteur à du user2 dossier de calendrier et autorisations de niveau relecteur au dossier Contacts de l’utilisateur 2. User1 ne recevra pas les copies des messages de réunion et ne pourront pas afficher les éléments privés dans la boîte aux lettres de l’utilisateur 2. Les demandes de réunion envoyés à user1 et user2. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <AddDelegate>
      <Mailbox>
        <t:EmailAddress>user2@example.com</t:EmailAddress>
      </Mailbox>
      <DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>user1@example.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Author</t:CalendarFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Reviewer</t:ContactsFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </DelegateUsers>
      <DeliverMeetingRequests>DelegatesAndMe</DeliverMeetingRequests>
    </AddDelegate>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-response-example"></a>Exemple de réponse AddDelegate

### <a name="description"></a>Description

L’exemple suivant d’une réponse **AddDelegate** montre une réponse positive à une demande de **AddDelegate** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
              <t:UserId>
                <t:SID>S-1-5-21-1333220396-2200287332-232816053-1116</t:SID>
                <t:PrimarySmtpAddress>User1@example.com</t:PrimarySmtpAddress>
                <t:DisplayName>User1</t:DisplayName>
              </t:UserId>
              <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
            </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="adddelegate-error-response-example"></a>Exemple de réponse d’erreur AddDelegate

### <a name="description"></a>Description

L’exemple suivant montre la réponse à une demande pour ajouter un délégué qui a déjà été ajouté à la boîte aux lettres de l’entité de sécurité.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is already a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorDelegateAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:AddDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Si le code de réponse ErrorDelegateAlreadyExists est renvoyé lorsque vous essayez d’ajouter un délégué, l' [opération GetDelegate](getdelegate-operation.md) permet d’obtenir toutes les autorisations pour le délégué en cours, puis utilisez l' [opération UpdateDelegate](updatedelegate-operation.md) pour définir les nouvelles autorisations. 
  
## <a name="see-also"></a>Voir aussi

- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

