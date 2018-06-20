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
description: L’élément de boîte aux lettres représente l’utilisateur de boîte aux lettres pour un SetUserOofSettings ou GetUserOofSettings demande.
ms.openlocfilehash: 2e901ae0df56542f56f247184254294735018468
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828254"
---
# <a name="mailbox-availability"></a>Boîte aux lettres (disponibilité)

L’élément de **boîte aux lettres** représente l’utilisateur de boîte aux lettres pour un SetUserOofSettings ou GetUserOofSettings demande. 
  
```xml
<Mailbox>
   <Name>...</Name>
   <Address>...</Address>
   <RoutingType>...</RoutingType>
</Mailbox>
```

**EmailAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddress)](name-emailaddress.md) <br/> |Représente le nom complet de l’utilisateur de boîte aux lettres. Cet élément est facultatif dans le SetUserOofSettingsRequest. Le GetUserOofSettingsRequest retournera cet élément.  <br/> |
|[Adresse (chaîne)](address-string.md) <br/> |Représente l’adresse de messagerie de l’utilisateur de boîte aux lettres. Cet élément est obligatoire.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Représente le protocole de routage pour le message. Cet élément est facultatif dans le SetUserOofSettingsRequest. Le GetUserOofSettingsRequest retournera cet élément.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsRequest](getuseroofsettingsrequest.md) <br/> |Permet d’obtenir les paramètres d’absence du bureau (OOF) et les messages d’un utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserOofSettingsRequest` <br/> |
|[SetUserOofSettingsRequest](setuseroofsettingsrequest.md) <br/> |Permet de définir les paramètres d’absence du bureau et des messages d’un utilisateur de boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/SetUserOofSettingsRequest` <br/> |
   
## <a name="remarks"></a>Remarques

L’adresse de messagerie est utilisée pour identifier le dossier calendrier qui contient les paramètres d’absence du bureau. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md)
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

