---
title: PolicyTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa4b1447-dc7b-47ad-a677-78fcee443dc6
description: L’élément PolicyTag spécifie l’identificateur de rétention sur un élément ou un dossier.
ms.openlocfilehash: 16759748dded6978e68450a6b8d504dd378c04be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519253"
---
# <a name="policytag"></a>PolicyTag

**L’élément PolicyTag** spécifie l’identificateur de rétention sur un élément ou un dossier. 
  
```xml
<PolicyTag IsExplicit="true | false"></PolicyTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsExplicit  <br/> |Indique si une balise de stratégie a été explicitement définie sur un élément ou un dossier.  <br/> Une valeur de texte **true** pour l’attribut **IsExplicit** indique que la balise de stratégie a été explicitement définie sur l’élément ou le dossier. Une valeur de texte **false** indique que la balise de stratégie a été implicitement définie sur l’élément ou le dossier en fonction de la balise de stratégie de dossier parent.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SearchPreviewItem](searchpreviewitem.md)  |  [Élément](item.md)  |  [Contact](contact.md)  |  [Message](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément PolicyTag** est l’identificateur de balise de stratégie. L’identificateur de balise de stratégie est un GUID. 
  
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
   

