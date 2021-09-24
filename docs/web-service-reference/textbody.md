---
title: TextBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bd0c0bce-3e7c-47c7-af7f-5ee5f5ad9820
description: L’élément TextBody spécifie le corps du texte.
ms.openlocfilehash: 5dfc0aa76f0b0778d785e46fe12259c4a226b89f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515179"
---
# <a name="textbody"></a>TextBody

**L’élément TextBody** spécifie le corps du texte. 
  
```XML
<TextBody BodyTypeType=" HTML | Text" IsTruncated=" true | false"></TextBody>
```

 **BodyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|BodyTypeType  <br/> |Indique le type de corps. La valeur de **Text pour** **l’attribut BodyTypeType** indique que le corps est en texte simple. La valeur html **de** **l’attribut BodyTypeType** indique que le corps est au format HTML. **L’attribut BodyTypeType** est obligatoire.  <br/> |
|IsTruncated  <br/> |Indique que le contenu du corps a été tronqué. Une valeur de texte **false** pour l’attribut **IsTruncated** indique que le contenu du corps n’a pas été tronqué. Le corps normalisé est tronqué si la longueur du corps du texte est plus longue que la valeur définie dans l’élément [MaximumBodySize.](maximumbodysize.md)  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Élément](item.md)  |  [Contact](contact.md)  |  [Message](message-ex15websvcsotherref.md)  |  [DistributionList](distributionlist.md)  |  [CalendarItem](calendaritem.md)  |  [PostItem](postitem.md)  |  [Tâche](task.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément TextBody** est le corps du texte de l’élément. 
  
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
   

