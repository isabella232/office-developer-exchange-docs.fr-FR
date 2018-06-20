---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: L’élément SharedFolderId représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une requête d’opération GetSharingFolder.
ms.openlocfilehash: 6d4e541ef3cae89e413efa8cc5f1beaf651dc4dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829477"
---
# <a name="sharedfolderid"></a>SharedFolderId

L’élément **SharedFolderId** représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) . 
  
```xml
<SharedFolderId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |Définit une demande pour obtenir l’identificateur de dossier local d’un dossier partagé spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte est une chaîne qui représente l’identificateur du dossier partagé pour lequel l’identificateur de dossier local doit être retournée par une demande [d’opération GetSharingFolder](getsharingfolder-operation.md) . 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetSharingFolder](getsharingfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

