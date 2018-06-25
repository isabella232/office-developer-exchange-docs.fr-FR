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
description: L’élément FractionalPageFolderView décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête FindFolder.
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756473"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

L’élément **FractionalPageFolderView** décrit où l’affichage paginé démarre et le nombre maximal de dossiers renvoyées dans une requête [FindFolder](findfolder.md) . 
  
[FindFolder](findfolder.md)
  
[FractionalPageFolderView](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifie le nombre maximal de résultats à retourner dans la réponse [FindFolder](findfolder.md) . Cet attribut est facultatif.  <br/> |
|**Numérateur** <br/> |Représente le numérateur du décalage en fraction à partir du début du jeu de résultats. Cet attribut est requis. Le numérateur doit être le dénominateur inférieur ou égal à. Cet attribut doit représenter une valeur intégrale est égale ou supérieure à zéro. Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
|**Dénominateur** <br/> |Représente le dénominateur de décalage fractionnaire à partir du début du nombre total de dossiers dans le jeu de résultats. Cet attribut est requis. Cet attribut doit représenter une valeur intégrale qui est supérieure à 1. Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande pour identifier les dossiers dans une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Le décalage d’affichage paginé à partir du début de l’ensemble des dossiers trouvés est décrit par une fraction. La fraction, qui est définie par les attributs **numérateur** et **dénominateur** , décrit où démarre la page d’informations. Par exemple, si **numérateur** est égale à quatre et **dénominateur** est égal à 5, la page d’informations renvoyées commence une entrée trouve quatre cinquièmes de la manière dans le jeu de résultats. 
  
Si la fraction correspond à zéro, qui indique le début du jeu de résultats. Si la fraction a la valeur 1, qui indique la fin du jeu de résultats.
  
> [!NOTE]
> La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats s’afficheront. 
  
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

