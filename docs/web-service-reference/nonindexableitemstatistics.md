---
title: NonIndexableItemStatistics
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 12f2934a-008c-4236-b8b3-7c7b6b5707e2
description: L’élément NonIndexableItemStatistics contient un tableau de statistiques pour les éléments qui n’ont pas pu être indexés.
ms.openlocfilehash: 29551d5f7f9b4cbdd54a1ee26920eff4fcb11f25
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541965"
---
# <a name="nonindexableitemstatistics"></a>NonIndexableItemStatistics

**L’élément NonIndexableItemStatistics** contient un tableau de statistiques pour les éléments qui n’ont pas pu être indexés. 
  
```XML
<NonIndexableItemStatistics>
   <NonIndexableItemStatistic/>
</NonIndexableItemStatistics>
```

 **ArrayOfNonIndexableItemStatisticsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[NonIndexableItemStatistic](nonindexableitemstatistic.md)
  
### <a name="parent-elements"></a>Éléments parents

[GetNonIndexableItemStatisticsResponse](getnonindexableitemstatisticsresponse.md) , [GetNonIndexableItemStatisticsResponseMessage](getnonindexableitemstatisticsresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

