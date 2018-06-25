---
title: Nom de configuration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConfigurationName
api_type:
- schema
ms.assetid: 3b524a2f-9c6b-4550-9f3d-f78d176b0f7b
description: L’élément de nom de configuration spécifie les configurations de service requis par un nom.
ms.openlocfilehash: a03a0bc0ab7ecbc1c2aec31f864503ee0f560908
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755535"
---
# <a name="configurationname"></a>Nom de configuration

L’élément de **nom de configuration** spécifie les configurations de service requis par un nom. 
  
```xml
<ConfigurationName>MailTips or UnifiedMessagingConfiguration or ProtectionRules</ConfigurationName>
```

 **ServiceConfigurationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RequestedConfiguration](requestedconfiguration.md) <br/> |Contient les configurations de service demandé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément de **nom de configuration** . 
  
**Valeurs des éléments de nom de configuration**

|**Valeur**|**Description**|
|:-----|:-----|
|Les infos-courrier  <br/> |Identifie la configuration du service Infos-courrier.  <br/> |
|UnifiedMessagingConfiguration  <br/> |Identifie la configuration du service de messagerie unifiée.  <br/> |
|ProtectionRules  <br/> |Identifie la configuration des règles de Protection du service.  <br/> |
   
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

