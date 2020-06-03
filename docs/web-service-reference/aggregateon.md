---
title: AggregateOn
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: L’élément AggregateOn représente la propriété utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé.
ms.openlocfilehash: 04359c187ef11538d64f8f0d3ea2fe84bc3d048b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463565"
---
# <a name="aggregateon"></a>AggregateOn

L’élément **AggregateOn** représente la propriété utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé. 
  
- [FindItem](finditem.md)  
- [GroupBy](groupby.md)
- [AggregateOn](aggregateon.md)
  
```xml
<AggregateOn>
   <FieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <IndexedFieldURI/>
</AggregateOn>
```

```xml
<AggregateOn>
   <ExtendedFieldURI/>
</AggregateOn>
```
 
**AggregateOnType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**Aggregate** <br/> | Indique la valeur maximale ou minimale de la propriété identifiée par l’élément [FieldURI](fielduri.md) utilisé pour classer les groupes d’éléments.<br/><br/>Les valeurs possibles sont les suivantes :  <br/><br/>-Minimum  <br/>-Maximum  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés référencées fréquemment par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues à obtenir, définir ou créer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupBy](groupby.md) <br/> |Spécifie des groupes arbitraires pour les requêtes FindItem.  <br/> Voici l’expression XPath de cet élément :`/FindItem/GroupBy` <br/> |
   
## <a name="remarks"></a>Remarques

L' [opération FindItem](finditem-operation.md) peut renvoyer des résultats groupés. Dans les résultats groupés, tous les éléments qui ont la même valeur pour une propriété de regroupement donnée sont rassemblés et présentés en tant qu’enfants de ce groupe. Par exemple, si vous regroupez par l’expéditeur, tous les messages électroniques sont organisés en groupes distincts selon qu’ils proviennent de l’expéditeur A, de l’expéditeur B, et ainsi de suite. Ces groupes sont les enfants du groupe expéditeur. 
  
Chacun des groupes au sein du groupe d’expéditeurs contient une collection d’éléments, tels que les messages électroniques réels provenant de chaque expéditeur. Vous pouvez utiliser l’élément [SortOrder](sortorder.md) pour trier les éléments au sein d’un groupe. Toutefois, pour trier les groupes en fonction des valeurs de propriété d’un élément, vous devez utiliser l’agrégation. 
  
Avec l’agrégation, l’ordre des groupes est basé sur une propriété spécifique des éléments au sein du groupe. Lorsque vous utilisez l’agrégation pour trier des éléments au sein d’un groupe, vous devez identifier une propriété représentative permettant de trier les groupes. Vous pouvez utiliser l’élément **AggregateOn** pour spécifier la propriété Representative. 
  
Lorsqu’une propriété représentative est identifiée, l’attribut **Aggregate** est utilisé pour indiquer si les groupes sont triés en fonction de la valeur maximale ou minimale de la propriété identifiée. Si l’attribut **Aggregate** est défini sur maximum, les groupes sont triés en commençant par la plus grande valeur pour la propriété **AggregateOn** . Si l’attribut **Aggregate** a la valeur minimum, les groupes sont triés en commençant par la plus petite valeur pour la propriété **AggregateOn** . 
  
Par exemple, si vous souhaitez émettre une requête groupée FindItem, un regroupement par expéditeur, mais vous souhaitez ordonner les groupes afin que le groupe dont le message électronique est le plus récent se trouve en premier, vous pouvez regrouper par expéditeur et agréger sur date/heure de réception avec un attribut d' **agrégat** de maximum. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une requête FindItem groupée et une réponse. L’exemple illustre une demande de renvoi d’éléments groupés par la propriété **ConversationTopic** . Deux groupes, A et B, sont renvoyés dans l’ordre décroissant en fonction de la valeur maximale de la propriété [DateTimeReceived](datetimereceived.md) . 
  
```XML
<!-- EXAMPLE REQUEST -->
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="message:ConversationTopic"/>
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AdditionalProperties>    
      </ItemShape>
      <IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="20" Offset="0"/>
      <GroupBy Order="Ascending">
        <t:FieldURI FieldURI="message:ConversationTopic"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:DateTimeReceived"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
<!-- EXAMPLE RESPONSE -->
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>B</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAH=" ChangeKey="CQAAABY" />
                    <t:DateTimeReceived>2006-09-14T23:59:18Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnAHR=" ChangeKey="CQAAAw" />
                    <t:DateTimeReceived>2006-09-15T00:00:24Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQAnA==" ChangeKey="CQAAJXT" />
                    <t:DateTimeReceived>2006-09-15T00:22:45Z</t:DateTimeReceived>
                    <t:ConversationTopic>B</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>A</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AQAnAAA==" ChangeKey="CQCJNe" />
                    <t:DateTimeReceived>2006-09-14T23:56:12Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AQWgAA==" ChangeKey="CQAACJV6" />
                    <t:DateTimeReceived>2006-09-14T23:57:33Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAAA==" ChangeKey="CQA6CJXw" />
                    <t:DateTimeReceived>2006-09-15T00:23:31Z</t:DateTimeReceived>
                    <t:ConversationTopic>A</t:ConversationTopic>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Pour trier les éléments d’un groupe, utilisez l’élément [OrdreTri](sortorder.md) . 
  
> [!NOTE]
> Les identificateurs d’élément et les clés de modification ont été raccourcies afin de préserver la lisibilité. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération FindItem](finditem-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

