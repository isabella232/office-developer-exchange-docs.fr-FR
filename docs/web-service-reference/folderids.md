---
title: FolderIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderIds
api_type:
- schema
ms.assetid: 3ff9d15a-7220-4785-ae6b-583a7eb82005
description: L’élément FolderIds contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements.
ms.openlocfilehash: 911a74ca778ee988c270c16c67620a40656d82d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756449"
---
# <a name="folderids"></a>FolderIds

L’élément **FolderIds** contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers pour copier, déplacer, obtenir, supprimer ou contrôler les notifications d’événements. 
  
```xml
<FolderIds>
   <FolderId/>
   <DistinguishedFolderId/>
</FolderIds>
```

 **NonEmptyArrayOfBaseFolderIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Identifie les dossiers Microsoft Exchange Server qui peuvent être référencés par un nom.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetFolder](getfolder.md) <br/> |Définit une demande pour obtenir un dossier à partir de la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/GetFolder` <br/> |
|[DeleteFolder](deletefolder.md) <br/> |Définit une demande pour supprimer des dossiers de la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/DeleteFolder` <br/> |
|[EmptyFolder](emptyfolder.md) <br/> |Définit une demande pour supprimer des dossiers de la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/EmptyFolder` <br/> |
|[MoveFolder](movefolder.md) <br/> |Définit une demande de déplacement d’un dossier dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Définit une demande pour copier un dossier dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :`/CopyFolder` <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification push d’événements.  <br/> |
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Représente un abonnement à un abonnement de notification d’événement de type pull.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages et http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma des messages ; Schéma de types  <br/> |
|Fichier de validation  <br/> |Messages.xsd ; Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetFolder](getfolder-operation.md)
  
[Opération DeleteFolder](deletefolder-operation.md)
  
[Opération MoveFolder](movefolder-operation.md)
  
[Opération CopyFolder](copyfolder-operation.md)
  
[Opération d'abonnement](subscribe-operation.md)

