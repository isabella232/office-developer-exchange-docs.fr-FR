---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: L’élément TextBody Spécifie le corps du texte.
ms.openlocfilehash: 78b18b27891d571605d2eeeeffb5c252cc790c11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838688"
---
# <a name="textbody"></a>TextBody

L’élément **TextBody** Spécifie le corps du texte. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BodyTypeType  <br/> |Indique le type de corps. La valeur de **texte** pour l’attribut **BodyTypeType** indique que le corps est au format texte brut. La valeur de **code HTML** pour l’attribut **BodyTypeType** indique que le corps est au format HTML. L’attribut **BodyTypeType** est requis.  <br/> |
|IsTruncated  <br/> |Indique que le contenu du corps a été tronqué. Texte la valeur **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué. Si la longueur du corps du texte est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) le corps normalisé sera tronqué.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Élément](item.md) | [Contact](contact.md) | [Message](message-ex15websvcsotherref.md) | [DistributionList](distributionlist.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tâche](task.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **TextBody** est le corps du texte de l’élément. 
  
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
   

