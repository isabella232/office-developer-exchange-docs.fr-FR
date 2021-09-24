---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: L’élément PhoneCallState spécifie l’état actuel d’un appel téléphonique.
ms.openlocfilehash: 8c0b8357b58826f18f05eb0fedc0865be1623c2b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528301"
---
# <a name="phonecallstate"></a>PhoneCallState

**L’élément PhoneCallState** spécifie l’état actuel d’un appel téléphonique. 
  
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
|[PhoneCallInformation](phonecallinformation.md) <br/> |Spécifie les informations d’état d’un appel téléphonique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément PhoneCallState.** 
  
**Valeurs des éléments PhoneCallState**

|**Valeur**|**Description**|
|:-----|:-----|
|Inactif  <br/> |État initial de l’appel.  <br/> |
|Connexion  <br/> |Le système compose cet appel.  <br/> |
|Alerted  <br/> |L’appel est en état d’alerte (le téléphone sonne).  <br/> |
|Connecté  <br/> |L’appel est dans l’état connecté.  <br/> |
|Déconnecté  <br/> |L’appel est déconnecté.  <br/> |
|Entrant  <br/> |L’appel est entrant.  <br/> |
|Transfert  <br/> |L’appel est transféré vers une autre destination.  <br/> |
|Forwarding  <br/> |L’appel est transmis à une autre destination.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire /ews/ de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

