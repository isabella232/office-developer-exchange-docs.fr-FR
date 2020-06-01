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
description: L’élément IndexedPageFolderView décrit comment les informations d’élément paginé sont renvoyées dans une réponse FindFolder.
ms.openlocfilehash: 6e9e2796c0bdcd9a15487f0e1bc7cbdf09d0a492
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457199"
---
# <a name="indexedpagefolderview"></a>IndexedPageFolderView

L’élément **IndexedPageFolderView** décrit comment les informations d’élément paginé sont renvoyées dans une réponse [FindFolder](findfolder.md) . 
  
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
|**Offset** <br/> |Décrit le décalage par rapport à l' **BasePoint**. Offset doit être supérieur ou égal à zéro. Si **BasePoint** est égal à début, le décalage est positif. Si **BasePoint** est égal à fin, le décalage est géré comme s’il était négatif.  <br/> Cela identifie le dossier qui sera le premier dossier remis dans la réponse. Cet attribut est obligatoire.  <br/> |
|**BasePoint** <br/> |Indique si la page de dossiers commence à partir du début ou de la fin de l’ensemble des dossiers trouvés avec les critères de recherche. La recherche à partir de la fin effectue toujours des recherches vers l’arrière. Cet attribut est obligatoire.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut BasePoint

|**Valeur**|**Description**|
|:-----|:-----|
|Entam  <br/> |L’affichage paginé commence au début de l’ensemble de dossiers trouvé.  <br/> |
|End  <br/> |La vue paginée commence à la fin de l’ensemble de dossiers trouvé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande de recherche de dossiers dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

La recherche de end implique le passage à l’origine identifiée par le décalage. De plus, le pointeur est ramené par le nombre d’enregistrements demandés. Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 à partir de la fin, la recherche commence à partir de 75. Si 10 enregistrements sont renvoyés, le pointeur de la souris recule de 10 enregistrements supplémentaires sur 65 et renvoie les enregistrements 65 à 75. L’index suivant est 64. Le prochain décalage par rapport à la fin d’une page est de 100 moins 64, ce qui équivaut à 36. La valeur du décalage suivant à partir de la fin pour obtenir la page indexée suivante est 36.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   

