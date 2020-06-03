---
title: FolderNames
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
description: L’élément FolderNames contient un tableau de dossiers gérés nommés à ajouter à une boîte aux lettres.
ms.openlocfilehash: 00cb1a81f420469033ccbc745313d2719b155aff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530985"
---
# <a name="foldernames"></a>FolderNames

L’élément **foldernames** contient un tableau de dossiers gérés nommés à ajouter à une boîte aux lettres. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
```xml
<FolderNames>
   <FolderName/>
</FolderNames>
```

 **NonEmptyArrayOfFolderNamesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderName](foldername.md) <br/> |Identifie un dossier géré unique à ajouter à la boîte aux lettres.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CreateManagedFolder](createmanagedfolder.md) <br/> |Élément racine dans une demande d’ajout d’un dossier géré à une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CreateManagedFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

