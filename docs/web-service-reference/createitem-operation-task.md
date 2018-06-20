---
title: Opération CreateItem (tâche)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 12c5da4d-290c-4a8a-a965-0bf5d55c7978
description: L’opération CreateItem crée des éléments de tâche dans la banque d’informations Exchange.
ms.openlocfilehash: 5a5203202071ae9391faa9348902424317ee96d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755722"
---
# <a name="createitem-operation-task"></a>Opération CreateItem (tâche)

L’opération CreateItem crée des éléments de tâche dans la banque d’informations Exchange.
  
## <a name="task-createitem-request"></a>CreateItem demande de tâche

### <a name="description"></a>Description

Une demande CreateItem l’exemple suivant montre comment créer un élément de tâche dans une boîte aux lettres.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

Demandes de tâches périodiques soient modifiées quand ils sont reçus par l’ordinateur qui exécute Microsoft Exchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. Les modifications suivantes se produisent :
  
- Seule la date est enregistrée pour la propriété [StartDate (périodicité)](startdate-recurrence.md) de la plage de périodicité de la tâche. La partie heure est tronquée. 
    
- La propriété [StartDate (périodicité)](startdate-recurrence.md) peut-être être ajustée en fonction de la périodicité. Par exemple, si la périodicité est spécifiée comme tous les lundis et StartDate est défini sur le 26 octobre 2006, qui est un jeudi, StartDate est réglé à 30 octobre 2006, qui est le lundi. 
    
- Si la propriété [date de début](startdate.md) de la tâche est définie, il est mis à jour pour correspondre à la [date de début (périodicité)](startdate-recurrence.md) de la plage de périodicité. La propriété [DueDate](duedate.md) de la tâche est également mis à jour en fonction de la nouvelle [date de début](startdate.md).
    
- Si [date_début](startdate.md) n’est pas définie, seule la propriété [DueDate](duedate.md) est mis à jour pour correspondre à la [date de début (périodicité)](startdate-recurrence.md) de la plage de périodicité. 
    
Le tableau suivant présente les modifications apportées par le serveur d’accès au Client à une tâche périodique ayant un Task.Recurrence.Pattern de tous les lundis.
  
**Modifications apportées à une tâche périodique**

|**Propriété**|**Valeur d’origine**|**Valeur mise à jour**|
|:-----|:-----|:-----|
|Task.StartDate  <br/> |1er janvier 2006  <br/> |30 octobre 2006  <br/> |
|Task.DueDate  <br/> |3 janvier 2006  <br/> |1er novembre 2006  <br/> |
|Task.Recurrence.Range.StartDate  <br/> |26 octobre 2006  <br/> |30 octobre 2006  <br/> |
   
Par défaut, si un dossier de destination n’est pas spécifié, les éléments de tâche sont créés dans le dossier tâches.
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [CreateItem](createitem.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tâche](task.md)
    
- [Objet](subject.md)
    
- [DueDate](duedate.md)
    
- [Status](status.md)
    
## <a name="successful-task-createitem-response"></a>Réponse CreateItem réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à la demande CreateItem.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont inclus dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Tâche](task.md)
    
- [ID d’élément](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[CreateItem Operation](createitem-operation.md)


[Création de tâches](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Mise à jour de tâches](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Suppression de tâches](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

