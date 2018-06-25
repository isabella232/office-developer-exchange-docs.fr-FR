---
title: GetRemindersResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b1c7288-2a98-4142-8961-4d2ebca5c37c
description: L’élément GetRemindersResponse spécifie la réponse à une demande de GetReminders.
ms.openlocfilehash: 1882ab377365908c0bc272059ab4e007c43d788c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756726"
---
# <a name="getremindersresponse"></a>GetRemindersResponse

L’élément **GetRemindersResponse** spécifie la réponse à une demande de **GetReminders** . 
  
```XML
<GetRemindersResponse>
   <Reminders></Reminders>
</GetRemindersResponse>

```

 **GetRemindersResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Rappels](reminders.md)
  
### <a name="parent-elements"></a>Éléments parents

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ResponseMessages](responsemessages.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

