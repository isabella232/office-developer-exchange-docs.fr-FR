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
description: L’élément IndexedPageItemView décrit comment paginée conversation ou élément les informations sont retournées pour une opération FindItem ou une requête d’opération FindConversation.
ms.openlocfilehash: f1743e22087158c1889977f03774fccbc5577390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827919"
---
# <a name="indexedpageitemview"></a>IndexedPageItemView

L’élément **IndexedPageItemView** décrit comment paginée conversation ou élément les informations sont retournées pour une demande [d’opération FindItem](finditem-operation.md) ou [FindConversation](findconversation-operation.md) . 
  
```XML
<IndexedPageViewItemView MaxEntriesReturned="" Offset="" BasePoint=""/>
```

 **IndexedPageViewType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Indique le nombre maximal d’éléments ou des conversations à renvoyer dans la réponse. Cet attribut est facultatif.  <br/> |
|**Offset** <br/> |Indique le décalage à partir du **point de base**. Si le **point de base** est égal au début, le décalage est positif. Si le **point de base** est égal à End, le décalage est géré comme s’il s’agissait négatif. Il identifie l’élément ou conversation sera le premier à être remis dans la réponse. Cet attribut est requis.  <br/> |
|**Point de base** <br/> |Indique si la page des éléments ou des conversations redémarre depuis le début ou la fin de l’ensemble des éléments ou des conversations qui sont trouvent à l’aide de critères de recherche. Recherche toujours à partir de la fin de recherche vers l’arrière. Cet attribut est requis.  <br/> |
   
#### <a name="basepoint-attribute"></a>Attribut de point de base

|**Valeur**|**Description**|
|:-----|:-----|
|Début  <br/> |L’affichage paginé commence au début de l’ensemble de conversation ou d’un élément trouvé.  <br/> |
|End  <br/> |L’affichage paginé commence à la fin de l’ensemble de conversation ou d’un élément trouvé.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher des éléments dans une boîte aux lettres.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindItem` <br/> |
|[FindConversation](findconversation.md) <br/> |Définit une requête pour rechercher les conversations dans une boîte aux lettres.  <br/> |
   
## <a name="remarks"></a>Remarques

Recherche à partir de la fin consiste à déplacer à l’origine identifié par le décalage. En outre, le pointeur est ramené par le nombre d’enregistrements demandés. Par exemple, si 100 enregistrements et le décalage est de 25 à partir de la fin, la recherche démarre 75. Si 10 enregistrements sont renvoyés, le pointeur est déplacé vers l’arrière 10 supplémentaires à 65 des enregistrements et retourne les enregistrements de 65 à 75. L’index suivant est de 64. Le prochain offset à partir de la fin d’une page est de 100 moins 64 qui est égale à 36. 36 est la valeur de décalage suivant à partir de la fin pour récupérer la page suivante indexée.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une demande [d’opération FindItem](finditem-operation.md) . Chaque élément est renvoyée avec son ID et son objet. Un maximum de six articles sont retournés dans la réponse, comme spécifié par l’attribut **MaxEntriesReturned** . Les éléments sont répertoriés dans l’ordre regroupé par importance croissant. Éléments d’un groupe sont regroupées par sujet. 
  
```XML
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[FindConversation Operation](findconversation-operation.md)


[Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

