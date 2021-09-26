---
title: DictionaryEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DictionaryEntry
api_type:
- schema
ms.assetid: 531ea96a-d411-43e6-9fec-11fa2c959a30
description: L’élément DictionaryEntry spécifie le contenu d’une propriété d’entrée de dictionnaire unique.
ms.openlocfilehash: 4a9e481f3b9d6fc2d0ef739031042354ed717bee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545320"
---
# <a name="dictionaryentry"></a>DictionaryEntry

**L’élément DictionaryEntry** spécifie le contenu d’une propriété d’entrée de dictionnaire unique. 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 **UserConfigurationDictionaryEntryType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DictionaryKey](dictionarykey.md) <br/> |Spécifie la clé de dictionnaire d’une propriété de dictionnaire.  <br/> |
|[DictionaryValue](dictionaryvalue.md) <br/> |Spécifie la valeur de dictionnaire d’une propriété de dictionnaire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Dictionnaire](dictionary.md) <br/> |Définit un ensemble d’entrées de propriété de dictionnaire pour un objet de configuration utilisateur.  <br/> |
   
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

