---
title: RelativeFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54e3ba52-08a6-4d48-8a44-6fd5fdbffb25
description: L’élément RelativeFolderPath contient un tableau de dossiers qui indiquent le chemin d’accès au dossier relatif du chemin d’accès au dossier à créer.
ms.openlocfilehash: 8a0fc0020943afdbe6cd4c79d51d61337f8dd329
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457157"
---
# <a name="relativefolderpath"></a>RelativeFolderPath

L’élément **RelativeFolderPath** contient un tableau de dossiers qui indiquent le chemin d’accès au dossier relatif du chemin d’accès au dossier à créer. 
  
```XML
<RelativeFolderPath>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</RelativeFolderPath>
```

 **NonEmptyArrayOfFoldersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Folder (dossier](folder.md)  |  ) [CalendarFolder](calendarfolder.md)  |  [ContactsFolder](contactsfolder.md)  |  [SearchFolder](searchfolder.md)  |  [TasksFolder](tasksfolder.md)
  
### <a name="parent-elements"></a>Éléments parents

[CreateFolderPath](createfolderpath.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

