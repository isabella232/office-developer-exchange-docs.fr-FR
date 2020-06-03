---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de contact partagées.
ms.openlocfilehash: 64b1e6d831068e9699e9cd47693e74919e0416a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526661"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a>SharingEffectiveRights (PermissionReadAccessType)

L’élément **SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de contact partagées. 
  
```XML
<SharingEffectiveRights>None | FullDetails</SharingEffectiveRights >
```

 **PermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts contenu dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **SharingEffectiveRights** . 
  
**Valeurs de texte de l’élément SharingEffectiveRights**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’utilisateur n’est pas autorisé à lire les éléments dans le dossier.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à lire tous les éléments dans le dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

