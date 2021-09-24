---
title: Éléments
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Items
api_type:
- schema
ms.assetid: 0811a73e-bf1f-4889-9219-73902dd47639
description: L’élément Items contient un tableau d’éléments.
ms.openlocfilehash: b6e9db6524640098a902f431393fccd6bd4e8868
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540886"
---
# <a name="items"></a>Éléments

**L’élément Items** contient un tableau d’éléments. 
  
```xml
<Items>
   <Item/>
   <Message/>
   <CalendarItem/>
   <Contact/>
   <DistributionList/>
   <MeetingMessage/>
   <MeetingRequest/>
   <MeetingResponse/>
   <MeetingCancellation/>
   <Task/>
   <PostItem/>
</Items>
```

 **ArrayOfRealItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente un message de réunion dans le magasin Exchange de réunion.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CopyItemResponseMessage](copyitemresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération CopyItem.](copyitem-operation.md)  <br/> |
|[CreateItemResponseMessage](createitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération CreateItem](createitem-operation.md) unique.  <br/> |
|[GetItemResponseMessage](getitemresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération GetItem.](getitem-operation.md)  <br/> |
|[GroupedItems](groupeditems.md) <br/> |Représente une collection d’éléments résultant d’un appel d’opération [FindItem groupé.](finditem-operation.md)  <br/> |
|[MoveItemResponseMessage](moveitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération MoveItem.](moveitem-operation.md)  <br/> |
|[RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md) <br/> |Contient les résultats d’une recherche d’un dossier racine unique au cours [d’une opération FindItem](finditem-operation.md).  <br/> |
|[UpdateItemResponseMessage](updateitemresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération UpdateItem.](updateitem-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Pour plus d’informations sur l’ensemble d’éléments dans une demande d’opération [CreateItem,](createitem-operation.md) voir [Items (NonEmptyArrayOfAllItemsType).](items-nonemptyarrayofallitemstype.md)
  
[Les](message-ex15websvcsotherref.md) éléments de message représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma Exchange Web Services (EWS). Éléments tels que IPM. Le partage et IPM.InfoPath sont renvoyés en tant **qu’éléments message.** Les versions de Exchange à partir Exchange Server 2010 ne retournent pas l’élément [Item](item.md) de base dans les réponses. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Référence EWS pour Exchange](ews-reference-for-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

