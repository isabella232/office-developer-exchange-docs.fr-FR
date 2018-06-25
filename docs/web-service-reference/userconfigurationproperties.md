---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: L’élément UserConfigurationProperties spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration.
ms.openlocfilehash: 4f993765bb7c36f28a41a3f2fa7e28698a3f709e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838952"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

L’élément **UserConfigurationProperties** spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration. 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Spécifie une requête pour obtenir un objet de configuration utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **UserConfigurationProperties** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|ID  <br/> |Spécifie la propriété identificateur.  <br/> |
|Dictionary  <br/> |Spécifie les types de propriétés de dictionnaire.  <br/> |
|XmlData  <br/> |Spécifie les types de propriété de données XML.  <br/> |
|BinaryData  <br/> |Spécifie les types de propriétés des données binaires.  <br/> |
|Tous  <br/> |Spécifie l’identificateur, dictionnaire, données XML et les types de propriétés des données binaires.  <br/> |
   
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

