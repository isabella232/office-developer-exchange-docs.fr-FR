---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: L’élément EmptyFolder définit une demande pour vider un dossier dans une boîte aux lettres dans la banque d’informations Exchange. Si vous le souhaitez, sous-dossiers peuvent également être supprimés lorsque le dossier est vidé.
ms.openlocfilehash: c72e11cea29e2e55c9c29754eec60e73bd1e4d9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756153"
---
# <a name="emptyfolder"></a>EmptyFolder

L’élément **EmptyFolder** définit une demande pour vider un dossier dans une boîte aux lettres dans la banque d’informations Exchange. Si vous le souhaitez, sous-dossiers peuvent également être supprimés lorsque le dossier est vidé. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleType** <br/> |Spécifie comment un dossier est vidé. Cet attribut est requis.  <br/> |
|**DeleteSubFolders** <br/> |Spécifie si les sous-dossiers doivent être supprimés. Cet attribut est requis.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |A les messages et les dossiers sont définitivement supprimés de la banque.  <br/> |
|SoftDelete  <br/> |A les messages et les dossiers sont déplacés vers la benne si la benne est activé.  <br/> |
|MoveToDeletedItems  <br/> |A les messages et les dossiers sont déplacés vers le dossier éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération EmptyFolder](emptyfolder-operation.md)

