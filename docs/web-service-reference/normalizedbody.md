---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: L’élément NormalizedBody spécifie une représentation HTML de la propriété Body d’un élément en tant que fragment qui peut être inséré dans un autre corps HTML.
ms.openlocfilehash: 07c2176d2c8a7473c06b7e42f8bcbbe6670581ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828548"
---
# <a name="normalizedbody"></a>NormalizedBody

L’élément **NormalizedBody** spécifie une représentation HTML de la propriété **Body** d’un élément en tant que fragment qui peut être inséré dans un autre corps HTML. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BodyType  <br/> |Indique le type de corps. La valeur de **texte** pour l’attribut **BodyType** indique que le corps est au format texte brut. La valeur de **code HTML** pour l’attribut **BodyType** indique que le corps est au format HTML. L’attribut **BodyType** est requis.  <br/> |
|IsTruncated  <br/> |Indique que le contenu du corps a été tronqué. Texte la valeur **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué. Si la longueur de corps normalisée est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) le corps normalisé sera tronqué.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Élément](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [tâche](task.md) | [PostItem ](postitem.md)  |  [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **NormalizedBody** est le corps de l’élément normalisé. 
  
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
   

