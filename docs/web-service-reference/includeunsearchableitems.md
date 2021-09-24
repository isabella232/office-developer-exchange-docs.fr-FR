---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: L’élément IncludeUnsearchableItems spécifie s’il faut inclure les éléments qui ne peuvent pas faire l’objet d’une recherche.
ms.openlocfilehash: 3bffd68c20623aa4c63dd295d8b4619999c1d4a5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533103"
---
# <a name="includeunsearchableitems"></a>IncludeUnsearchableItems

**L’élément IncludeUnsearchableItems** spécifie s’il faut inclure les éléments qui ne peuvent pas faire l’objet d’une recherche. 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
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

Une valeur de texte **true** pour l’élément **IncludeUnsearchableItems** indique que les statistiques ne sont pas incluses pour les éléments qui ne peuvent pas faire l’objet d’une recherche. La valeur **false indique** que des statistiques sont incluses pour les éléments qui ne peuvent pas faire l’objet d’une recherche. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
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

