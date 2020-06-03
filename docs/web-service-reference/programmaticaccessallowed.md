---
title: ProgrammaticAccessAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a1fc7dff-a303-4809-b7f4-9672f86c183c
description: L’élément ProgrammaticAccessAllowed spécifie si l’accès par programme est activé pour les données gérées par des droits.
ms.openlocfilehash: 8a5cf4e57a97807e5940a0402768d7123b9912d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465638"
---
# <a name="programmaticaccessallowed"></a>ProgrammaticAccessAllowed

L’élément **ProgrammaticAccessAllowed** spécifie si l’accès par programme est activé pour les données gérées par des droits. 
  
```XML
<ProgrammaticAccessAllowed> true | false </ProgrammaticAccessAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[RightsManagementLicenseData](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **ProgrammaticAccessAllowed** indique que les données sont accessibles par programme. La valeur **false** indique que les données ne sont pas accessibles par programme. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

