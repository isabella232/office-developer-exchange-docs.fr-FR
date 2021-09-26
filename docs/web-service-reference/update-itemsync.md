---
title: Update (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: L’élément Update identifie un seul élément à mettre à jour dans le magasin de clients local.
ms.openlocfilehash: 936226c671916b974eed9dea9ad2ea39bde482a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541818"
---
# <a name="update-itemsync"></a>Update (ItemSync)

**L’élément Update** identifie un seul élément à mettre à jour dans le magasin de clients local. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Modifications (éléments)](changes-items.md)  
- [Mise à jour (ItemSync)](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Item](item.md) <br/> |Représente un élément générique Exchange à mettre à jour.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message Exchange message électronique à mettre à jour.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément Exchange calendrier à mettre à jour.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément Exchange contact à mettre à jour.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution à mettre à jour.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion à mettre à jour.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion à mettre à jour.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse de réunion à mettre à jour.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion à mettre à jour.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche à mettre à jour.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Modifications (éléments)](changes-items.md) <br/> |Contient un tableau de séquences de types de modification qui représentent le type de différences entre les éléments sur le client et les éléments sur le Exchange serveur.  <br/> |
   
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

