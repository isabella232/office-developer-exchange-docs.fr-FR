---
title: Créer (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: L’élément créer identifie un élément unique à créer dans le magasin du client local.
ms.openlocfilehash: 39056bcaab3577b1b729421118a45571910922fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755679"
---
# <a name="create-itemsync"></a>Créer (ItemSync)

L’élément **créer** identifie un élément unique à créer dans le magasin du client local. 
  
[SyncFolderItemsResponse](syncfolderitemsresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
  
[Modifications (éléments)](changes-items.md)
  
[Créer (ItemSync)](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

 **SyncFolderItemsCreateOrUpdateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Item](item.md) <br/> |Représente un élément Exchange générique à créer.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique d’Exchange à créer.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange à créer.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange à créer.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution à créer.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion à créer.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion à créer.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion à créer.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion à créer.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche à créer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Modifications (éléments)](changes-items.md) <br/> |Contient un tableau de séquence de types de modification qui représentent les types de différences entre les éléments sur le client et les éléments sur le serveur Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

