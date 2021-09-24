---
title: UserConfigurationProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UserConfigurationProperties
api_type:
- schema
ms.assetid: c143a6ec-62ad-4d48-b844-b1ad88054bc1
description: L’élément UserConfigurationProperties spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration.
ms.openlocfilehash: 0aed3ffc680ac881410469fe762349739ba924a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515004"
---
# <a name="userconfigurationproperties"></a>UserConfigurationProperties

**L’élément UserConfigurationProperties** spécifie les types de propriétés à obtenir dans une opération GetUserConfiguration. 
  
```xml
<UserConfigurationProperties>Id | Dictionary | XmlData | BinaryData | All</UserConfigurationProperties>
```

 **UserConfigurationPropertyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserConfiguration](getuserconfiguration.md) <br/> |Spécifie une demande d’obtenir un objet de configuration utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément UserConfigurationProperties.** 
  
|**Valeur**|**Description**|
|:-----|:-----|
|ID  <br/> |Spécifie la propriété d’identificateur.  <br/> |
|Dictionary  <br/> |Spécifie les types de propriétés de dictionnaire.  <br/> |
|XmlData  <br/> |Spécifie les types de propriétés de données XML.  <br/> |
|BinaryData  <br/> |Spécifie les types de propriétés de données binaires.  <br/> |
|Tous  <br/> |Spécifie l’identificateur, le dictionnaire, les données XML et les types de propriétés de données binaires.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

