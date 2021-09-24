---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: L’élément BaseShape identifie l’ensemble des propriétés à renvoyer dans une réponse d’élément ou de dossier.
ms.openlocfilehash: b4e7f5c6d6520e7338f274b6275e371366b1bed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514857"
---
# <a name="baseshape"></a>BaseShape

**L’élément BaseShape** identifie l’ensemble des propriétés à renvoyer dans une réponse d’élément ou de dossier. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifie les propriétés de dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.<br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés et le contenu de l’élément à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.<br/><br/>Les expressions XPath de cet élément sont les suivantes :<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs de texte possibles.
  
**Valeurs de texte pour l’élément BaseShape**

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |Renvoie uniquement l’ID de l’élément ou du dossier.  <br/> |
|Par défaut  <br/> |Renvoie un ensemble de propriétés qui sont définies comme valeur par défaut pour l’élément ou le dossier.  <br/> |
|AllProperties  <br/> |Renvoie toutes les propriétés utilisées par la couche Exchange Logique métier pour construire un dossier.  <br/> |
   
Le tableau suivant répertorie les propriétés par défaut renvoyées pour une demande FindFolder. Tous les sous-dossiers d’un dossier donné sont renvoyés dans l’ordre par nom.
  
**Propriétés par défaut**

|**Folder**|**Propriétés par défaut**|
|:-----|:-----|
|Boîte de réception  <br/> |FolderId, nom d’affichage, nombre non lu, nombre total, nombre de sous-dossiers  <br/> |
|Contacts  <br/> |FolderId, nom complet, nombre total, nombre de sous-dossiers  <br/> |
|Calendrier  <br/> |FolderId, nom d’affichage, nombre de sous-dossiers  <br/> |
|Brouillons  <br/> |FolderId, nom d’affichage, nombre non lu, nombre total, nombre de sous-dossiers  <br/> |
|Éléments supprimés  <br/> |FolderId, nom d’affichage, nombre non lu, nombre total, nombre de sous-dossiers  <br/> |
|Autres dossiers  <br/> |FolderId, nom d’affichage, nombre non lu, nombre total, nombre de sous-dossiers  <br/> |
|Boîte d’envoi  <br/> |FolderId, nom d’affichage, nombre non lu, nombre total, nombre de sous-dossiers  <br/> |
|Tâches  <br/> |FolderId, nom complet, nombre d’échéances passées, nombre total, nombre de sous-dossiers  <br/> |
|Remarques  <br/> |FolderId, nom complet, nombre total, nombre de sous-dossiers  <br/> |
   
## <a name="remarks"></a>Remarques

Pour renvoyer des propriétés en plus de celles identifiées par [l’élément BaseShape,](baseshape.md) utilisez [l’élément AdditionalProperties.](additionalproperties.md) 
  
## <a name="example"></a>Exemple

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

