---
title: UserRoles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: be003e12-3496-468d-a61c-48af0b819654
description: L’élément UserRoles spécifie les rôles d’utilisateur que l’utilisateur appelant, ou l’utilisateur que l’application partenaire d’appel agit, souhaite appliquer à l’appel actuel.
ms.openlocfilehash: c861cda9a010e909c9ecc5303ddc637a14bcb824
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514976"
---
# <a name="userroles"></a>UserRoles

**L’élément UserRoles** spécifie les rôles d’utilisateur que l’utilisateur appelant, ou l’utilisateur que l’application partenaire d’appel agit, souhaite appliquer à l’appel actuel. 
  
```XML
<UserRoles>
   <Role/>
</UserRoles>
```

 **NonEmptyArrayOfRoleType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Role](role.md)
  
### <a name="parent-elements"></a>Éléments parents

[ManagementRole](managementrole.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

