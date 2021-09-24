---
title: Mailbox (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Mailbox
api_type:
- schema
ms.assetid: affd192e-8914-473f-9098-d9bdf898de2c
description: L’élément Mailbox représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.
ms.openlocfilehash: 5e32c4be807dae92b27df7012caa8eb1b295b26c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522921"
---
# <a name="mailbox-availability"></a>Mailbox (Availability)

**L’élément Mailbox** représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings. 
  
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
|[Name (EmailAddress)](name-emailaddress.md) <br/> |Représente le nom complet de l’utilisateur de la boîte aux lettres. Cet élément est facultatif dans setUserOofSettingsRequest. GetUserOofSettingsRequest retourne cet élément.  <br/> |
|[Address (String)](address-string.md) <br/> |Représente l’adresse de messagerie de l’utilisateur de la boîte aux lettres. Cet élément est obligatoire.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Représente le protocole de routage pour le message. Cet élément est facultatif dans setUserOofSettingsRequest. GetUserOofSettingsRequest retourne cet élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Permet d’obtenir les paramètres et les messages d’absence Office d’un utilisateur de boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Permet de définir les paramètres et les messages d’absence du travail d’un utilisateur de boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Remarques

L’adresse de messagerie est utilisée pour identifier le dossier de calendrier qui contient les paramètres d’absence du travail. 
  
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

