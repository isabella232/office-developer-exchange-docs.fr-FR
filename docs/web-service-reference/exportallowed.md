---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: L’élément ExportAllowed Spécifie si l’exportation est activée.
ms.openlocfilehash: 5c07941e0a79394bbdaa1a1f62b20adedfe7a9bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756262"
---
# <a name="exportallowed"></a>ExportAllowed

L’élément **ExportAllowed** Spécifie si l’exportation est activée. 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Spécifie des informations sur la licence de gestion des droits.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **ExportAllowed** indique que l’exportation est autorisée. La valeur **false** indique que l’option exportation n’est pas autorisée. 
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

