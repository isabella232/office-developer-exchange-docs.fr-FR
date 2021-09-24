---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: L’élément ForwardAllowed spécifie si le forwarding e-mails est activé.
ms.openlocfilehash: 8c9b2319ed6b3665e5d59d9f07b93fb78043042c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528664"
---
# <a name="forwardallowed"></a>ForwardAllowed

**L’élément ForwardAllowed** spécifie si le forwarding e-mails est activé. 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
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

Une valeur de texte **true pour** **l’élément ForwardAllowed** indique que le forwarding e-mails est autorisé. La valeur **false indique** que le forwarding n’est pas autorisé. 
  
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

