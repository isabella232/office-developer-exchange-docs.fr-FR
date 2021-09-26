---
title: IncludePersonalArchive
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b373bb1a-6b1d-4959-98a1-4c4ea62973bc
description: L’élément IncludePersonalArchive spécifie s’il faut inclure l’archive personnelle dans la recherche.
ms.openlocfilehash: 2567475fbb2542c7d01e651f2d348f6f91d50b78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547217"
---
# <a name="includepersonalarchive"></a>IncludePersonalArchive

**L’élément IncludePersonalArchive** spécifie s’il faut inclure l’archive personnelle dans la recherche. 
  
```XML
<IncludePersonalArchive>true | false</IncludePersonalArchive>
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
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |Spécifie une demande de recherche de statistiques de boîte aux lettres par mot clé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true pour** l’élément **IncludePersonalArchive** indique que l’archive personnelle est incluse dans la recherche. La valeur **false indique** que l’archive personnelle n’est pas incluse dans la recherche. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

