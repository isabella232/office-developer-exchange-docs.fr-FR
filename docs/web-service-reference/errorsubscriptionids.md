---
title: ErrorSubscriptionIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrorSubscriptionIds
api_type:
- schema
ms.assetid: e64e76ff-4d98-4082-9acc-a1114ae45f44
description: L’élément ErrorSubscriptionIds contient un tableau d’ID d’abonnement non valides.
ms.openlocfilehash: 7a84a945991e0c002701586e21f5e8612c884334
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545208"
---
# <a name="errorsubscriptionids"></a>ErrorSubscriptionIds

**L’élément ErrorSubscriptionIds contient** un tableau d’ID d’abonnement non valides. 
  
```xml
<ErrorSubscriptionIds>
   <SubscriptionId/>
</ErrorSubscriptionIds>
```

 **NonEmptyArrayOfSubscriptionIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SubscriptionId (GetEvents)](subscriptionid-getevents.md) <br/> |Représente l’identificateur d’un abonnement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetStreamingEvents](getstreamingevents-operation.md) unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages et https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma des messages ; Schéma types  <br/> |
|Fichier de validation  <br/> |Messages.xsd; Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetStreamingEvents](getstreamingevents-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

