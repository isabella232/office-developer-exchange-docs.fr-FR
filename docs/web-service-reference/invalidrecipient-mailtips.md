---
title: InvalidRecipient (infos-courrier)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InvalidRecipient
api_type:
- schema
ms.assetid: 48959a99-bb0d-4004-963e-5a5baaa96476
description: L’élément InvalidRecipient indique si le destinataire n’est pas valide.
ms.openlocfilehash: fddd75beb2228c50084bd38b4f4745064cc281dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530001"
---
# <a name="invalidrecipient-mailtips"></a>InvalidRecipient (infos-courrier)

L’élément **InvalidRecipient** indique si le destinataire n’est pas valide. 
  
```XML
<InvalidRecipient>true | false</InvalidRecipient>
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
|[Infos-courrier](mailtips.md) <br/> |Représente les valeurs de différents types de conseils de courrier.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est **true** si le destinataire n’est pas valide. La valeur est **false** si le destinataire n’est pas valide. 
  
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

