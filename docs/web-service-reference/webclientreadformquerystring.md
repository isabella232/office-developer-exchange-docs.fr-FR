---
title: WebClientReadFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WebClientReadFormQueryString
api_type:
- schema
ms.assetid: 13e8871a-32a6-4bb9-9493-864c4c07efff
description: L’élément WebClientReadFormQueryString représente une URL à concaténer au point de terminaison Outlook Web App pour lire un élément dans Outlook Web App.
ms.openlocfilehash: 10035aa001c74926ae36e96e09b5b2995844cb68
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538470"
---
# <a name="webclientreadformquerystring"></a>WebClientReadFormQueryString

**L’élément WebClientReadFormQueryString** représente une URL à concaténer au point de terminaison Outlook Web App pour lire un élément dans Outlook Web App. 
  
```XML
<WebClientReadFormQueryString/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément de publication dans la Exchange store.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

L’identificateur d’élément Outlook URL Web App est l’identificateur EWS de l’élément. Vous pouvez coder l’identificateur d’élément EWS en URL et l’appendre à la chaîne de requête pour obtenir l’URL Outlook Web App pour un élément.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
### <a name="version-differences"></a>Différences entre les versions

Les versions de Exchange commençant par la version principale 15 et se terminant par Exchange Server 2013 build 15.0.775.38 (CU3) et Exchange Online version 15.00.0775.009 ne retournent pas un fragment de chaîne de requête correct dans l’élément **WebClientReadFormQueryString.** 
  
Dans les versions Exchange antérieures à la version principale 15, l’identificateur d’élément pour les URL Outlook Web App est un identificateur web app Outlook. Si vous ciblez une version de Exchange antérieure à la version majeure 15, vous devez utiliser l’opération [ConvertId](convertid-operation.md) pour convertir l’identificateur. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

