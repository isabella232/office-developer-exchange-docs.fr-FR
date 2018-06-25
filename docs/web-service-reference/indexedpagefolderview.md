---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: L’élément IndexedPageFolderView décrit comment paginé informations sont retournées dans une réponse FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827910"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

L’élément **IndexedPageFolderView** décrit comment paginé informations sont retournées dans une réponse [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Indique le nombre maximal de dossiers à renvoyer dans la réponse. Cet attribut est facultatif.  <br/> |
|**Offset** <br/> |Indique le décalage à partir du **point de base**. Offset doit être supérieure ou égale à zéro. Si le **point de base** est égal au début, le décalage est positif. Si le **point de base** est égal à End, le décalage est géré comme s’il s’agissait négatif.  <br/> Identifie le dossier qui sera le premier dossier fourni dans la réponse. Cet attribut est requis.  <br/> |
|**Point de base** <br/> |Indique si la page des dossiers démarre au début ou à la fin de l’ensemble des dossiers se trouvant avec les critères de recherche. Recherche toujours à partir de la fin de recherche vers l’arrière. Cet attribut est requis.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut de point de base

|**Valeur**|**Description**|
|:-----|:-----|
|Début  <br/> |L’affichage paginé commence au début de l’ensemble du dossier trouvé.  <br/> |
|End  <br/> |L’affichage paginé commence à la fin de l’ensemble du dossier trouvé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une requête pour rechercher les dossiers dans une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Recherche à partir de fin consiste à déplacer à l’origine identifié par le décalage. En outre, le pointeur est ramené par le nombre d’enregistrements demandés. Par exemple, si 100 enregistrements et le décalage est de 25 à partir de la fin, la recherche démarre 75. Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière 10 supplémentaires à 65 des enregistrements et retourne les enregistrements de 65 à 75. L’index suivant est de 64. Le prochain offset à partir de la fin d’une page est de 100 moins 64 qui est égale à 36. La valeur de décalage suivant à partir de la fin pour récupérer la page suivante indexée est 36.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

