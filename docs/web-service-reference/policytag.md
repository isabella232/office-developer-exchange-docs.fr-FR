---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: L’élément PolicyTag spécifie l’identificateur de rétention d’un élément ou d’un dossier.
ms.openlocfilehash: ddc4d890d1e514586ba5ea7f6a8b541b2e4786c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460896"
---
# <a name="policytag"></a>PolicyTag

L’élément **PolicyTag** spécifie l’identificateur de rétention d’un élément ou d’un dossier. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsExplicit  <br/> |Indique si une balise de stratégie a été définie explicitement sur un élément ou un dossier.  <br/> Une valeur de texte de **true** pour l’attribut **IsExplicit** indique que la balise de stratégie a été explicitement définie sur l’élément ou le dossier. Une valeur de type **false** indique que la balise de stratégie a été définie de manière implicite sur l’élément ou le dossier en fonction de la balise de stratégie de dossier parent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchPreviewItem](searchpreviewitem.md)  |  [Élément](item.md)  |  [Contact](contact.md)  |  [Message](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **PolicyTag** est l’identificateur de la balise de stratégie. L’identificateur de la balise de stratégie est un GUID. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

