---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: L’élément CopiedEvent représente un événement dans lequel un élément ou un dossier est copié.
ms.openlocfilehash: 7ebfbb744a80e3a2d14ee9e0e1b952d2269dbf94
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353167"
---
# <a name="copiedevent"></a>CopiedEvent

L’élément **CopiedEvent** représente un événement dans lequel un élément ou un dossier est copié. 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

**MovedCopiedEventType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Représente un signet d’événements dans la table d’événements de boîte aux lettres.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Représente l’horodatage d’un événement de boîte aux lettres de dossier d’éléments de copie.  <br/> |
|[FolderId](folderid.md) <br/> |Représente l’identificateur du dossier.  <br/> |
|[ID d’élément](itemid.md) <br/> |Représente l’identificateur de l’élément.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier qui contient la copie.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Représente l’identificateur de dossier du dossier d’origine avant qu’il a été copié.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contient l’identificateur unique de l’élément d’origine avant qu’il a été copié.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contient l’identificateur du dossier parent d’origine d’un élément ou d’un dossier qui a été copié.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Notification](notification-ex15websvcsotherref.md) <br/> |Contient des informations sur l’abonnement et les événements qui se sont produites depuis la dernière notification.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération d'abonnement](subscribe-operation.md) 
- [Opération de GetEvents](getevents-operation.md) 
- [Opération de résiliation d'abonnement](unsubscribe-operation.md)
- [À l’aide d’abonnement](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [Exemple d'application de notification Push](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

