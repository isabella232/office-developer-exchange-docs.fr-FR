---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: L’élément RemoveItem représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation.
ms.openlocfilehash: c0cd5c1f9894287ee78c2f7a65b8f4d3b943414e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467689"
---
# <a name="removeitem"></a>RemoveItem

L’élément **RemoveItem** représente un objet de réponse qui est utilisé pour supprimer un élément de réunion lors de la réception d’un message MeetingCancellation. 
  
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
|**ObjectName** <br/> |Représente le nom de la classe d’objet de réponse RemoveItem sous la forme d’une chaîne en anglais.  <br/> |
   
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

 **RemoveItem** est valide uniquement pour un [MeetingCancellation](meetingcancellation.md). Sinon, une erreur est générée.
  
> [!NOTE]
> Le [ItemClass](itemclass.md) pour une annulation de réunion est IPM. Schedule. Meeting. Canceled. 
  
Pour supprimer un [propriété meetingrequest](meetingrequest.md) et les [CalendarItem](calendaritem.md)associés, utilisez l’objet Response [DeclineItem](declineitem.md) au lieu de **RemoveItem**.
  
 **RemoveItem** n’est pas pris en charge pour l’accès délégué. 
  
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

