---
title: IndexedPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IndexedPageItemView
api_type:
- schema
ms.assetid: 6d1b0b04-cc35-4a57-bd7a-824136d14fda
description: L’élément IndexedPageItemView décrit comment les informations de conversation pagiée ou d’élément sont renvoyées pour une opération FindItem ou une demande d’opération FindConversation.
ms.openlocfilehash: bf46bdbd457c4f4fa47e6b575d3b797b74f58995
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541125"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

**L’élément IndexedPageItemView** décrit comment les informations de conversation pagiée ou d’élément sont renvoyées pour une opération [FindItem](finditem-operation.md) ou [une demande d’opération FindConversation.](findconversation-operation.md) 
  
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
|**Offset** <br/> |Décrit le décalage par rapport au **point de base.** Si **BasePoint est** égal à Début, le décalage est positif. Si **BasePoint est** égal à End, le décalage est géré comme s’il était négatif. Cela permet d’identifier l’élément ou la conversation qui sera le premier à être remis dans la réponse. Cet attribut est obligatoire.  <br/> |
|**BasePoint** <br/> |Indique si la page d’éléments ou de conversations commence au début ou à la fin de l’ensemble d’éléments ou de conversations trouvés à l’aide des critères de recherche. La recherche à partir de la fin recherche toujours vers l’arrière. Cet attribut est obligatoire.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut BasePoint

|**Valeur**|**Description**|
|:-----|:-----|
|Début  <br/> |La vue pagyée commence au début de la conversation ou du jeu d’éléments trouvé.  <br/> |
|End  <br/> |La vue pagyée commence à la fin de la conversation ou du jeu d’éléments trouvé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une demande de recherche d’éléments dans une boîte aux lettres.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une demande de recherche de conversations dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

La recherche de la fin implique le déplacement vers l’origine identifiée par le décalage. En outre, le pointeur est déplacé vers l’arrière par le nombre d’enregistrements demandés. Par exemple, s’il y a 100 enregistrements et que le décalage est de 25 par rapport à la fin, la recherche commence à 75. Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière de 10 enregistrements supplémentaires à 65 et renvoie les enregistrements 65 à 75. L’index suivant est 64. Le décalage suivant par rapport à la fin d’une page est de 100 moins 64, ce qui correspond à 36. 36 est la valeur du décalage suivant par rapport à la fin pour obtenir la page indexée suivante.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant illustre une [demande d’opération FindItem.](finditem-operation.md) Chaque élément est renvoyé avec son ID et son objet. Un maximum de six éléments sont renvoyés dans la réponse, comme spécifié par l’attribut **MaxEntriesReturned.** Les éléments sont répertoriés par ordre croissant, regroupés par importance. Les éléments d’un groupe sont agrégés par objet. 
  
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
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[Opération FindConversation](findconversation-operation.md)


[Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

