---
title: Type (UserConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Type
api_type:
- schema
ms.assetid: d09a9621-6950-451a-90dc-920af9cab35c
description: L’élément Type spécifie un type d’objet dictionnaire.
ms.openlocfilehash: f0bafa9023a42fdf8464891e8df7931a0766b416
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538729"
---
# <a name="type-userconfiguration"></a>Type (UserConfiguration)

**L’élément Type** spécifie un type d’objet dictionnaire. 
  
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
|[DictionaryKey](dictionarykey.md) <br/> |Spécifie la clé de dictionnaire d’une propriété de dictionnaire.  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |Spécifie la valeur de dictionnaire d’une propriété de dictionnaire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément Type.** 
  
**Valeurs des éléments de type**

|**Valeur**|**Description**|
|:-----|:-----|
|Date/heure  <br/> ||
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

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

