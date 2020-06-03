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
description: L’élément MoreEvents indique s’il y a plus d’événements dans la file d’attente à remettre au client.
ms.openlocfilehash: fd12dd2e2e64ce1711e553ba5eb29bd0eb64c892
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462730"
---
# <a name="moreevents"></a>MoreEvents

L’élément **MoreEvents** indique s’il y a plus d’événements dans la file d’attente à remettre au client. 
  
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

La valeur de texte représente une valeur de type Boolean. La valeur **true** indique que d’autres événements se trouvent dans la file d’attente. La valeur **false** indique qu’aucun autre événement ne se trouve dans la file d’attente. Cette propriété est en lecture seule. 
  
## <a name="remarks"></a>Remarques

Dans le cas des notifications de type pull, une valeur **true** dans cet élément indique au client qu’une autre demande GetEvents doit être émise pour obtenir les autres événements. En supposant que les spécifications client requièrent une latence minimale pour les notifications d’événement, les demandes GetEvents doivent continuer en succession continue jusqu’à ce qu’une valeur **false** **MoreEvents** soit renvoyée. 
  
Dans le cas des notifications de type transmission, la valeur **true** pour **MoreEvents** indique au client qu’une autre demande de notification sera envoyée au client pour fournir les autres événements. De la même manière que pour les notifications de type pull, ces demandes de suivi se poursuivent en succession continue jusqu’à ce que la file d’attente d’événements sur le serveur d’accès au client soit vide. 
  
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

