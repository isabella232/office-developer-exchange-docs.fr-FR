---
title: IsMeetingRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingRequest
api_type:
- schema
ms.assetid: 72102a55-fd51-4ec9-abce-9a4ec45b86d2
description: L’élément IsMeetngRequest indique si les messages entrants doivent être une demande de réunion afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 8b4969faaeb7dfa98edbf4fe8747e8b783808313
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465960"
---
# <a name="ismeetingrequest"></a>IsMeetingRequest

L’élément **IsMeetngRequest** indique si les messages entrants doivent être une demande de réunion afin que la condition ou l’exception s’applique. 
  
```XML
<IsMeetingRequest>true | false</IsMeetingRequest>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conditions](conditions.md) <br/> |Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** indique que le message doit être une demande de réunion afin que la condition ou l’exception s’applique. La valeur **false** indique que le message ne doit pas être une demande de réunion afin que la condition ou l’exception s’applique. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

