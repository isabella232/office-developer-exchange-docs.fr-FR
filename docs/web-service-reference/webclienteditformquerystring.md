---
title: WebClientEditFormQueryString
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WebClientEditFormQueryString
api_type:
- schema
ms.assetid: 9e571021-d58f-424b-8db2-48cf683533dc
description: L’élément WebClientEditFormQueryString représente une URL à concaténer au point de terminaison d’Outlook Web App pour modifier un élément dans Outlook Web App.
ms.openlocfilehash: d6f20d1342746a764f754a6b20633a7bded3f6c1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464986"
---
# <a name="webclienteditformquerystring"></a>WebClientEditFormQueryString

L’élément **WebClientEditFormQueryString** représente une URL à concaténer au point de terminaison d’Outlook Web App pour modifier un élément dans Outlook Web App. 
  
```XML
<WebClientEditFormQueryString/>
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
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément post dans la Banque d’Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Pour les versions d’Exchange à partir d’Exchange Server 2013, y compris Exchange Online, utilisez les informations de l’élément [WebClientReadFormQueryString](webclientreadformquerystring.md) pour ouvrir un brouillon dans Outlook Web App, puis utilisez l’interface utilisateur pour modifier l’élément de brouillon. L’élément **WebClientEditFormQueryString** ne s’applique pas aux versions d’Exchange commençant par exchange Server 2013, y compris Exchange Online. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

