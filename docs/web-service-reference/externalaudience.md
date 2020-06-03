---
title: ExternalAudience
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalAudience
api_type:
- schema
ms.assetid: 79dc2a4c-f7dd-46d1-8f31-149116e1f76e
description: L’élément ExternalAudience définit ou contient une valeur qui détermine à qui les messages externes d’absence du Bureau (OOF) sont envoyés.
ms.openlocfilehash: b3fcebd9042b07bb9a8294196799ef2a13d78bdd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530599"
---
# <a name="externalaudience"></a>ExternalAudience

L’élément **ExternalAudience** définit ou contient une valeur qui détermine à qui les messages externes d’absence du Bureau (OOF) sont envoyés. 
  
```xml
<ExternalAudience>None or Known or All</ExternalAudience>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |Spécifie les paramètres OOF.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |Contient les paramètres OOF.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise pour cet élément. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|**Aucun** <br/> |Les expéditeurs de messages électroniques situés en dehors de l’organisation de l’utilisateur de la boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent pas de réponse externe aux messages OOF.  <br/> |
|**Connus** <br/> |Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront uniquement une réponse externe aux messages OOF si l’expéditeur se trouve dans la liste des contacts de la banque Exchange de l’utilisateur.  <br/> |
|**All** <br/> |Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront une réponse externe aux messages OOF.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément partage le même type que l’élément [AllowExternalOof](allowexternaloof.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple de requête SetUserOofSettings suivant définit le OoFState sur **activé**, définit l’audience externe sur **tous**, définit la durée du OOF sur 10 jours et définit les messages OOF internes et externes.
  
```
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

