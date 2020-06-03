---
title: Type (UserConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Type
api_type:
- schema
ms.assetid: d09a9621-6950-451a-90dc-920af9cab35c
description: L’élément type spécifie un type d’objet Dictionary.
ms.openlocfilehash: ea196e070279bb809cc2e4c2a51dd2453dd9b331
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458872"
---
# <a name="type-userconfiguration"></a>Type (UserConfiguration)

L’élément **type** spécifie un type d’objet Dictionary. 
  
```xml
<Type>DateTime or Boolean or Byte or String or Integer32 or UnsignedInteger32 or Integer64 or UnsignedInteger64 or StringArray or ByteArray</Type> 
```

 **UserConfigurationDictionaryObjectTypesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DictionaryKey](dictionarykey.md) <br/> |Spécifie la clé de dictionnaire pour une propriété de dictionnaire.  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |Spécifie la valeur de dictionnaire pour une propriété de dictionnaire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **type** . 
  
**Valeurs des éléments de type**

|**Valeur**|**Description**|
|:-----|:-----|
|DateTime
  <br/> ||
|Boolean  <br/> ||
|Octet  <br/> ||
|Chaîne  <br/> ||
|Integer32  <br/> ||
|UnsignedInteger32  <br/> ||
|Integer64  <br/> ||
|UnsignedInteger64  <br/> ||
|StringArray  <br/> ||
|ByteArray  <br/> ||
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

