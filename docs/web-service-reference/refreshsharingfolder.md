---
title: RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 14571c28-effa-430a-802e-82fb99bafa7f
description: L’élément RefreshSharingFolder définit une demande pour actualiser le dossier local spécifié. Il s’agit de l’élément de base pour l’opération RefreshSharingFolder.
ms.openlocfilehash: b09e311d0ba38b0cdcc9fe0864ed3e2b0151b0fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829043"
---
# <a name="refreshsharingfolder"></a>RefreshSharingFolder

L’élément **RefreshSharingFolder** définit une demande pour actualiser le dossier local spécifié. Il s’agit de l’élément de base pour l' [opération RefreshSharingFolder](refreshsharingfolder-operation.md).
  
```xml
<RefreshSharingFolder>   <SharingFolderId/></RefreshSharingFolder>
```

 **RefreshSharingFolderType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SharingFolderId](sharingfolderid.md) <br/> |Représente l’identificateur du dossier local dans une relation de partage.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

