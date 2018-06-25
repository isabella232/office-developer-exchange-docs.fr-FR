---
title: MeetingRequestType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequestType
api_type:
- schema
ms.assetid: bcd5c97c-19aa-4b1d-a8e8-e8c4bd473dd9
description: L’élément MeetingRequestType décrit le type de la demande de réunion.
ms.openlocfilehash: 7269587e2fa72aeb9070a7b53ee9215829729329
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828432"
---
# <a name="meetingrequesttype"></a>MeetingRequestType

L’élément **MeetingRequestType** décrit le type de la demande de réunion. 
  
```xml
<MeetingRequestType/>
```

 **MeetingRequestTypeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. Le tableau suivant répertorie les valeurs de texte possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|FullUpdate  <br/> |Identifie la demande de réunion en tant qu’une mise à jour complète pour une requête existante. Une mise à jour intégrale a mis à jour le contenu d’information et du temps.  <br/> |
|InformationalUpdate  <br/> |Identifie la demande de réunion contenant uniquement de mise à jour le contenu d’information.  <br/> |
|NewMeetingRequest  <br/> |Identifie la demande de réunion en tant qu’une nouvelle demande de réunion.  <br/> |
|Aucun  <br/> |Indique que la demande de réunion type n’est pas défini.  <br/> |
|Obsolètes  <br/> |Identifie la demande de réunion est obsolète.  <br/> |
|PrincipalWantsCopy  <br/> |Indique que la demande de réunion appartient à une entité qui a transféré des messages de réunion à un délégué et sa copie marqué comme d’information.  <br/> |
|SilentUpdate  <br/> |Identifie la demande de réunion en tant qu’une mise à jour en mode silencieux à une réunion existante.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

