---
title: ExtractAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc213f0e-a655-44e9-9ac9-bc1673bae1fe
description: L’élément ExtractAllowed indique si l’extraction d’entités est activée.
ms.openlocfilehash: 48584e50be0ff66d156d9a3c3768729d63a9a3fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756345"
---
# <a name="extractallowed"></a>ExtractAllowed

L’élément **ExtractAllowed** indique si l’extraction d’entités est activée. 
  
```XML
<ExtractAllowed>true | false</ExtractAllowed
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

Une valeur de texte de **la valeur true** pour l’élément **ExtractAllowed** indique que l’extraction d’entités est activé. La valeur **false** indique que l’extraction d’entités n’est pas activé. 
  
## <a name="remarks"></a>Remarques

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

