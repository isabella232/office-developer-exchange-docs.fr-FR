---
title: EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 502b2841-103d-4340-97d5-51a1db813fb2
description: L’élément EmptyFolder définit une demande de vider un dossier dans une boîte aux lettres dans Exchange magasin. Si vous le souhaitez, les sous-dossiers peuvent également être supprimés lorsque le dossier est vidé.
ms.openlocfilehash: c1b0e953f677c1fe5ae0958b35f85f3f5c4fb973
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519673"
---
# <a name="emptyfolder"></a>EmptyFolder

**L’élément EmptyFolder** définit une demande de vider un dossier dans une boîte aux lettres dans Exchange magasin. Si vous le souhaitez, les sous-dossiers peuvent également être supprimés lorsque le dossier est vidé. 
  
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
|**DeleteType** <br/> |Spécifie la façon dont un dossier est vidé. Cet attribut est obligatoire.  <br/> |
|**DeleteSubFolders** <br/> |Spécifie si les sous-fichiers doivent être supprimés. Cet attribut est obligatoire.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleteType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un message et des dossiers sont définitivement supprimés de la boutique.  <br/> |
|SoftDelete  <br/> |Un message et des dossiers sont déplacés vers la benne si la benne est activée.  <br/> |
|MoveToDeletedItems  <br/> |Un message et des dossiers sont déplacés vers le dossier Éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à supprimer.  <br/> |
   
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
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération EmptyFolder](emptyfolder-operation.md)

