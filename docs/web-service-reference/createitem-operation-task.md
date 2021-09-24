---
title: Opération CreateItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: L’opération CreateItem crée des éléments de tâche dans Exchange store.
ms.openlocfilehash: 814a32e82cd5c1c95be252d1b53387741898dd40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510255"
---
# <a name="createitem-operation-task"></a>Opération CreateItem (tâche)

L’opération CreateItem crée des éléments de tâche dans Exchange store.
  
## <a name="task-createitem-request"></a>Demande CreateItem de tâche

### <a name="description"></a>Description

L’exemple suivant d’une demande CreateItem montre comment créer un élément de tâche dans une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                MessageDisposition="SaveOnly">
      <Items>
        <t:Task>
          <t:Subject>My task</t:Subject>
          <t:DueDate>2006-10-26T21:32:52</t:DueDate>
          <t:Status>NotStarted</t:Status>
        </t:Task>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les demandes de tâches périodiques sont modifiées lorsqu’elles sont reçues par l’ordinateur exécutant Microsoft Exchange Server 2007 sur le rôle serveur d’accès au client. Les modifications suivantes se produisent :
  
- Seule la date est enregistrée pour la [propriété StartDate (Recurrence)](startdate-recurrence.md) de la plage de récurrences de la tâche. La partie temps est tronquée. 
    
- La [propriété StartDate (Recurrence)](startdate-recurrence.md) peut être ajustée en fonction de la récurrence. Par exemple, si la récurrence est spécifiée comme tous les lundis et que la date de début est définie sur le 26 octobre 2006, c’est-à-dire le jeudi, la date de début est ajustée au 30 octobre 2006, qui est le lundi suivant. 
    
- Si la [propriété StartDate](startdate.md) de la tâche est définie, elle est mise à jour pour correspondre à la [valeur StartDate (Recurrence)](startdate-recurrence.md) de la plage de récurrence. La [propriété DueDate](duedate.md) de la tâche est également mise à jour en fonction de la [nouvelle startDate](startdate.md).
    
- Si la [propriété StartDate](startdate.md) n’est pas définie, seule la propriété [DueDate](duedate.md) est mise à jour pour correspondre à [la valeur StartDate (Recurrence)](startdate-recurrence.md) de la plage de récurrences. 
    
Le tableau suivant indique les modifications apportées par le serveur d’accès au client à une tâche périodique dont la tâche Task.Recurrence.Pattern a lieu tous les lundis.
  
**Modifications apportées à une tâche périodique**

|**Propriété**|**Valeur d’origine**|**Valeur mise à jour**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1er janvier 2006  <br/> |30 octobre 2006  <br/> |
|Task.DueDate  <br/> |3 janvier 2006  <br/> |1er novembre 2006  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 octobre 2006  <br/> |30 octobre 2006  <br/> |
   
Par défaut, si un dossier de destination n’est pas spécifié, les éléments de tâche sont créés dans le dossier Tâches.
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [CreateItem](createitem.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tâche](task.md)
    
- [Sujet](subject.md)
    
- [DueDate](duedate.md)
    
- [État](status.md)
    
## <a name="successful-task-createitem-response"></a>Réponse CreateItem de tâche réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande CreateItem.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Task>
              <t:ItemId Id="AAAtAE=" ChangeKey="EwAAABYA"/>
            </t:Task>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont inclus dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tâche](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[Opération CreateItem](createitem-operation.md)


[Création de tâches](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Mise à jour des tâches](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Suppression de tâches](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

