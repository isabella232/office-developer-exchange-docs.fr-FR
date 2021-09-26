---
title: DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: e37963f4-af9e-4481-b389-16175711e66d
description: L’élément DeleteFolder définit une demande de suppression de dossiers d’une boîte aux lettres dans la Exchange store.
ms.openlocfilehash: d1d64b84604acec54d9153144e5bfd7abaece94c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542476"
---
# <a name="deletefolder"></a>DeleteFolder

**L’élément DeleteFolder** définit une demande de suppression de dossiers d’une boîte aux lettres dans Exchange store. 
  
```XML
<DeleteFolder DeleteType="">
   <FolderIds/>
</DeleteFolder>
```

 **DeleteFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**DeleteType** <br/> |Décrit comment un dossier est supprimé. Cet attribut est obligatoire.  <br/> |
   
#### <a name="deletetype-attribute"></a>Attribut DeleteType

|**Valeur**|**Description**|
|:-----|:-----|
|HardDelete  <br/> |Un dossier est définitivement supprimé de la boutique.  <br/> |
|SoftDelete  <br/> |Un dossier est déplacé vers la benne si la benne est activée.  <br/> |
|MoveToDeletedItems  <br/> |Un dossier est déplacé vers le dossier Éléments supprimés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à supprimer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les options **MoveToDeletedItems** et **HardDelete** sont transactionnelles, ce qui signifie qu’au moment où un appel de service Web se termine, la base de données a déplacé l’élément vers le dossier Éléments supprimés ou supprimé définitivement de la base de données Exchange. Ce comportement est le même pour MicrosoftExchange Server 2007 et Exchange Server 2010. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteFolder](deletefolder-operation.md)

