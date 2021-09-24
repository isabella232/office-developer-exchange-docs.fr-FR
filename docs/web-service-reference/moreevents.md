---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: L’élément MoreEvents indique s’il existe d’autres événements dans la file d’attente à remettre au client.
ms.openlocfilehash: 7a19349e406a7e55e52c8a8cf0c3febba0a7301b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521808"
---
# <a name="moreevents"></a>MoreEvents

**L’élément MoreEvents** indique s’il existe d’autres événements dans la file d’attente à remettre au client. 
  
```xml
<MoreEvents/>
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
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente une valeur boolé américaine. La valeur **true indique** que d’autres événements sont dans la file d’attente. La valeur **false indique** qu’aucun autre événement n’est dans la file d’attente. Cette propriété est en lecture seule. 
  
## <a name="remarks"></a>Remarques

Dans le cas des notifications de pull, une valeur true dans cet élément indique au client qu’une autre demande GetEvents doit être émise pour obtenir les événements restants.  En supposant que les spécifications client nécessitent une latence minimale pour les notifications d’événements, les demandes GetEvents doivent continuer en continu jusqu’à ce qu’une valeur  **MoreEvents** fausse soit renvoyée. 
  
Dans le cas des notifications Push, une valeur true pour **MoreEvents** indique au client qu’une autre demande de notification sera envoyée au client pour remettre les événements restants.  Comme les notifications pull, ces demandes de suivi se poursuivent successivement jusqu’à ce que la file d’attente d’événements sur le serveur d’accès au client soit vide. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

