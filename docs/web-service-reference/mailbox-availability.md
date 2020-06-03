---
title: Boîte aux lettres (disponibilité)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: L’élément Mailbox représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.
ms.openlocfilehash: 1bda6e8b90551b86b4e1c2711ac25693a65e5410
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458074"
---
# <a name="mailbox-availability"></a>Boîte aux lettres (disponibilité)

L’élément **Mailbox** représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddress)](name-emailaddress.md) <br/> |Représente le nom complet de l’utilisateur de boîte aux lettres. Cet élément est facultatif dans le SetUserOofSettingsRequest. L’GetUserOofSettingsRequest renverra cet élément.  <br/> |
|[Address (chaîne)](address-string.md) <br/> |Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres. Cet élément est obligatoire.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Représente le protocole de routage du message. Cet élément est facultatif dans le SetUserOofSettingsRequest. L’GetUserOofSettingsRequest renverra cet élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Utilisé pour obtenir les paramètres et les messages d’absence du Bureau d’un utilisateur de boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Permet de définir les paramètres et les messages OOF d’un utilisateur de boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Remarques

L’adresse de messagerie est utilisée pour identifier le dossier de calendrier qui contient les paramètres OOF. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md)
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

