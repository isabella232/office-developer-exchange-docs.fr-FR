---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: L’élément UserOofSettings spécifie les paramètres hors Office (OOF).
ms.openlocfilehash: 0fa550a97464414570faf391d3633243ff2e2144
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513968"
---
# <a name="useroofsettings"></a>UserOofSettings

**L’élément UserOofSettings** spécifie les paramètres De Office (OOF). 
  
[SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
  
[UserOofSettings](useroofsettings.md)
  
```xml
<UserOofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</UserOofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Définit l’état d’absence du travail de l’utilisateur.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Définit ou contient une valeur qui détermine à qui les messages d’absence du système externes sont envoyés.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Spécifie la durée pendant laquelle l’état d’absence du travail est activé si l’élément [OofState](oofstate.md) est définie sur **Scheduled**. Si [l’élément OofState](oofstate.md) est activé ou **désactivé,** la valeur de cet élément est ignorée.   <br/> |
|[InternalReply](internalreply.md) <br/> |Contient la réponse OOF envoyée à d’autres utilisateurs dans le domaine ou les domaines de confiance de l’utilisateur.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contient la réponse OOF envoyée aux adresses en dehors du domaine du destinataire ou des domaines de confiance.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Contient les arguments utilisés pour définir les paramètres et les messages d’absence du travail d’un utilisateur de boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une demande SetUserOofSettings définit OoFState sur **Enabled,** définit la durée de l’absence du travail pendant 10 jours et définit les messages d’absence du travail internes et externes.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

