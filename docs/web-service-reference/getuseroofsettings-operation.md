---
title: Opération GetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: L’opération GetUserOofSettings obtient les messages et les paramètres d’absence du Bureau d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 622faa622b0ea231a6331ff62631885d4252c1f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457696"
---
# <a name="getuseroofsettings-operation"></a>Opération GetUserOofSettings

L’opération **GetUserOofSettings** obtient les messages et les paramètres d’absence du Bureau d’un utilisateur de boîte aux lettres. 
  
## <a name="soap-headers"></a>En-têtes SOAP

L’opération **GetUserOofSettings** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a>Utilisation de l’opération GetUserOofSettings

L’opération **GetUserOofSettings** permet d’accéder aux paramètres OOF d’un utilisateur. Un utilisateur est identifié par l’adresse e-mail de l’utilisateur. Si le message d’absence du Bureau est null et que le Bureau d’attente est activé, aucun message d’absence du Bureau n’est envoyé. 
  
> [!IMPORTANT]
> Si les messages OOF sont définis par MicrosoftOfficeOutlook, cette opération renverra les messages OOF au format HTML. 
  
## <a name="getuseroofsettings-request-example"></a>Exemple de requête GetUserOofSettings

### <a name="description"></a>Description

L’exemple suivant montre une requête **GetUserOofSettings** qui récupère les informations du Bureau d’veille d’un utilisateur unique. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
    
- [Boîte aux lettres (disponibilité)](mailbox-availability.md)
    
- [Address (chaîne)](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a>Exemple de réponse GetUserOofSettings réussi

### <a name="description"></a>Description

L’exemple suivant montre un État OOF désactivé avec les messages OOF.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a>Éléments Response GetUserOofSettings réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
    
- [ResponseMessage](responsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [OofSettings](oofsettings.md)
    
- [OofState](oofstate.md)
    
- [ExternalAudience](externalaudience.md)
    
- [Durée (UserOofSettings)](duration-useroofsettings.md)
    
- [StartTime](starttime.md)
    
- [EndTime](endtime.md)
    
- [InternalReply](internalreply.md)
    
- [ExternalReply](externalreply.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [AllowExternalOof](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a>Exemple de réponse d’erreur GetUserOofSettings

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur causée par une tentative d’accès aux informations d’absence du Bureau d’un autre utilisateur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

