---
title: InternetMessageHeaders
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InternetMessageHeaders
api_type:
- schema
ms.assetid: 4dcf8671-96df-4a2d-9836-7e8e3a67e0db
description: L’élément InternetMessageHeaders contient une collection de certains en-têtes de message Internet contenus dans un élément d’une boîte aux lettres. Pour obtenir l’ensemble de la collection d’en-têtes de messages Internet, utilisez la propriété PR_TRANSPORT_MESSAGE_HEADERS. Pour plus d’informations sur EWS et les en-têtes de message Internet, voir En-têtes de message Internet EWS, MIME et les en-têtes de message Internet manquants.
ms.openlocfilehash: 1ea49f2d5cc31aef09a9bc6d38dff25652696842
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541078"
---
# <a name="internetmessageheaders"></a>InternetMessageHeaders

**L’élément InternetMessageHeaders** contient une collection de certains en-têtes de message Internet contenus dans un élément d’une boîte aux lettres. Pour obtenir l’ensemble de la collection d’en-têtes de messages Internet, utilisez **la PR_TRANSPORT_MESSAGE_HEADERS** internet. Pour plus d’informations sur EWS et les en-têtes de message Internet, voir « Obtention d’en-têtes de message Internet » dans [EWS, MIME](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)et les en-têtes de message Internet manquants.
  
```XML
<InternetMessageHeaders>
   <InternetMessageHeader/>
</InternetMessageHeaders>
```

 **NonEmptyArrayOfInternetHeadersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[InternetMessageHeader](internetmessageheader.md) <br/> |Représente l’en-tête de message Internet pour un en-tête donné au sein de la collection d’en-têtes.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AcceptItem](acceptitem.md) <br/> |Représente une réponse à accepter à une demande de réunion.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente la réponse à une demande de réunion acceptée provisoirement.  <br/> |
   
## <a name="remarks"></a>Remarques

Voici la définition de propriété étendue de l’API gérée EWS pour **PR_TRANSPORT_MESSAGE_HEADERS** propriété. 
  
```cs
ExtendedPropertyDefinition transportMsgHdr = new ExtendedPropertyDefinition(0x007D, MapiPropertyType.String);
```

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[EWS, MIME et en-têtes de message Internet manquants](https://msdn.microsoft.com/library/exchange/hh545614%28v=exchg.140%29.aspx)

