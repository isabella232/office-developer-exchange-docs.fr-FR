---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: L’élément DictionaryKey spécifie la clé de dictionnaire pour une propriété de dictionnaire.
ms.openlocfilehash: 7e706f16fe155278ea56f303ffbb5971c1779879
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755923"
---
# <a name="dictionarykey"></a>DictionaryKey

L’élément **DictionaryKey** spécifie la clé de dictionnaire pour une propriété de dictionnaire. 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 **UserConfigurationDictionaryObjectType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Type (UserConfiguration)](type-userconfiguration.md) <br/> | Spécifie un type d’objet dictionary.<br/><br/>Le type peut être une des valeurs de chaîne suivantes :<br/><br/>-DateTime  <br/>-Booléen  <br/>-Octets  <br/>-String  <br/>-Integer32  <br/>-UnsignedInteger32  <br/>-Integer64  <br/>-UnsignedInteger64  <br/>-StringArray  <br/>-ByteArray  <br/> |
|[Valeur (UserConfiguration)](value-userconfiguration.md) <br/> |Spécifie la valeur d’objet dictionnaire sous forme de chaîne.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DictionaryEntry](dictionaryentry.md) <br/> |Spécifie le contenu d’une propriété de l’entrée de dictionnaire unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

