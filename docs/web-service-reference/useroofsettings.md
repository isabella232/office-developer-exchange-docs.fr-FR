---
title: UserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserOofSettings
api_type:
- schema
ms.assetid: 0a95ca63-660e-4cc0-82e4-3f74fb4ae21c
description: L’élément UserOofSettings spécifie les paramètres d’absence du bureau (OOF).
ms.openlocfilehash: a035fd89387ece632d83f5f72a564e4896bc6753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838969"
---
# <a name="useroofsettings"></a>UserOofSettings

L’élément **UserOofSettings** spécifie les paramètres d’absence du bureau (OOF). 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Définit l’état d’absence du bureau de l’utilisateur.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Définit ou contient une valeur qui détermine les messages d’absence du bureau externes qui sont envoyés.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Spécifie la durée pour laquelle le statut d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur **planifiées**. Si l’élément [OofState](oofstate.md) est défini sur **activé** ou **désactivé**, la valeur de cet élément est ignorée.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contient la réponse d’absence du bureau envoyée à d’autres utilisateurs dans le domaine de l’utilisateur ou de domaines approuvés.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contient la réponse d’absence du bureau envoyée aux adresses à l’extérieur du destinataire ou les domaines approuvés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Contient les arguments permet de définir les paramètres d’absence du bureau et des messages d’un utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant d’une demande SetUserOofSettings définit le OoFState sur **activé**, définit la durée d’absence du bureau pour 10 jours et définit les messages d’absence du bureau internes et externes.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

