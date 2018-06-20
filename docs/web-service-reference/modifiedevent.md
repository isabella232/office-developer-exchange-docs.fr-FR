---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: L’élément ModifiedEvent représente un événement auquel un élément ou un dossier est modifiée.
ms.openlocfilehash: fb464fb0a270d8ca7d33d40e5425e260970b2f1e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828482"
---
# <a name="modifiedevent"></a>ModifiedEvent

L’élément **ModifiedEvent** représente un événement auquel un élément ou un dossier est modifiée. 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

 **ModifiedEventType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Filigrane](watermark.md) <br/> |Représente un signet d’événements dans la table d’événements de boîte aux lettres.  <br/> |
|[Horodatage](timestamp.md) <br/> |Représente l’horodatage d’un événement de boîte aux lettres élément ou le dossier modifié.  <br/> |
|[FolderId](folderid.md) <br/> |Représente l’identificateur du dossier modifié.  <br/> |
|[ID d’élément](itemid.md) <br/> |Représente l’identificateur de l’élément modifié.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent de l’élément modifié ou d’un dossier.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Représente le nombre d’éléments non lus dans un dossier donné.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

Deux événements modifiés sont générés pour chaque modification d’un élément dans un dossier. Un événement s’applique à l’élément qui a été modifié. L’événement est pertinent pour le dossier parent de l’élément. Voici le même dossier que l’abonnement a été créé par rapport à. L’événement qui est associé au dossier est utilisé pour communiquer une modification à la propriété [UnreadCount](unreadcount.md) sur le dossier potentielle. 
  
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

