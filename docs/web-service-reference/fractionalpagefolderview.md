---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: L’élément FractionalPageFolderView décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463068"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

L’élément **FractionalPageFolderView** décrit l’emplacement où l’affichage paginé démarre et le nombre maximal de dossiers renvoyés dans une demande [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifie le nombre maximal de résultats à renvoyer dans la réponse [FindFolder](findfolder.md) . Cet attribut est facultatif.  <br/> |
|**Monnaie** <br/> |Représente le numérateur du décalage fractionnaire à partir du début du jeu de résultats. Cet attribut est obligatoire. Le numérateur doit être inférieur ou égal au dénominateur. Cet attribut doit représenter une valeur intégrale égale ou supérieure à zéro. Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.  <br/> |
|**Petit** <br/> |Représente le dénominateur du décalage fractionnaire à partir du début du nombre total de dossiers dans le jeu de résultats. Cet attribut est obligatoire. Cet attribut doit représenter une valeur intégrale supérieure à 1. Pour plus d’informations, consultez la section Remarques plus loin dans cette rubrique.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande pour identifier les dossiers d’une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Le décalage de l’affichage paginé à partir du début de l’ensemble des dossiers trouvés est décrit par une fraction. La fraction, définie par les attributs **numérateur** et **dénominateur** , décrit l’emplacement de début de la page d’informations. Par exemple, si le **numérateur** est égal à quatre et que le **dénominateur** est égal à cinq, la page des informations retournées commence à une entrée située quatre cinquièmes du contenu du jeu de résultats. 
  
Si la fraction est égale à zéro, cela indique le début du jeu de résultats. Si la fraction est égale à 1, cela indique la fin du jeu de résultats.
  
> [!NOTE]
> La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats. 
  
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

