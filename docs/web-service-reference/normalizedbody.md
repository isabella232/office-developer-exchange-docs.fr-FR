---
title: NormalizedBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfb813e4-642d-4f1b-9e91-1fee89dbd083
description: L’élément NormalizedBody spécifie une représentation HTML de la propriété Body d’un élément sous la forme d’un fragment qui peut être inséré dans un autre corps HTML.
ms.openlocfilehash: fb249794bccfeed198e7a3230ab53c66893dcf96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462667"
---
# <a name="normalizedbody"></a>NormalizedBody

L’élément **NormalizedBody** spécifie une représentation HTML de la propriété **Body** d’un élément sous la forme d’un fragment qui peut être inséré dans un autre corps HTML. 
  
```XML
<NormalizedBody BodyType="Text | HTML" IsTruncated="true | false"></NormalizedBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BodyType  <br/> |Indique le type de corps. La valeur de **Text** pour l’attribut **BodyType** indique que le corps est en texte brut. La valeur de **HTML** pour l’attribut **BodyType** indique que le corps est au format html. L’attribut **BodyType** est obligatoire.  <br/> |
|IsTruncated  <br/> |Indique que le contenu du corps a été tronqué. Une valeur de texte **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué. Le corps normalisé est tronqué si la longueur de corps normalisé est supérieure à la valeur définie dans l’élément [MaximumBodySize](maximumbodysize.md) .  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Élément](item.md)  |  [Message](message-ex15websvcsotherref.md)  |  [MeetingMessage](meetingmessage.md)  |  [Propriété meetingrequest](meetingrequest.md)  |  [MeetingResponse](meetingresponse.md)  |  [MeetingCancellation](meetingcancellation.md)  |  [Tâche](task.md)  |  [PostItem](postitem.md)  |  [CalendarItem](calendaritem.md)  |  [Contact](contact.md)  |  [DistributionList](distributionlist.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **NormalizedBody** est le corps normalisé de l’élément. 
  
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
   

