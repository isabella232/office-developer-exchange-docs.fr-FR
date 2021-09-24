---
title: ModifiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ModifiedEvent
api_type:
- schema
ms.assetid: ca1309f4-2df7-4289-811c-75c3db0e7072
description: L’élément ModifiedEvent représente un événement dans lequel un élément ou un dossier est modifié.
ms.openlocfilehash: 92002c2824168687e6984913dbf46ee85da921e7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539358"
---
# <a name="modifiedevent"></a>ModifiedEvent

**L’élément ModifiedEvent** représente un événement dans lequel un élément ou un dossier est modifié. 
  
```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

```xml
<ModifiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/> 
   <ParentFolderId/>
   <UnreadCount/>
</ModifiedEvent>
```

**ModifiedEventType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Représente un signet d’événement dans la table des événements de boîte aux lettres.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Représente l’timestamp d’un événement de boîte aux lettres d’élément ou de dossier modifié.  <br/> |
|[FolderId](folderid.md) <br/> |Représente l’identificateur du dossier modifié.  <br/> |
|[ItemId](itemid.md) <br/> |Représente l’identificateur de l’élément modifié.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier parent de l’élément ou dossier modifié.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Représente le nombre d’éléments non lus dans un dossier donné.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

Deux événements modifiés sont générés pour chaque modification d’un élément dans un dossier. Un événement est pertinent pour l’élément qui a été modifié. L’autre événement est pertinent pour le dossier parent de l’élément. Il s’agit du même dossier que celui sur qui l’abonnement a été créé. L’événement associé au dossier est utilisé pour communiquer une modification potentielle à la [propriété UnreadCount](unreadcount.md) sur le dossier. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération d'abonnement](subscribe-operation.md)  
- [Opération de GetEvents](getevents-operation.md)  
- [Opération de résiliation d'abonnement](unsubscribe-operation.md)

