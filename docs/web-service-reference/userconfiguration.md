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
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838949"
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[UserConfigurationName](userconfigurationname.md) <br/> |Représente le nom d’un objet de configuration utilisateur. Cet élément doit être utilisé lorsque vous créez un objet de configuration utilisateur.  <br/> |
|[ID d’élément](itemid.md) <br/> |Définit l’identificateur d’élément objet configuration utilisateur.  <br/> |
|[Dictionnaire](dictionary.md) <br/> |Définit un ensemble d’entrées de dictionnaire de propriétés pour un objet de configuration utilisateur.  <br/> |
|[XmlData](xmldata.md) <br/> |Contient le contenu de propriété de données XML pour un objet de configuration utilisateur.  <br/> |
|[BinaryData](binarydata.md) <br/> |Contient des données binaires propriété pour un objet de configuration utilisateur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateUserConfiguration](createuserconfiguration.md) <br/> |Représente une demande pour créer un objet de configuration utilisateur.  <br/> |
|[GetUserConfigurationResponseMessage](getuserconfigurationresponsemessage.md) <br/> |Représente une réponse qui renvoie un objet de configuration utilisateur.  <br/> |
|[UpdateUserConfiguration](updateuserconfiguration.md) <br/> |Représente une demande pour mettre à jour un objet de configuration utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

