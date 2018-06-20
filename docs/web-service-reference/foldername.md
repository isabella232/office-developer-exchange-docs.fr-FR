---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: L’élément FolderName identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres.
ms.openlocfilehash: 56a7a7d256624c5103c88a333222807519d21501
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756455"
---
# <a name="foldername"></a>FolderName

L’élément **FolderName** identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[Noms de dossier](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Noms de dossier](foldernames.md) <br/> |Contient un tableau de nommé dossiers personnalisés gérés à ajouter à une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte représente un nom de dossier.
  
## <a name="remarks"></a>Remarques

Bien que vous pouvez utiliser les Services Web Exchange pour ajouter des dossiers personnalisés gérés à une boîte aux lettres, vous ne pouvez pas utiliser la même technologie pour accéder à la liste des dossiers personnalisés gérés disponibles. Vous pouvez obtenir une liste des dossiers personnalisés gérés à l’aide d’une commande Exchange Management Shell ou à l’aide d’une API qui interagit avec le service d’annuaire Active Directory. Le nom du dossier est le nom de l’objet Active Directory correspondant.
  
Vous pouvez utiliser l' [opération FindFolder](findfolder-operation.md) pour rechercher des dossiers personnalisés gérés. Utilisez l' [opération DeleteFolder](deletefolder-operation.md) pour supprimer des dossiers personnalisés gérés. 
  
Il est important de noter que **nom_dossier** est le nom d’un dossier personnalisé géré existant dans l’organisation. Tentative d’ajout d’un dossier qui n’est pas dans l’organisation entraînera une réponse d’erreur. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

