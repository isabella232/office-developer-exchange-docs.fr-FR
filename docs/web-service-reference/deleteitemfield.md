---
title: DeleteItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteItemField
api_type:
- schema
ms.assetid: 3893be6a-49a7-49f6-bf53-c7f819ec3f87
description: L’élément DeleteItemField représente une opération de suppression d’une propriété donnée d’un élément au cours d’un appel UpdateItem.
ms.openlocfilehash: 7f29dd4e4c14262d7954fb7422e5bee35112e2e4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540187"
---
# <a name="deleteitemfield"></a>DeleteItemField

**L’élément DeleteItemField représente** une opération de suppression d’une propriété donnée d’un élément au cours d’un appel UpdateItem. 
 
- [UpdateItem](updateitem.md)  
- [ItemChanges](itemchanges.md) 
- [ItemChange](itemchange.md) 
- [Mises à jour (élément)](updates-item.md) 
- [DeleteItemField](deleteitemfield.md)
  
```xml
<DeleteItemField>
   <FieldURI/>
</DeleteItemField>
```

```xml
<DeleteItemField>
   <IndexedFieldURI/> 
</DeleteItemField>
```

```xml
<DeleteItemField>
   <ExtendedFieldURI/>
</DeleteItemField>
```

**DeleteItemFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’une propriété de dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Mises à jour (élément)](updates-item.md) <br/> |Contient un ensemble d’éléments qui définissent l’application, la définition et la suppression des modifications apportées aux propriétés d’élément.  <br/><br/>Voici l’expression XPath de cet élément :<br/>`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |schéma types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [UpdateItem Operation](updateitem-operation.md)

