---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: L’élément IndexedPageItemView décrit comment la conversation paginée ou les informations d’élément sont renvoyées pour une opération FindItem ou une demande d’opération FindConversation.
ms.openlocfilehash: 0a66f17855fd425082e3651886d3eeec4f217ac4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456912"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

L’élément **IndexedPageItemView** décrit comment la conversation paginée ou les informations d’élément sont renvoyées pour une [opération FindItem](finditem-operation.md) ou une demande d' [opération FindConversation](findconversation-operation.md) . 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Décrit le nombre maximal d’éléments ou de conversations à renvoyer dans la réponse. Cet attribut est facultatif.  <br/> |
|**Offset** <br/> |Décrit le décalage par rapport à l' **BasePoint**. Si **BasePoint** est égal à début, le décalage est positif. Si **BasePoint** est égal à fin, le décalage est géré comme s’il était négatif. Cela identifie l’élément ou la conversation qui sera le premier à être remis dans la réponse. Cet attribut est obligatoire.  <br/> |
|**BasePoint** <br/> |Indique si la page d’éléments ou de conversations commence à partir du début ou de la fin de l’ensemble d’éléments ou de conversations trouvé à l’aide des critères de recherche. La recherche à partir de la fin effectue toujours des recherches vers l’arrière. Cet attribut est obligatoire.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut BasePoint

|**Valeur**|**Description**|
|:-----|:-----|
|Entam  <br/> |L’affichage paginé commence au début de la conversation ou de l’ensemble d’éléments trouvé.  <br/> |
|End  <br/> |L’affichage paginé commence à la fin de la conversation ou de l’ensemble d’éléments trouvé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une requête pour rechercher des conversations dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

La recherche à partir de la fin implique le déplacement vers l’origine identifiée par le décalage. De plus, le pointeur est ramené par le nombre d’enregistrements demandés. Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 à partir de la fin, la recherche commence à partir de 75. Si 10 enregistrements sont renvoyés, le pointeur de la souris recule de 10 enregistrements supplémentaires sur 65 et renvoie les enregistrements 65 à 75. L’index suivant est 64. Le prochain décalage par rapport à la fin d’une page est de 100 moins 64, ce qui équivaut à 36. 36 est la valeur du décalage suivant à partir de la fin pour obtenir la page indexée suivante.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une demande d' [opération FindItem](finditem-operation.md) . Chaque élément est renvoyé avec son ID et son objet. Un maximum de six éléments sont renvoyés dans la réponse, comme spécifié par l’attribut **MaxEntriesReturned** . Les éléments sont répertoriés par ordre croissant groupés par importance. Les éléments d’un groupe sont regroupés par objet. 
  
```XML
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
      <IndexedPageItemView MaxEntriesReturned="6" BasePoint="Beginning" Offset="0" />
      <GroupBy Order="Ascending">
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

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindConversation](findconversation-operation.md)


[Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

