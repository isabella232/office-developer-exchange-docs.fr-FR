---
title: FolderName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderName
api_type:
- schema
ms.assetid: c5a2cd55-ac47-43bf-94b5-3ab3a4c28a62
description: L’élément FolderName identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres.
ms.openlocfilehash: 76263d56c423411a58ea45d691ce93e2b3202571
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511564"
---
# <a name="foldername"></a>FolderName

**L’élément FolderName** identifie un dossier personnalisé géré unique à ajouter à une boîte aux lettres. 
  
[CreateManagedFolder](createmanagedfolder.md)
  
[FolderNames](foldernames.md)
  
[FolderName](foldername.md)
  
```xml
<FolderName>...</FolderName>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FolderNames](foldernames.md) <br/> |Contient un tableau de dossiers personnalisés gérés nommés à ajouter à une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/CreateManagedFolder/FolderNames` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. La valeur de texte représente un nom de dossier.
  
## <a name="remarks"></a>Remarques

Bien que vous pouvez utiliser Exchange Web Services pour ajouter des dossiers personnalisés gérés à une boîte aux lettres, vous ne pouvez pas utiliser la même technologie pour accéder à la liste des dossiers personnalisés gérés disponibles. Vous pouvez obtenir une liste de dossiers personnalisés gérés à l’aide d’une commande Exchange Management Shell ou à l’aide d’une API qui s’interface avec le service d’annuaire Active Directory. Le nom du dossier est le nom de l’objet Active Directory correspondant.
  
Vous pouvez utiliser [l’opération FindFolder](findfolder-operation.md) pour rechercher des dossiers personnalisés gérés. Utilisez [l’opération DeleteFolder pour](deletefolder-operation.md) supprimer des dossiers personnalisés gérés. 
  
Il est important de noter que **FolderName** est le nom d’un dossier personnalisé géré existant dans l’organisation. Une tentative d’ajout d’un dossier qui ne se trouve pas dans l’organisation entraîne une réponse d’erreur. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[Ajout de dossiers gérés](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

