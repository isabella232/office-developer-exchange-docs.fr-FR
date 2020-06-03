---
title: Corps
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: L’élément Body spécifie le corps d’un élément.
ms.openlocfilehash: c565c5701ae5bc210cf0a9dc694108752860e24b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529489"
---
# <a name="body"></a>Corps

L’élément **Body** spécifie le corps d’un élément. 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BodyType  <br/> |Spécifie le type du corps.  <br/> |
|IsTruncated  <br/> |Valeur booléenne qui indique si le corps est tronqué.  <br/> |
   
#### <a name="bodytype"></a>BodyType

|**Valeur**|**Description**|
|:-----|:-----|
|HTML  <br/> |Indique que le corps est au format HTML.  <br/> |
|Texte  <br/> |Indique que le corps est dans le texte.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Représente un élément de calendrier Exchange.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact dans la banque d'informations Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Élément](item.md) <br/> |Représente un élément générique dans la Banque d’Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Représente un élément post dans la Banque d’Exchange.  <br/> |
|[Tâche](task.md) <br/> |Représente une tâche dans la banque d'informations Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **Body** est le contenu du corps de l’élément. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

