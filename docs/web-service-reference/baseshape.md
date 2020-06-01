---
title: BaseShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BaseShape
api_type:
- schema
ms.assetid: 42c04f3b-abaa-4197-a3d6-d21677ffb1c0
description: L’élément BaseShape identifie le jeu de propriétés à renvoyer dans une réponse d’élément ou de dossier.
ms.openlocfilehash: 9b3f00ff94fbfe6ad6373b16ad95eb9136f81c64
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464489"
---
# <a name="baseshape"></a>BaseShape

L’élément **BaseShape** identifie le jeu de propriétés à renvoyer dans une réponse d’élément ou de dossier. 
  
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
|[FolderShape](foldershape.md) <br/> | Identifie les propriétés de dossier à inclure dans la réponse GetFolder, FindFolder ou Opérationsyncfolderhierarchy.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés d’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.<br/><br/>Voici les expressions XPath de cet élément :<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Le tableau suivant répertorie les valeurs de texte possibles.
  
**Valeurs de texte pour l’élément BaseShape**

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |Renvoie uniquement l’ID d’élément ou de dossier.  <br/> |
|Par défaut  <br/> |Renvoie un ensemble de propriétés qui sont définies comme valeur par défaut pour l’élément ou le dossier.  <br/> |
|AllProperties  <br/> |Renvoie toutes les propriétés utilisées par la couche de logique métier Exchange pour créer un dossier.  <br/> |
   
Le tableau suivant répertorie les propriétés par défaut qui sont renvoyées pour une demande FindFolder. Tous les sous-dossiers d’un dossier donné sont renvoyés par nom.
  
**Propriétés par défaut**

|**Folder**|**Propriétés par défaut**|
|:-----|:-----|
|Boîte de réception  <br/> |FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers  <br/> |
|Contacts  <br/> |FolderId, nom complet, nombre total, nombre de sous-dossiers  <br/> |
|Calendrier  <br/> |FolderId, nom d’affichage, nombre de sous-dossiers  <br/> |
|Brouillons  <br/> |FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers  <br/> |
|Éléments supprimés  <br/> |FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers  <br/> |
|Autres dossiers  <br/> |FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers  <br/> |
|Boîte d'envoi  <br/> |FolderId, nom d’affichage, nombre de messages non lus, nombre total, nombre de sous-dossiers  <br/> |
|Tâches  <br/> |FolderId, nom complet, nombre de retard, nombre total, nombre de sous-dossiers  <br/> |
|Notes  <br/> |FolderId, nom complet, nombre total, nombre de sous-dossiers  <br/> |
   
## <a name="remarks"></a>Remarques

Pour renvoyer des propriétés en plus de celles identifiées par l’élément [BaseShape](baseshape.md) , utilisez l’élément [AdditionalProperties](additionalproperties.md) . 
  
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

