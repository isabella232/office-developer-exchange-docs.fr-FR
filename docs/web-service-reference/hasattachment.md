---
title: HasAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: de152be6-fc2f-48bc-a05d-1211935da20a
description: L’élément HasAttachment spécifie une valeur de type Boolean pour indiquer si l’élément comporte des pièces jointes.
ms.openlocfilehash: c6bc0932a08a1bbec215bb8a974ed746d2961123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530260"
---
# <a name="hasattachment"></a>HasAttachment

L’élément **HasAttachment** spécifie une valeur de type Boolean pour indiquer si l’élément comporte des pièces jointes. 
  
```XML
<HasAttachment> true | false </HasAttachment
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
|[SearchPreviewItem](searchpreviewitem.md) <br/> |Spécifie les 256 premiers caractères d’un élément de boîte aux lettres pour l’aperçu sans ouvrir l’élément.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **HasAttachment** indique que l’élément a une pièce jointe. La valeur **false** indique que l’élément n’a pas de pièce jointe. 
  
## <a name="remarks"></a>Remarques

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

