---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: L’élément DictionaryKey spécifie la clé de dictionnaire pour une propriété de dictionnaire.
ms.openlocfilehash: feae35d292c212b41394f63c0840ec4d3c3b8800
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519778"
---
# <a name="dictionarykey"></a>DictionaryKey

**L’élément DictionaryKey** spécifie la clé de dictionnaire pour une propriété de dictionnaire. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (UserConfiguration)](type-userconfiguration.md) <br/> | Spécifie un type d’objet dictionnaire.<br/><br/>Le type peut être l’une des valeurs de chaîne suivantes :<br/><br/>- DateTime  <br/>- Boolean  <br/>- Byte  <br/>- Chaîne  <br/>- Integer32  <br/>- UnsignedInteger32  <br/>- Integer64  <br/>- UnsignedInteger64  <br/>- StringArray  <br/>- ByteArray  <br/> |
|[Value (UserConfiguration)](value-userconfiguration.md) <br/> |Spécifie la valeur de l’objet dictionary en tant que chaîne.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Spécifie le contenu d’une propriété d’entrée de dictionnaire unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

