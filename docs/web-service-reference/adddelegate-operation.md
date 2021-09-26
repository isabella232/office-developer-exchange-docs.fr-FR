---
title: Opération AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 012d8cc5-648c-4ba0-a155-15c422b1e994
description: L’opération AddDelegate ajoute un ou plusieurs délégués à la boîte aux lettres d’un principal et définit des autorisations d’accès spécifiques.
ms.openlocfilehash: 687080c58a0dbde2ddb0f0049b96d543204c6018
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543813"
---
# <a name="adddelegate-operation"></a>Opération AddDelegate

**L’opération AddDelegate ajoute** un ou plusieurs délégués à la boîte aux lettres d’un principal et définit des autorisations d’accès spécifiques. 
  
## <a name="soap-headers"></a>En-têtes SOAP

**L’opération AddDelegate peut** utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
   
## <a name="adddelegate-request-example"></a>Exemple de requête AddDelegate

### <a name="description"></a>Description

L’exemple suivant d’une **demande AddDelegate** illustre une tentative d’accorder à l’utilisateur 1 des autorisations de délégué sur les dossiers dont est propriétaire user2. User1 se voir donner des autorisations au niveau de l’auteur sur le dossier Calendrier de l’utilisateur2 et des autorisations au niveau du réviseur sur le dossier Contacts de l’utilisateur2. User1 ne recevra pas de copies des messages de réunion et ne pourra pas afficher les éléments privés dans la boîte aux lettres de l’utilisateur 2. Les demandes de réunion sont envoyées à user1 et user2. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

L’exemple suivant **d’une réponse AddDelegate** affiche une réponse réussie à **une demande AddDelegate.** 
  
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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           ResponseClass="Success" 
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

L’exemple suivant montre la réponse à une demande d’ajout d’un délégué qui a déjà été ajouté à la boîte aux lettres du principal.
  
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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:AddDelegateResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                           ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Si le code de réponse ErrorDelegateAlreadyExists est renvoyé lorsque vous essayez d’ajouter un délégué, utilisez l’opération [GetDelegate](getdelegate-operation.md) pour obtenir toutes les autorisations actuelles pour le délégué, puis utilisez l’opération [UpdateDelegate](updatedelegate-operation.md) pour définir les nouvelles autorisations. 
  
## <a name="see-also"></a>Voir aussi

- [Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

