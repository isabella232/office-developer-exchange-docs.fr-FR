---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: L’élément RemoveItem représente un objet de réponse utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation.
ms.openlocfilehash: 4dbe9ede36bf6e3c008a2186cfe617519ecfae1f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517958"
---
# <a name="removeitem"></a>RemoveItem

**L’élément RemoveItem** représente un objet de réponse utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation. 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**ObjectName** <br/> |Représente le nom de la classe d’objet de réponse RemoveItem en tant que chaîne anglaise.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Identifie l’élément auquel l’objet de réponse RemoveItem fait référence.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Contient un tableau d'éléments à créer dans le dossier qui est identifié par l'élément [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md).  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Contient une collection de tous les objets de réponse associés à un élément dans la banque d'informations Exchange.  <br/> |
   
## <a name="remarks"></a>Remarques

 **RemoveItem est** valide uniquement pour [un MeetingCancellation](meetingcancellation.md). Sinon, une erreur est lancée.
  
> [!NOTE]
> ItemClass [pour une](itemclass.md) annulation de réunion est IPM. Schedule.Meeting.Canceled. 
  
Pour supprimer un [MeetingRequest et](meetingrequest.md) l’objet [CalendarItem](calendaritem.md)associé, utilisez l’objet de réponse [DeclineItem](declineitem.md) au lieu **de RemoveItem**.
  
 **RemoveItem n’est** pas pris en charge pour l’accès délégué. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

