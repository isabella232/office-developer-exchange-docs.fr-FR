---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: L’élément FractionalPageItemView décrit l’endroit où démarre la vue pagiée et le nombre maximal d’éléments renvoyés dans une demande FindItem.
ms.openlocfilehash: 0d948bad0ba24c4a105be32daa645d1864cb4f3b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530245"
---
# <a name="fractionalpageitemview"></a>FractionalPageItemView

**L’élément FractionalPageItemView** décrit l’endroit où démarre la vue pagiée et le nombre maximal d’éléments renvoyés dans une [demande FindItem.](finditem.md) 
  
[FindItem](finditem.md)
  
[FractionalPageItemView](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 **FractionalPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Identifie le nombre maximal de résultats à renvoyer dans la [réponse FindItem.](finditem.md) Cet attribut est facultatif. Si cet attribut n’est pas spécifié, l’appel retourne tous les éléments disponibles.  <br/> |
|**Numerator** <br/> |Représente le numérateur du décalage fractionnel par rapport au début du jeu de résultats. Cet attribut est obligatoire. Le numérateur doit être égal ou inférieur au dénominateur. Cet attribut doit représenter une valeur intégrale égale ou supérieure à zéro.  <br/> Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
|**Denominator** <br/> |Représente le dénominateur du décalage fractionnaire par rapport au début du nombre total d’éléments dans le jeu de résultats. Cet attribut est obligatoire. Cet attribut doit représenter une valeur intégrale supérieure à une.  <br/> Pour plus d’informations, voir les remarques plus loin dans cette rubrique.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Remarques

Le décalage de l’affichage pagacé par rapport au début de l’ensemble d’éléments trouvés est décrit par une fraction. La fraction, qui est définie par les attributs **Numerator** et **Denominator,** décrit l’endroit où commence la page d’informations. Par exemple, si **Numerator** est égal à quatre et **Quenominator** est égal à cinq, la page d’informations renvoyées commence à une entrée située quatre-cinquièmes du chemin d’accès au jeu de résultats. 
  
Si la fraction est évaluée à zéro, cela indique le début du jeu de résultats. Si la fraction est évaluée à un, cela indique la fin du jeu de résultats.
  
> [!NOTE]
> La fraction représente le point de départ de la page, et non le nombre de résultats renvoyés dans le jeu de résultats. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant illustre [une demande FindItem.](finditem.md) La requête renvoie les éléments des résultats de recherche qui commencent après le deuxième tiers de tous les éléments du jeu de résultats. 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Par exemple, si le jeu de résultats contient neuf éléments, l’affichage pagayé retourne jusqu’à 12 éléments, en commençant à l’élément trouvé à deux tiers du chemin d’accès au jeu de résultats. Dans ce cas, la page commence au septième élément. La page contient les septième, huitième et neuvième éléments. Si le numérateur est définie sur zéro, l’affichage de page retourne tous les éléments du jeu de résultats tant que le nombre est inférieur à l’attribut **MaxEntriesReturned.** 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)


[Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

