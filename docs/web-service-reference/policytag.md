---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: L’élément PolicyTag Spécifie l’identificateur de rétention sur un élément ou un dossier.
ms.openlocfilehash: d6cd5aab1145f6006912541c8f8c1d0a91d1e17e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828835"
---
# <a name="policytag"></a>PolicyTag

L’élément **PolicyTag** Spécifie l’identificateur de rétention sur un élément ou un dossier. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsExplicit  <br/> |Indique si une balise de stratégie a été explicitement définie sur un élément ou un dossier.  <br/> Une valeur de texte de **la valeur true** pour l’attribut **IsExplicit** indique que la balise de stratégie a été explicitement définie sur l’élément ou d’un dossier. Texte la valeur **false** indique que la balise de stratégie a été implicitement définie sur l’élément ou un dossier en fonction de la balise de stratégie de dossier parent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchPreviewItem](searchpreviewitem.md) | [élément](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tâche](task.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **PolicyTag** est l’identificateur de balise de stratégie. L’identificateur de balise de stratégie est un GUID. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

