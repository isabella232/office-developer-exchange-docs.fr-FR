---
title: WithinDateRange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- WithinDateRange
api_type:
- schema
ms.assetid: 226aeb15-016f-45ca-992a-c137ba09ca08
description: L’élément WithinDateRange spécifie la plage de dates dans laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.
ms.openlocfilehash: 15f370746b375b4f2b59ca351b3bd3c8defdd947
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538463"
---
# <a name="withindaterange"></a>WithinDateRange

**L’élément WithinDateRange** spécifie la plage de dates dans laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique. 
  
```XML
<WithinDateRange>
     <StartDateTime/>
     <EndDateTime/>
</WithinDateRange>
```

 **RulePredicateDateRangeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartDateTime](startdatetime.md) <br/> |Spécifie la période de règle et indique que la condition de règle est remplie après cette valeur.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Spécifie la période de règle et indique que la condition de règle est remplie avant cette valeur.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Conditions](conditions.md) <br/> |Représente les conditions qui, lorsqu'elles sont remplies, vont déclencher les actions de règle pour une règle.  <br/> |
|[Exceptions](exceptions.md) <br/> |Représente toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

