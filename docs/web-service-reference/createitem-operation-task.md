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
description: L’opération CreateItem crée des éléments de tâche dans la Banque d’Exchange.
ms.openlocfilehash: 502108843193e7ed8377b0fade9e106ef3d1976c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457101"
---
# <a name="createitem-operation-task"></a>Opération CreateItem (tâche)

L’opération CreateItem crée des éléments de tâche dans la Banque d’Exchange.
  
## <a name="task-createitem-request"></a>Demande CreateItem de la tâche

### <a name="description"></a>Description

L’exemple de requête CreateItem suivant montre comment créer un élément de tâche dans une boîte aux lettres.
  
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

Les demandes de tâches périodiques sont modifiées lorsqu’elles sont reçues par l’ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé. Les modifications suivantes se produisent :
  
- Seule la date est enregistrée pour la propriété [StartDate (Recurrence)](startdate-recurrence.md) de la plage de périodicité de la tâche. Le composant d’heure est tronqué. 
    
- La propriété [StartDate (Recurrence)](startdate-recurrence.md) peut être ajustée, en fonction de la périodicité. Par exemple, si la périodicité est définie à chaque lundi et que la valeur de StartDate est fixée au 26 octobre 2006, soit un jeudi, la valeur de StartDate est ajustée à 30 octobre 2006, qui est le lundi suivant. 
    
- Si la propriété [StartDate](startdate.md) de la tâche est définie, elle est mise à jour pour correspondre à la valeur [StartDate (périodicité)](startdate-recurrence.md) de la plage de périodicité. La propriété [DueDate](duedate.md) de la tâche est également mise à jour en fonction de la nouvelle [StartDate](startdate.md).
    
- Si la propriété [StartDate](startdate.md) n’est pas définie, seule la propriété [DueDate](duedate.md) est mise à jour pour correspondre à la valeur [StartDate (périodicité)](startdate-recurrence.md) de la plage de périodicité. 
    
Le tableau suivant présente les modifications apportées par le serveur d’accès au client à une tâche périodique qui a une tâche. Recurrence. Pattern de chaque lundi.
  
**Modifications apportées à une tâche périodique**

|**Property**|**Valeur d’origine**|**Valeur mise à jour**|
|:-----|:-----|:-----|
|Task. StartDate  <br/> |1er janvier 2006  <br/> |30 octobre 2006  <br/> |
|Task. DueDate  <br/> |Le 3 janvier 2006  <br/> |1er novembre 2006  <br/> |
|Task. Recurrence. Range. StartDate  <br/> |26 octobre 2006  <br/> |30 octobre 2006  <br/> |
   
Par défaut, si aucun dossier de destination n’est spécifié, les éléments de tâche sont créés dans le dossier tâches.
  
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [CreateItem](createitem.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [Subject](subject.md)
    
- [DueDate](duedate.md)
    
- [Status](status.md)
    
## <a name="successful-task-createitem-response"></a>Réponse CreateItem de la tâche réussie

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

Les éléments suivants sont inclus dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateItemResponse](createitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateItemResponseMessage](createitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Task](task.md)
    
- [ItemId](itemid.md)
    
## <a name="see-also"></a>Voir aussi



[Opération CreateItem](createitem-operation.md)


[Création de tâches](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[Mise à jour des tâches](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)
  
[Suppression de tâches](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

