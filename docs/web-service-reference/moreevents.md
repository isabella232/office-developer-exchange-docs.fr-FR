---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: L’élément MoreEvents indique s’il existe plusieurs événements dans la file d’attente pour être remis au client.
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828489"
---
# <a name="moreevents"></a>MoreEvents

L’élément **MoreEvents** indique s’il existe plusieurs événements dans la file d’attente pour être remis au client. 
  
```xml
<MoreEvents/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente une valeur de type Boolean. La valeur **true** indique que plusieurs événements sont dans la file d’attente. La valeur **false** indique que plus aucun événement ne se trouvent dans la file d’attente. Cette propriété est en lecture seule. 
  
## <a name="remarks"></a>Remarques

Dans le cas des notifications de type Pull, la valeur **true** dans cet élément indique au client qu’une autre demande GetEvents doit être émise pour obtenir les autres événements. En supposant que les spécifications client nécessitent latence minimale pour les notifications d’événements, les demandes GetEvents devraient continuer dans une suite continue jusqu'à ce qu’un **faux** valeur **MoreEvents** est retourné. 
  
Dans le cas de notifications Push, la valeur **true** pour **MoreEvents** indique au client qu’un autre notification demande sera envoyée au client pour fournir les autres événements. Similaire aux notifications de type Pull, ces demandes suivis continuera à la suite continue jusqu'à ce que la file d’attente sur le serveur d’accès au Client est vide. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

