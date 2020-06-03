---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: L’élément EmptyFolder définit une demande de vidage d’un dossier dans une boîte aux lettres dans la Banque d’Exchange. Vous pouvez également supprimer des sous-dossiers lorsque le dossier est vidé.
ms.openlocfilehash: a42e4e3f25741a96ee65fe6f87fc3236b68f4dc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457276"
---
# <a name="emptyfolder"></a>EmptyFolder

L’élément **EmptyFolder** définit une demande de vidage d’un dossier dans une boîte aux lettres dans la Banque d’Exchange. Vous pouvez également supprimer des sous-dossiers lorsque le dossier est vidé. 
  
```XML
<EmptyFolder>
   <FolderIds/>
</EmptyFolder>
```

 **EmptyFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleteType** <br/> |Spécifie le mode de vidage d’un dossier. Cet attribut est obligatoire.  <br/> |
|**DeleteSubFolders** <br/> |Indique si les sous-dossiers doivent être supprimés. Cet attribut est obligatoire.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleteType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Les messages et les dossiers sont définitivement supprimés de la Banque.  <br/> |
|SoftDelete  <br/> |Les messages et les dossiers sont déplacés vers la benne si la benne est activée.  <br/> |
|MoveToDeletedItems  <br/> |Les messages et les dossiers sont déplacés vers le dossier éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau des identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma de message  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération EmptyFolder](emptyfolder-operation.md)

