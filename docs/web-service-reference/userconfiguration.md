---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: L’élément UserConfiguration définit un objet de configuration utilisateur unique.
ms.openlocfilehash: 1217f5d591570c2d8df49a116b6bf35c243d1e0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468907"
---
# <a name="userconfiguration"></a>UserConfiguration

L’élément **UserConfiguration** définit un objet de configuration utilisateur unique. 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 **UserConfigurationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Cet élément doit être utilisé lors de la création d’un objet de configuration utilisateur.  <br/> |
|[ItemId](itemid.md) <br/> |Définit l’identificateur d’élément d’objet de configuration utilisateur.  <br/> |
|[Dictionnaire](dictionary.md) <br/> |Définit un ensemble d’entrées de propriété de dictionnaire pour un objet de configuration utilisateur.  <br/> |
|[XmlData](xmldata.md) <br/> |Contient le contenu de propriété de données XML pour un objet de configuration utilisateur.  <br/> |
|[BinaryData](binarydata.md) <br/> |Contient le contenu de propriété de données binaires pour un objet de configuration utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Représente une demande de création d’un objet de configuration utilisateur.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Représente une réponse qui retourne un objet de configuration utilisateur.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Représente une demande de mise à jour d’un objet de configuration utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

