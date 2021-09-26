---
title: DeliveryStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliveryStatus
api_type:
- schema
ms.assetid: eab55db3-affb-42be-a586-5caa04052433
description: L’élément DeliveryStatus spécifie l’état d’un message.
ms.openlocfilehash: f11952f401e0d22d780725598bfb32cbd3a8d622
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543386"
---
# <a name="deliverystatus"></a>DeliveryStatus

**L’élément DeliveryStatus** spécifie l’état d’un message. 
  
```XML
<DeliveryStatus>Unsuccessful | Pending | Delivered | Transferred | Read</DeliveryStatus>
```

 **MessageTrackingDeliveryStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientTrackingEvent](recipienttrackingevent.md) <br/> |Contient des informations pour un événement unique pour un destinataire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs de texte possibles pour **l’élément DeliveryStatus.** 
  
**Valeurs des éléments DeliveryStatus**

|**Valeur**|**Description**|
|:-----|:-----|
|Échec  <br/> |Spécifie qu’un message n’a pas été remis.  <br/> |
|En attente  <br/> |Spécifie que le message attend l’approbation d’un modérateur.  <br/> |
|Remis  <br/> |Spécifie que le message a été remis à tous les destinataires spécifiés.  <br/> |
|Transféré  <br/> |Spécifie que le message a été transféré vers un serveur en dehors de l’étendue de recherche.  <br/> |
|Lire  <br/> |Spécifie que le message a été remis et lu par les destinataires.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément DeliveryStatus** était de type **MessageTrackingDeliveryStatusType** Exchange Server 2010. 
  
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

