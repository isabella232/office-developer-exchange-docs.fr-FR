---
title: SharingEffectiveRights (PermissionReadAccessType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SharingEffectiveRights
api_type:
- schema
ms.assetid: 808bb4a1-aa2d-48c5-94b3-551b52c348bd
description: L’élément SharingEffectiveRights indique les autorisations dont dispose l’utilisateur pour les données de contact en cours de partage.
ms.openlocfilehash: ecae44dd99f61e1e59648134d10190a758a28b17
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531778"
---
# <a name="sharingeffectiverights-permissionreadaccesstype"></a>SharingEffectiveRights (PermissionReadAccessType)

**L’élément SharingEffectiveRights** indique les autorisations dont dispose l’utilisateur pour les données de contact en cours de partage. 
  
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
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier Contacts contenu dans une boîte aux lettres.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément SharingEffectiveRights.** 
  
**Valeurs de texte de l’élément SharingEffectiveRights**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’utilisateur n’est pas autorisé à lire les éléments du dossier.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à lire tous les éléments du dossier.  <br/> |
   
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

