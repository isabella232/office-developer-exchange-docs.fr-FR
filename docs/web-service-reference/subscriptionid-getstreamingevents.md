---
title: SubscriptionId (GetStreamingEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f86c178-2311-4844-82db-c2a0e469d116
description: L’élément SubscriptionId représente l’identificateur d’un abonnement de diffusion en continu.
ms.openlocfilehash: eb451e611c4922fa3b9cff7edec54dfb8260f5f5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838642"
---
# <a name="subscriptionid-getstreamingevents"></a>SubscriptionId (GetStreamingEvents)

L’élément **SubscriptionId** représente l’identificateur d’un abonnement de diffusion en continu. 
  
```XML
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetStreamingEvents](getstreamingevents.md) <br/> |Représente l’opération qui est utilisée par les clients pour demander des notifications de diffusion en continu à partir du serveur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur texte est requise. La valeur de texte est un GUID.
  
## <a name="remarks"></a>Remarques

Le GUID qui représente l’identificateur d’abonnement est généré par le serveur d’accès au Client lors de la création de l’abonnement.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetStreamingEvents](getstreamingevents-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

