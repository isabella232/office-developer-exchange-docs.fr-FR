---
title: IncludeUnsearchableItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9a9bd2dc-f5b9-4b82-a6a0-f643d2951080
description: L’élément IncludeUnsearchableItems Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés.
ms.openlocfilehash: 4c6b9b3752330bf914c9901d2e8f69e93546fec6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827907"
---
# <a name="includeunsearchableitems"></a>IncludeUnsearchableItems

L’élément **IncludeUnsearchableItems** Spécifie s’il faut inclure des éléments qui ne peuvent pas être recherchés. 
  
```XML
<IncludeUnsearchableItems>true | false</IncludeUnsearchableItems>
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
|[FindMailboxStatisticsByKeywords](findmailboxstatisticsbykeywords.md) <br/> |Spécifie une requête pour rechercher des statistiques de boîtes aux lettres par mot clé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **IncludeUnsearchableItems** indique que les statistiques ne sont pas inclus pour les éléments qui ne sont pas utilisables dans une requête. La valeur **false** indique que les statistiques sont inclus pour les éléments qui ne sont pas utilisables dans une requête. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

