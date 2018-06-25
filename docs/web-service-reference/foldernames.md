---
title: Noms de dossier
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderNames
api_type:
- schema
ms.assetid: 6cbe4083-5705-4695-a54e-8dab3e472662
description: L’élément de noms de dossier contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres.
ms.openlocfilehash: 819b3c2df1cfcae3a5d4a48539e369a00b1f7229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756452"
---
# <a name="foldernames"></a>Noms de dossier

L’élément de **noms de dossier** contient un tableau des dossiers gérés nommées à ajouter à une boîte aux lettres. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[Noms de dossier](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 **NonEmptyArrayOfFolderNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderName](foldername.md) <br/> |Identifie un dossier géré unique à ajouter à la boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateManagedFolder](createmanagedfolder.md) <br/> |L’élément racine dans une demande pour ajouter un dossier géré à une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

