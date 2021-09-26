---
title: AggregateOn
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AggregateOn
api_type:
- schema
ms.assetid: 9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb
description: L’élément AggregateOn représente la propriété utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé.
ms.openlocfilehash: 4fa46837cc794bc6c4b23a6b5627d95509d60d70
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541552"
---
# <a name="aggregateon"></a>AggregateOn

**L’élément AggregateOn** représente la propriété utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé. 
  
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
|**Aggregate** <br/> | Indique la valeur maximale ou minimale de la propriété identifiée par l’élément [FieldURI](fielduri.md) utilisé pour l’ordre des groupes d’éléments.<br/><br/>Les valeurs possibles sont les suivantes :  <br/><br/>- Minimum  <br/>- Maximum  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Identifie les propriétés fréquemment référencés par URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Identifie les membres individuels d’un dictionnaire.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie les propriétés MAPI étendues à obtenir, définir ou créer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GroupBy](groupby.md) <br/> |Spécifie les regroupements arbitraires pour les requêtes FindItem.  <br/> Voici l’expression XPath de cet élément :  `/FindItem/GroupBy` <br/> |
   
## <a name="remarks"></a>Remarques

[L’opération FindItem peut](finditem-operation.md) renvoyer des résultats groupés. Dans les résultats groupés, tous les éléments qui ont la même valeur pour une propriété de regroupement donnée sont regroupés et présentés en tant qu’enfants de ce groupe. Par exemple, si vous groupez par expéditeur, tous les messages électroniques sont organisés en groupes distincts selon qu’ils sont issus de l’expéditeur A, de l’expéditeur B, etc. Ces groupes sont des enfants du groupe d’expéditeurs. 
  
Chacun des groupes au sein du groupe d’expéditeurs contient une collection d’éléments, tels que les messages électroniques réels provenant de chaque expéditeur. Vous pouvez utiliser [l’élément SortOrder](sortorder.md) pour trier les éléments d’un groupe. Toutefois, pour trier les groupes en fonction des valeurs de propriété d’un élément, vous devez utiliser l’agrégation. 
  
Avec l’agrégation, l’ordre des groupes est basé sur une propriété spécifique des éléments au sein du groupe. Lorsque vous utilisez l’agrégation pour trier des éléments au sein d’un groupe, vous devez identifier une propriété représentative par laquelle trier les groupes. Vous pouvez utiliser **l’élément AggregateOn** pour spécifier la propriété représentative. 
  
Lorsqu’une propriété représentative est identifiée, l’attribut **Aggregate** est utilisé pour indiquer si les groupes sont triés en fonction de la valeur maximale ou minimale de la propriété identifiée. Si **l’attribut Aggregate** est définie sur Maximum, les groupes sont triés en commençant par la plus grande valeur de la **propriété AggregateOn.** Si **l’attribut Aggregate** est définie sur Minimum, les groupes sont triés en commençant par la plus petite valeur de la **propriété AggregateOn.** 
  
Par exemple, si vous souhaitez émettre une requête groupée FindItem, regroupée par expéditeur, mais que vous souhaitez commander les groupes de sorte que le groupe avec le message électronique le plus récent soit en haut, vous pouvez regrouper par expéditeur et agréger la date/l’heure reçue avec l’attribut **Aggregate** de Maximum. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="example"></a>Exemple

L’exemple suivant montre une requête et une réponse FindItem groupées. L’exemple montre une demande de retour d’éléments regroupés par la **propriété ConversationTopic.** Deux groupes, A et B, sont renvoyés dans l’ordre décroit en fonction de la valeur maximale de la [propriété DateTimeReceived.](datetimereceived.md) 
  
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

Pour trier les éléments d’un groupe, utilisez [l’élément SortOrder.](sortorder.md) 
  
> [!NOTE]
> Les identificateurs d’élément et les touches de modification ont été raccourcis pour préserver la lisibilité. 
  
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

