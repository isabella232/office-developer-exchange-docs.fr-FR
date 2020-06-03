---
title: DeleteFolderField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderField
api_type:
- schema
ms.assetid: f9c2187b-4c60-4358-b4b4-ede50eadae48
description: L’élément DeleteFolderField représente une opération permettant de supprimer une propriété donnée d’un dossier lors d’un appel UpdateFolder.
ms.openlocfilehash: a0b48b667c8c8afbd5729d5deb84359a6a6ccc25
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462156"
---
# <a name="deletefolderfield"></a>DeleteFolderField

L’élément **DeleteFolderField** représente une opération permettant de supprimer une propriété donnée d’un dossier lors d’un appel UpdateFolder. 
  
- [UpdateFolder](updatefolder.md) 
- [FolderChanges](folderchanges.md)  
- [FolderChange](folderchange.md)  
- [Mises à jour (dossier)](updates-folder.md) 
- [DeleteFolderField](deletefolderfield.md)
  
```xml
<DeleteFolderField>
   <FieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <ExtendedFieldURI/>
</DeleteFolderField>
```

```xml
<DeleteFolderField>
   <IndexedFieldURI/>
</DeleteFolderField>
```

**DeleteFolderFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés référencées fréquemment par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’une propriété de dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Mises à jour (dossier)](updates-folder.md) <br/> |Contient un ensemble d’éléments qui définissent les modifications apportées par l’ajout, la définition et la suppression aux propriétés du dossier.  <br/> Voici l’expression XPath de cet élément :`/UpdateFolder/FolderChanges/FolderChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération UpdateFolder](updatefolder-operation.md)

