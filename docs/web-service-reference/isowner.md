---
title: IsOwner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ea0f0afc-32fe-46cb-8530-62a6ce9490f6
description: L’élément IsOwner spécifie si l’utilisateur de messagerie spécifié en est le propriétaire.
ms.openlocfilehash: 7e3baaf0f3fb2eac028117622eedd57088d71612
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541006"
---
# <a name="isowner"></a>IsOwner

**L’élément IsOwner** spécifie si l’utilisateur de messagerie spécifié en est le propriétaire. 
  
```XML
<IsOwner>true | false</IsOwner>
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
|[RightsManagementLicenseData](rightsmanagementlicensedata.md) <br/> |Spécifie des informations sur la licence de gestion des droits.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** l’élément **IsOwner** indique que l’utilisateur est le propriétaire des droits émis sur un élément. La valeur **false indique** que l’utilisateur n’est pas le propriétaire des droits émis sur un élément. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

