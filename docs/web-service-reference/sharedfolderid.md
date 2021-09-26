---
title: SharedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharedFolderId
api_type:
- schema
ms.assetid: 21181ba3-9626-4284-9717-0b1c16948e8f
description: L’élément SharedFolderId représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d’opération GetSharingFolder.
ms.openlocfilehash: 7e47ba49abed99bdb3cfd00eb43d2ef276d4ef37
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545971"
---
# <a name="sharedfolderid"></a>SharedFolderId

**L’élément SharedFolderId** représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d’opération [GetSharingFolder.](getsharingfolder-operation.md) 
  
```xml
<SharedFolderId/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetSharingFolder](getsharingfolder.md) <br/> |Définit une demande d’obtenir l’identificateur de dossier local d’un dossier partagé spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est une chaîne qui représente l’identificateur du dossier partagé dont l’identificateur de dossier local doit être renvoyé par une demande d’opération [GetSharingFolder.](getsharingfolder-operation.md) 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetSharingFolder](getsharingfolder-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

