---
title: ChildFolderCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ChildFolderCount
api_type:
- schema
ms.assetid: e0e4eabd-802f-4dd0-9911-89e08c66a15e
description: L’élément ChildFolderCount représente le nombre de dossiers enfants immédiats contenus dans un dossier. Cette propriété est en lecture seule.
ms.openlocfilehash: c05d93e3f9df2d2acbb1b65f1116dab1aea24a3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537000"
---
# <a name="childfoldercount"></a>ChildFolderCount

**L’élément ChildFolderCount** représente le nombre de dossiers enfants immédiats contenus dans un dossier. Cette propriété est en lecture seule. 
  
```xml
<ChildFolderCount/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier Calendrier dans une boîte aux lettres.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier Contacts dans une boîte aux lettres.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Représente un dossier Tâches dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente un integer. Cette propriété est en lecture seule.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

