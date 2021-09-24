---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: L’élément MovedEvent représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.
ms.openlocfilehash: 4e0795fc3f335139e22fb51a4cf215a870ec62c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518133"
---
# <a name="movedevent"></a>MovedEvent

**L’élément MovedEvent représente** un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent. 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</MovedEvent>
```


**MovedCopiedEventType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Représente un signet d’événements dans la table des événements de boîte aux lettres.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Représente l’timestamp d’un événement de boîte aux lettres d’élément de déplacement/dossier.  <br/> |
|[FolderId](folderid.md) <br/> |Représente l’identificateur du dossier déplacé.  <br/> |
|[ItemId](itemid.md) <br/> |Représente l’identificateur de l’élément déplacé.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier qui contient l’élément ou le dossier déplacé.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Contient l’identificateur de dossier du dossier d’origine avant son déplacer ou sa copie.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contient l’identificateur unique de l’élément d’origine avant qu’il ne soit déplacé.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contient l’identificateur du dossier parent d’origine d’un élément ou d’un dossier déplacé.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produits depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

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

