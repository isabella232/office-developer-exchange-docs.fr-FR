---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: L’élément CopiedEvent représente un événement dans lequel un élément ou un dossier est copié.
ms.openlocfilehash: bc4902eb1e62344a7d5980ec573ac13b1bb084ee
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536592"
---
# <a name="copiedevent"></a>CopiedEvent

**L’élément CopiedEvent** représente un événement dans lequel un élément ou un dossier est copié. 
  
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
   <OldItemId/>
   <OldParentFolderId/>
</CopiedEvent>
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
|[TimeStamp](timestamp.md) <br/> |Représente l’timestamp d’un événement de boîte aux lettres d’élément/dossier de copie.  <br/> |
|[FolderId](folderid.md) <br/> |Représente l’identificateur du dossier.  <br/> |
|[ItemId](itemid.md) <br/> |Représente l’identificateur de l’élément.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Représente l’identificateur du dossier qui contient la copie.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Représente l’identificateur de dossier du dossier d’origine avant sa copie.  <br/> |
|[OldItemId](olditemid.md) <br/> |Contient l’identificateur unique de l’élément d’origine avant sa copie.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Contient l’identificateur du dossier parent d’origine d’un élément ou d’un dossier qui a été copié.  <br/> |
   
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
- [Utilisation des abonnements Pull](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [Exemple d'application de notification Push](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

