---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: L’élément DeliveryStatus Spécifie l’état d’un message.
ms.openlocfilehash: 4e6f31e8ef4f98d8e838ba91167c7dd5d6ab2590
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755890"
---
# <a name="deliverystatus"></a>DeliveryStatus

L’élément **DeliveryStatus** Spécifie l’état d’un message. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un seul événement pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs de texte possibles pour l’élément **DeliveryStatus** . 
  
**Valeurs des éléments DeliveryStatus**

|**Valeur**|**Description**|
|:-----|:-----|
|Échec  <br/> |Spécifie qu’un message n’a pas été remis.  <br/> |
|En attente  <br/> |Spécifie que le message est en attente d’approbation d’un modérateur.  <br/> |
|Remis  <br/> |Spécifie que le message a été remis à tous les destinataires spécifiés.  <br/> |
|Transféré  <br/> |Spécifie que le message a été transféré vers un serveur à l’extérieur de l’étendue de recherche.  <br/> |
|Lire  <br/> |Spécifie que le message a été remis et lu par les destinataires.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **DeliveryStatus** est du type **MessageTrackingDeliveryStatusType** dans Exchange Server 2010. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

