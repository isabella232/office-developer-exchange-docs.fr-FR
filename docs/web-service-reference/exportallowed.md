---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: L’élément ExportAllowed spécifie si l’exportation est activée.
ms.openlocfilehash: f5a9aa3040c45d535ef338010bb37bcedb797ffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460630"
---
# <a name="exportallowed"></a>ExportAllowed

L’élément **ExportAllowed** spécifie si l’exportation est activée. 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Spécifie les informations relatives à la licence de gestion des droits.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **ExportAllowed** indique que l’exportation est autorisée. La valeur **false** indique que l’exportation n’est pas autorisée. 
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

