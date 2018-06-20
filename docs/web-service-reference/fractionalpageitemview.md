---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: L’élément FractionalPageItemView décrit où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête FindItem.
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756476"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

L’élément **FractionalPageItemView** décrit où l’affichage paginé démarre et le nombre maximal d’éléments renvoyés dans une requête [FindItem](finditem.md) . 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifie le nombre maximal de résultats à retourner dans la réponse [FindItem](finditem.md) . Cet attribut est facultatif. Si cet attribut n’est pas spécifié, l’appel retournera tous les éléments disponibles.  <br/> |
|**Numérateur** <br/> |Représente le numérateur du décalage en fraction à partir du début du jeu de résultats. Cet attribut est requis. Le numérateur doit être le dénominateur inférieur ou égal à. Cet attribut doit représenter une valeur intégrale est égale ou supérieure à zéro.  <br/> Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
|**Dénominateur** <br/> |Représente le dénominateur de décalage fractionnaire à partir du début du nombre total d’éléments dans le jeu de résultats. Cet attribut est requis. Cet attribut doit représenter une valeur intégrale qui est supérieure à 1.  <br/> Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le décalage d’affichage paginé à partir du début du jeu d’éléments trouvés est décrit par une fraction. La fraction, qui est définie par les attributs **numérateur** et **dénominateur** , décrit où démarre la page d’informations. Par exemple, si **numérateur** est égale à quatre et **dénominateur** est égal à 5, la page d’informations renvoyées commence une entrée trouve quatre cinquièmes de la manière dans le jeu de résultats. 
  
Si la fraction correspond à zéro, qui indique le début du jeu de résultats. Si la fraction a la valeur 1, qui indique la fin du jeu de résultats.
  
> [!NOTE]
> La fraction représente le point de départ de la page, pas le nombre de résultats dans le jeu de résultats s’afficheront. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une demande [FindItem](finditem.md) . La requête renvoie les éléments dans les résultats de recherche qui démarre après le second troisième de tous les éléments dans le jeu de résultats. 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

Par exemple, si le jeu de résultats contient des neuf éléments, l’affichage paginé renverra jusqu'à 12 éléments, en commençant au niveau de l’élément trouvé deux tiers de la manière dans le jeu de résultats. Dans ce cas, la page commence à l’élément septième. La page contiendra le septième, huitième et neuvième éléments. Si le numérateur est égale à zéro, l’affichage de la page retournera tous les éléments du résultat dans la mesure où le nombre est inférieur à l’attribut **MaxEntriesReturned** . 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)


[Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

