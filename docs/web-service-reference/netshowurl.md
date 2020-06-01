---
title: NetShowUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NetShowUrl
api_type:
- schema
ms.assetid: a5d48fc1-b141-422c-bcb0-05d0f9ba90dd
description: L’élément NetShowUrl spécifie l’URL d’une réunion Microsoft NetShow online.
ms.openlocfilehash: 66e288a5e66eecf404698135cc3257085b852034
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466331"
---
# <a name="netshowurl"></a>NetShowUrl

L’élément **NetShowUrl** spécifie l’URL d’une réunion Microsoft NetShow online. 
  
```xml
<NetShowUrl/>
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
|[Propriété meetingrequest](meetingrequest.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une URL est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cette propriété NetShowUrl est accessible en lecture pour l’élément de calendrier de l’organisateur. Elle est en lecture seule pour les demandes de réunion et pour les participants.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

