---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: L’élément InternalReply contient la réponse d’absence du Bureau envoyée aux autres utilisateurs dans le domaine ou les domaines approuvés de l’utilisateur.
ms.openlocfilehash: 24c278ebd3acf83e87fbf72650eb3d5d438d5c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465582"
---
# <a name="internalreply"></a>InternalReply

L’élément **InternalReply** contient la réponse d’absence du Bureau envoyée aux autres utilisateurs dans le domaine ou les domaines approuvés de l’utilisateur. 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 **ReplyBody**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|XML : lang  <br/> |Spécifie la langue utilisée dans le message **InternalReply** . Les valeurs possibles de cet attribut sont définies par IETF RFC 3066.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Message (disponibilité)](message-availability.md) <br/> |Contient la réponse OOF.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Spécifie les paramètres OOF.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contient les paramètres OOF.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple de requête SetUserOofSettings suivant définit le [OofState](oofstate.md) sur **activé**, définit la durée de l’absence du Bureau pour 10 jours et définit les messages OOF internes et externes.
  
```XML
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserOofSettings](getuseroofsettings-operation.md)
  
[Opération SetUserOofSettings](setuseroofsettings-operation.md)

