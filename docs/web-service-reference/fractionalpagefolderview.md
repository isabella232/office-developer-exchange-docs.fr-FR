---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: L’élément FractionalPageFolderView décrit le début de l’affichage pagacé et le nombre maximal de dossiers renvoyés dans une demande FindFolder.
ms.openlocfilehash: b3d4bd63f94c2db7761dabfad1e32558ceb30be5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530252"
---
# <a name="fractionalpagefolderview"></a>FractionalPageFolderView

**L’élément FractionalPageFolderView** décrit le début de l’affichage pagacé et le nombre maximal de dossiers renvoyés dans une [demande FindFolder.](findfolder.md) 
  
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
|**MaxEntriesReturned** <br/> |Identifie le nombre maximal de résultats à renvoyer dans la [réponse FindFolder.](findfolder.md) Cet attribut est facultatif.  <br/> |
|**Numerator** <br/> |Représente le numérateur du décalage fractionnel par rapport au début du jeu de résultats. Cet attribut est obligatoire. Le numérateur doit être égal ou inférieur au dénominateur. Cet attribut doit représenter une valeur intégrale égale ou supérieure à zéro. Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
|**Denominator** <br/> |Représente le dénominateur du décalage fractionnaire par rapport au début du nombre total de dossiers dans le jeu de résultats. Cet attribut est obligatoire. Cet attribut doit représenter une valeur intégrale supérieure à une. Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolder](findfolder.md) <br/> |Définit une demande d’identification des dossiers dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a>Remarques

Le décalage de l’affichage pagacé par rapport au début de l’ensemble de dossiers trouvés est décrit par une fraction. La fraction, qui est définie par les attributs **Numerator** et **Denominator,** décrit l’endroit où commence la page d’informations. Par exemple, si **Numerator** est égal à quatre et **Quenominator** est égal à cinq, la page d’informations renvoyées commence à une entrée située quatre-cinquièmes du chemin d’accès au jeu de résultats. 
  
Si la fraction est évaluée à zéro, cela indique le début du jeu de résultats. Si la fraction est évaluée à un, cela indique la fin du jeu de résultats.
  
> [!NOTE]
> La fraction représente le point de départ de la page, et non le nombre de résultats renvoyés dans le jeu de résultats. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

