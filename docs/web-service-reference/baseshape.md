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
description: L’élément BaseShape identifie le jeu de propriétés à retourner dans une réponse de l’élément ou le dossier.
ms.openlocfilehash: 69b27d23fd75d4c1a274f31dfa419b759dbb2bbe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755381"
---
# <a name="baseshape"></a>BaseShape

L’élément **BaseShape** identifie le jeu de propriétés à retourner dans une réponse de l’élément ou le dossier. 
  
```xml
<BaseShape>IdOnly or Default or AllProperties</BaseShape>
```

 **DefaultShapeNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> | Identifie les propriétés du dossier à inclure dans la réponse GetFolder, FindFolder ou SyncFolderHierarchy.<br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/GetFolder/FolderShape` <br/>  `/FindFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[ItemShape](itemshape.md) <br/> | Identifie les propriétés de l’élément et le contenu à inclure dans une réponse GetItem, FindItem ou SyncFolderItems.<br/><br/>Les expressions XPath pour cet élément sont les suivantes :<br/><br/>`/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Le tableau suivant répertorie les valeurs possibles de texte.
  
**Valeurs de texte pour l’élément BaseShape**

|**Valeur**|**Description**|
|:-----|:-----|
|IdOnly  <br/> |Renvoie uniquement l’élément ou le dossier ID de.  <br/> |
|Default (Défaut)  <br/> |Renvoie un ensemble de propriétés qui sont définies par défaut pour l’élément ou d’un dossier.  <br/> |
|AllProperties  <br/> |Retourne toutes les propriétés utilisées par la couche de la logique du système Exchange pour créer un dossier.  <br/> |
   
Le tableau suivant répertorie les propriétés par défaut qui sont retournées pour une demande FindFolder. Tous les sous-dossiers d’un dossier donné sont retournés dans l’ordre par nom.
  
**Propriétés par défaut**

|**Folder**|**Propriétés par défaut**|
|:-----|:-----|
|Inbox  <br/> |FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers  <br/> |
|Contacts  <br/> |FolderId, nom complet, le nombre total, count sous-dossier  <br/> |
|Calendrier  <br/> |FolderId, nom d’affichage, le nombre de sous-dossiers  <br/> |
|Brouillons  <br/> |FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers  <br/> |
|Éléments supprimés  <br/> |FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers  <br/> |
|Autres dossiers  <br/> |FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers  <br/> |
|La boîte d’envoi  <br/> |FolderId, nom d’affichage, lus, nombre total, le nombre de sous-dossiers  <br/> |
|Tâches  <br/> |FolderId, nom d’affichage, en retard count, nombre total, le nombre de sous-dossiers  <br/> |
|Remarques  <br/> |FolderId, nom complet, le nombre total, count sous-dossier  <br/> |
   
## <a name="remarks"></a>Remarques

Pour renvoyer les propriétés en plus de celles identifié par l’élément [BaseShape](baseshape.md) , utilisez l’élément [AdditionalProperties](additionalproperties.md) . 
  
## <a name="example"></a>Exemple

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [FolderShape](foldershape.md)
- [ItemShape](itemshape.md)

