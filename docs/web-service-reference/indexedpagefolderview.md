---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: L’élément IndexedPageFolderView décrit comment les informations d’élément pagué sont renvoyées dans une réponse FindFolder.
ms.openlocfilehash: 0a5d0f7e63549b7a851862d957ff32dff4333ce3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542238"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

**L’élément IndexedPageFolderView décrit** comment les informations d’élément pagué sont renvoyées dans une [réponse FindFolder.](findfolder.md) 
  
[FindFolder](findfolder.md)
  
[IndexedPageFolderView](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Décrit le nombre maximal de dossiers à renvoyer dans la réponse. Cet attribut est facultatif.  <br/> |
|**Offset** <br/> |Décrit le décalage par rapport au **point de base.** Le décalage doit être supérieur ou égal à zéro. Si **BasePoint est** égal à Début, le décalage est positif. Si **BasePoint est** égal à End, le décalage est géré comme s’il était négatif.  <br/> Cela permet d’identifier le dossier qui sera le premier dossier remis dans la réponse. Cet attribut est obligatoire.  <br/> |
|**BasePoint** <br/> |Indique si la page de dossiers commence au début ou à la fin de l’ensemble de dossiers qui sont trouvés avec les critères de recherche. La recherche à partir de la fin recherche toujours vers l’arrière. Cet attribut est obligatoire.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut BasePoint

|**Valeur**|**Description**|
|:-----|:-----|
|Début  <br/> |La vue pagyée commence au début du jeu de dossiers trouvé.  <br/> |
|End  <br/> |La vue pagyée commence à la fin de l’ensemble de dossiers trouvés.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande de recherche de dossiers dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

La recherche de bout en bout implique le déplacement vers l’origine identifiée par le décalage. En outre, le pointeur est déplacé vers l’arrière par le nombre d’enregistrements demandés. Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 par rapport à la fin, la recherche commence à 75. Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière de 10 enregistrements supplémentaires à 65 et renvoie les enregistrements 65 à 75. L’index suivant est 64. Le décalage suivant par rapport à la fin d’une page est de 100 moins 64, ce qui correspond à 36. La valeur du décalage suivant entre la fin et la page indexée suivante est 36.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

