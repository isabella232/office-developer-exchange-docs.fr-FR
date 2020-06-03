---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: L’élément PhoneCallState spécifie l’état actuel d’un appel téléphonique.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468529"
---
# <a name="phonecallstate"></a>PhoneCallState

L’élément **PhoneCallState** spécifie l’état actuel d’un appel téléphonique. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Spécifie les informations d’État pour un appel téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **PhoneCallState** . 
  
**Valeurs de l’élément PhoneCallState**

|**Valeur**|**Description**|
|:-----|:-----|
|Engrenage  <br/> |État initial de l’appel.  <br/> |
|Connexion  <br/> |Le système compose cet appel.  <br/> |
|Averti  <br/> |L’appel est en état d’alerte (sonnerie du téléphone).  <br/> |
|Connecté  <br/> |L’appel est à l’état connecté.  <br/> |
|Déconnecté  <br/> |L’appel est déconnecté.  <br/> |
|Entrant  <br/> |L’appel est entrant.  <br/> |
|Transférés  <br/> |L’appel est transféré vers une autre destination.  <br/> |
|Transfert  <br/> |L’appel est transféré vers une autre destination.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

