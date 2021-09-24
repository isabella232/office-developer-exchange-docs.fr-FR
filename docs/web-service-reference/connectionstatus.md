---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: L’élément ConnectionStatus fournit une description textuelle de l’état d’un abonnement de diffusion en continu.
ms.openlocfilehash: 05ff80ac3e6c3c8bf1341a179a14c9d052c9947f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536850"
---
# <a name="connectionstatus"></a>ConnectionStatus

**L’élément ConnectionStatus** fournit une description textuelle de l’état d’un abonnement de diffusion en continu. 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 **ConnectionStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetStreamingEventsResponseMessage](getstreamingeventsresponsemessage.md) <br/> |Contient l’état et le résultat d’une [demande d’opération GetStreamingEvents](getstreamingevents-operation.md) unique.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise. Voici les valeurs de texte possibles pour cet élément :
  
- OK
    
- Fermé
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetStreamingEvents](getstreamingevents-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

