---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: L’élément FolderIds contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événements.
ms.openlocfilehash: 7c0cf46d5fdaf35ec72cf3b5750b51edc5a8bfe0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518364"
---
# <a name="folderids"></a>FolderIds

**L’élément FolderIds** contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à copier, déplacer, obtenir, supprimer ou surveiller les notifications d’événements. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie Microsoft Exchange Server dossiers qui peuvent être référencés par leur nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Définit une demande d’obtenir un dossier à partir de la Exchange store.  <br/> Voici l’expression XPath de cet élément :  `/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Définit une demande de suppression de dossiers de la Exchange store.  <br/> Voici l’expression XPath de cet élément :  `/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Définit une demande de suppression de dossiers de la Exchange store.  <br/> Voici l’expression XPath de cet élément :  `/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Définit une demande de déplacement d’un dossier dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Définit une demande de copie d’un dossier dans la Exchange store.  <br/> Voici l’expression XPath de cet élément :  `/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événements push.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement basé sur un pull.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages et https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma des messages ; Schéma types  <br/> |
|Fichier de validation  <br/> |Messages.xsd; Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetFolder](getfolder-operation.md)
  
[Opération DeleteFolder](deletefolder-operation.md)
  
[Opération MoveFolder](movefolder-operation.md)
  
[Opération CopyFolder](copyfolder-operation.md)
  
[Opération d'abonnement](subscribe-operation.md)

