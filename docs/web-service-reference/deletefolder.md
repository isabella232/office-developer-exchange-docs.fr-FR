---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: L’élément DeleteFolder définit une demande pour supprimer des dossiers à partir d’une boîte aux lettres dans la banque d’informations Exchange.
ms.openlocfilehash: d31f98f26f537104e40b303de4199f45c65f49c7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755862"
---
# <a name="deletefolder"></a>DeleteFolder

L’élément **DeleteFolder** définit une demande pour supprimer des dossiers à partir d’une boîte aux lettres dans la banque d’informations Exchange. 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleType** <br/> |Décrit comment un dossier est supprimé. Cet attribut est requis.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un dossier est définitivement supprimé de la banque.  <br/> |
|SoftDelete  <br/> |Un dossier est déplacé vers la benne si la benne est activé.  <br/> |
|MoveToDeletedItems  <br/> |Un dossier est déplacé vers le dossier éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossier qui sont utilisés pour identifier les dossiers à supprimer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel au service Web est terminée, la base de données a déplacé l’élément vers le dossier éléments supprimés ou définitivement supprimé l’élément de la base de données Exchange. Ce comportement est la même valeur MicrosoftExchange Server 2007 et Exchange Server 2010. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteFolder](deletefolder-operation.md)

