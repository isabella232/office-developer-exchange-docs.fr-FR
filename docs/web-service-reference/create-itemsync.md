---
title: Create (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: L’élément Create identifie un seul élément à créer dans le magasin de clients local.
ms.openlocfilehash: 2b36fad021c7ccb767eb80b31f71f12ef6cbbd22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510332"
---
# <a name="create-itemsync"></a>Create (ItemSync)

**L’élément Create** identifie un seul élément à créer dans le magasin de clients local. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) 
- [Modifications (éléments)](changes-items.md) 
- [Créer (ItemSync)](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Item](item.md) <br/> |Représente un élément générique Exchange à créer.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message Exchange message électronique à créer.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément Exchange calendrier à créer.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément Exchange contact à créer.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution à créer.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion à créer.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion à créer.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse de réunion à créer.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion à créer.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche à créer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Modifications (éléments)](changes-items.md) <br/> |Contient un tableau de séquences de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur Exchange serveur.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération SyncFolderItems](syncfolderitems-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

