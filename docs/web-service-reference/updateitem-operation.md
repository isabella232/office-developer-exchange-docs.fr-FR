---
title: Opération UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: L’opération UpdateItem est utilisée pour modifier les propriétés d’un élément existant dans la Exchange store.
ms.openlocfilehash: 6ac09c24c13efff8053fc605ec2c0e6cf2957429
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514059"
---
# <a name="updateitem-operation"></a>Opération UpdateItem

**L’opération UpdateItem** est utilisée pour modifier les propriétés d’un élément existant dans la Exchange store. 
  
## <a name="remarks"></a>Remarques

Vous pouvez effectuer trois actions de mise à jour de base sur un élément. Le tableau suivant répertorie les actions que vous pouvez effectuer.
  
|**Action**|**Description**|
|:-----|:-----|
|Ajout  <br/> |Ajoute des données à une propriété existante. Cette action conserve les données actuelles. Append ne s’applique pas à toutes les propriétés.  <br/> |
|Set  <br/> |Remplace les données d’une propriété si la propriété contient des données, ou crée la propriété et définit sa valeur si la propriété n’existe pas. L’action de jeu s’applique uniquement aux propriétés accessibles en writable.  <br/> |
|Supprimer  <br/> |Supprime une propriété d’un élément. Cela diffère de la définition d’une propriété sur une valeur vide. Lorsque cette action est terminée, la propriété n’existe pas pour l’élément. La suppression s’applique uniquement aux propriétés accessibles en writable.  <br/> |
   
Un **appel UpdateItem** peut être utilisé pour modifier un ou plusieurs éléments et une ou plusieurs propriétés sur chaque élément. [L’élément ItemChanges](itemchanges.md) contient toutes les modifications qui doivent être effectuées dans le cadre de cet appel. [L’élément ItemChange,](itemchange.md) un enfant de l’élément [ItemChanges,](itemchanges.md) représente les modifications à effectuer sur un seul élément. [L’élément ItemChange](itemchange.md) contient un ensemble d’actions de mise à jour qui peuvent être effectuées sur un seul élément. Ces modifications sont contenues dans [l’élément Updates (Item).](updates-item.md) [L’élément ItemId](itemid.md) identifie l’élément à mettre à jour. Pour mettre à jour plusieurs propriétés sur un élément, un [élément SetItemField,](setitemfield.md) [AppendToItemField](appendtoitemfield.md)ou [DeleteItemField](deleteitemfield.md) doit être fourni pour chaque propriété nécessitant la mise à jour. 
  
> [!NOTE]
> Les actions de mise à jour sont appliquées dans l’ordre dans lequel elles sont spécifiées. 
  
Pour chaque modification, vous devez spécifier le chemin d’accès de la propriété à modifier et une représentation de cet élément avec sa nouvelle valeur. L’action de suppression est légèrement différente dans la mesure où seul le chemin d’accès de la propriété à supprimer est requis. Pour les actions définies et d’application, le chemin d’accès spécifié doit faire référence à la propriété définie dans la représentation d’élément. Si elles diffèrent, une erreur est renvoyée.
  
**L’opération UpdateItem peut** [](end-ex15websvcsotherref.md) définir l’heure [de](start.md) début et de fin d’un élément Exchange magasin. Dans une **demande UpdateItem,** l’heure [de](start.md) début peut être définie sans définir l’heure [de](end-ex15websvcsotherref.md) fin. Cela peut provoquer une erreur si l’heure [de](start.md) début est ultérieure à [l’heure de ](end-ex15websvcsotherref.md) fin. N’ignorez pas que les applications [](start.md) clientes doivent ajuster l’heure [de](end-ex15websvcsotherref.md) fin lorsque l’heure de début est modifiée afin de conserver la durée. 
  
Lorsqu’un élément de calendrier unique est mis à jour pour devenir un élément de calendrier principal périodique, la propriété [MeetingTimeZone](meetingtimezone.md) doit être définie par l’opération **UpdateItem** afin de conserver le fuseau horaire d’origine de l’élément de calendrier. 
  
## <a name="setitemfield-request-example"></a>Exemple de requête SetItemField

### <a name="description"></a>Description

L’exemple suivant **d’une requête UpdateItem** montre comment définir la propriété de sensibilité sur un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

L’identificateur d’élément et la touche de modification ont été raccourcis pour préserver la lisibilité.
  
### <a name="setitemfield-request-elements"></a>Éléments de requête SetItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Sensitivity](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a>Exemple de requête AppendToItemField

### <a name="description"></a>Description

L’exemple suivant **d’une requête UpdateItem** montre comment appender du texte à la propriété body d’un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Les propriétés suivantes prendre en charge l’action d’application :
  
- **message:ReplyTo**
    
- **item:Body**
    
- Toutes les propriétés de la collection de destinataires et de participants
    
L’identificateur d’élément et la touche de modification ont été raccourcis pour préserver la lisibilité.
  
### <a name="appendtoitemfield-request-elements"></a>Éléments de requête AppendToItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [AppendToItemField](appendtoitemfield.md)
    
- [FieldURI](fielduri.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Corps](body.md)
    
## <a name="deleteitemfield-request-example"></a>Exemple de requête DeleteItemField

### <a name="description"></a>Description

L’exemple suivant **d’une demande UpdateItem** montre comment supprimer une propriété sur un élément. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

L’identificateur d’élément et la touche de modification ont été raccourcis pour préserver la lisibilité.
  
### <a name="deleteitemfield-request-elements"></a>Éléments de requête DeleteItemField

Les éléments suivants sont utilisés dans la demande :
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [ItemId](itemid.md)
    
- [Mises à jour (élément)](updates-item.md)
    
- [DeleteItemField](deleteitemfield.md)
    
- [FieldURI](fielduri.md)
    
## <a name="successful-response-example"></a>Exemple de réponse réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à une **demande UpdateItem.** 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

L’identificateur d’élément et la touche de modification ont été raccourcis pour préserver la lisibilité.
  
### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[Opération UpdateItem (tâche)](updateitem-operation-task.md)
  
[Opération UpdateItem (Contact)](updateitem-operation-contact.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Updating Contacts](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[Mise à jour des tâches](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

