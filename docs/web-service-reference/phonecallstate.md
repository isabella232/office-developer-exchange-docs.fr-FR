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
description: L’élément PhoneCallState Spécifie l’état actuel d’un appel téléphonique.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828761"
---
# <a name="phonecallstate"></a>PhoneCallState

L’élément **PhoneCallState** Spécifie l’état actuel d’un appel téléphonique. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Spécifie les informations d’état pour un appel téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **PhoneCallState** . 
  
**Valeurs des éléments PhoneCallState**

|**Valeur**|**Description**|
|:-----|:-----|
|Inactif  <br/> |État de l’appel initial.  <br/> |
|Connexion  <br/> |Le système appelle cet appel.  <br/> |
|Alerté  <br/> |L’appel se trouve dans l’alerte d’état (téléphone sonne).  <br/> |
|Connecté  <br/> |L’appel est dans l’état connecté.  <br/> |
|Déconnecté  <br/> |L’appel est déconnecté.  <br/> |
|Entrant  <br/> |L’appel est entrant.  <br/> |
|Transfert  <br/> |L’appel est transféré vers une autre destination.  <br/> |
|Transfert  <br/> |L’appel est transféré vers une autre destination.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire /ews/ de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

