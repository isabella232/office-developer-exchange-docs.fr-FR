---
title: UpdateItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: L’opération UpdateItem est utilisée pour modifier les propriétés d’un élément existant dans la banque d’informations Exchange.
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838889"
---
# <a name="updateitem-operation"></a>UpdateItem Operation

L’opération **UpdateItem** est utilisée pour modifier les propriétés d’un élément existant dans la banque d’informations Exchange. 
  
## <a name="remarks"></a>Remarques

Vous pouvez effectuer trois actions de mise à jour de base sur un élément. Le tableau suivant répertorie les actions que vous pouvez effectuer.
  
|**Action**|**Description**|
|:-----|:-----|
|Ajout  <br/> |Ajoute des données à une propriété existante. Cette action permet de conserver les données actuelles. Append ne s’applique pas à toutes les propriétés.  <br/> |
|Set  <br/> |Remplace les données d’une propriété si la propriété contient des données, ou crée la propriété et lui affecte la valeur si la propriété n’existe pas. L’action Définir concerne uniquement les propriétés accessibles en écriture.  <br/> |
|Suppression  <br/> |Supprime une propriété d’un élément. Cela diffère de la définition d’une propriété d’une valeur vide. Lorsque cette action est terminée, la propriété n’existe pas pour l’élément. Supprimer n’est pas applicable aux propriétés accessibles en écriture.  <br/> |
   
Un appel **UpdateItem** peut être utilisé pour modifier un ou plusieurs éléments et un ou plusieurs propriétés de chaque élément. L’élément [ItemChanges](itemchanges.md) contient toutes les modifications qui doivent être suivies dans le cadre de cet appel. L’élément [ItemChange](itemchange.md) , un enfant de l’élément [ItemChanges](itemchanges.md) , représente les modifications à effectuer sur un seul élément. L’élément [ItemChange](itemchange.md) contient un ensemble d’actions de mise à jour qui peuvent être effectuées sur un seul élément. Ces modifications sont contenues dans l’élément [mises à jour (élément)](updates-item.md) . L’élément [ItemId](itemid.md) identifie l’élément à mettre à jour. Pour mettre à jour plusieurs propriétés sur un élément, un [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) doit être fourni pour chaque propriété qui nécessite la mise à jour. 
  
> [!NOTE]
> Actions de mise à jour sont appliquées dans l’ordre dans lequel ils sont spécifiés. 
  
Pour chaque modification, vous devez spécifier le chemin d’accès de la propriété à modifier et une représentation de l’élément dont la valeur est nouveau. L’action de suppression est légèrement différente uniquement le chemin d’accès de la propriété qui doit être supprimée est requis. Pour définir et ajouter des actions, le chemin d’accès spécifié doit faire référence à la même propriété est définie dans la représentation de l’élément. Si elles diffèrent, une erreur sera renvoyée.
  
L’opération **UpdateItem** peut définir l’heure de [début](start.md) et [fin](end-ex15websvcsotherref.md) d’un élément de la banque Exchange. Dans une demande **UpdateItem** , l’heure de [début](start.md) peut être défini sans également définir l’heure de [fin](end-ex15websvcsotherref.md) . Cela peut provoquer une erreur si l’heure de [début](start.md) est postérieure à l’heure de [fin](end-ex15websvcsotherref.md) . Sachez que les applications clientes doivent régler l’heure de [fin](end-ex15websvcsotherref.md) lorsque l’heure de [début](start.md) est modifiée afin de conserver la durée. 
  
Lorsqu’un élément de calendrier unique est mis à jour pour devenir un élément de calendrier principal périodique, la propriété [MeetingTimeZone](meetingtimezone.md) doit être définie par l’opération **UpdateItem** pour conserver le fuseau horaire d’origine de l’élément de calendrier. 
  
## <a name="setitemfield-request-example"></a>Exemple de requête SetItemField

### <a name="description"></a>Description

Une demande **UpdateItem** l’exemple suivant montre comment définir la propriété sensitivity sur un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.
  
### <a name="setitemfield-request-elements"></a>Éléments de la demande SetItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ID d’élément](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Exemple de requête AppendToItemField

### <a name="description"></a>Description

Une demande **UpdateItem** l’exemple suivant montre comment ajouter du texte à la propriété body sur un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les propriétés suivantes prennent en charge l’action d’ajout :
  
- **message : ReplyTo**
    
- **Corps de l’élément :**
    
- Les propriétés de collection destinataires et les participants
    
L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.
  
### <a name="appendtoitemfield-request-elements"></a>Éléments de la demande AppendToItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ID d’élément](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Corps](body.md)
    
## <a name="deleteitemfield-request-example"></a>Exemple de requête DeleteItemField

### <a name="description"></a>Description

Une demande **UpdateItem** l’exemple suivant montre comment supprimer une propriété sur un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.
  
### <a name="deleteitemfield-request-elements"></a>Éléments de la demande DeleteItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ID d’élément](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Exemple de réponse réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à une demande de **UpdateItem** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’identificateur d’élément et modifier la clé ont été réduits afin de préserver la lisibilité.
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ID d’élément](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[Opération UpdateItem (tâche)](updateitem-operation-task.md)
  
[Opération UpdateItem (contacts)](updateitem-operation-contact.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Updating Contacts](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Mise à jour de tâches](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

