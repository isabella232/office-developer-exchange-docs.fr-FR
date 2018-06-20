---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique lors d’une opération FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829253"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

L’élément **RootFolder** contient les résultats d’une recherche d’un dossier racine unique lors d’une [opération FindFolder](findfolder-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |Représente l’index suivant doit être utilisé pour la requête suivante lors de l’utilisation d’une vue indexée de pagination.  <br/> |
|NumeratorOffset  <br/> |Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lors de l’utilisation des affichages de page en fraction.  <br/> |
|AbsoluteDenominator  <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination en fraction.  <br/> |
|IncludesLastItemInRange  <br/> |Indique si les résultats actuels de contient le dernier dossier dans la requête, telles que davantage de pagination n’est pas nécessaire.  <br/> |
|TotalItemsInView  <br/> |Représente le nombre total de dossiers qui transmet la restriction.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau des dossiers qui que se trouve à l’aide de l' [opération FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande [d’opération FindFolder](findfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
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

