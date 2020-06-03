---
title: UniqueBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8f7276aa-e354-40e4-b9cb-950fad46ac93
description: L’élément UniqueBodyType spécifie si le corps unique est renvoyé au format texte ou HTML.
ms.openlocfilehash: 7e6c4631ef589555ce4d5da747c200ffe956f3a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459439"
---
# <a name="uniquebodytype"></a>UniqueBodyType

L’élément **UniqueBodyType** spécifie si le corps unique est renvoyé au format texte ou html. 
  
```XML
<UniqueBodyType> Best | HTML | Text </UniqueBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **UniqueBodyType** indique le format dans lequel le corps unique est renvoyé. Le tableau suivant répertorie les valeurs possibles pour cet élément. 
  
****

|**Valeur**|**Description**|
|:-----|:-----|
|Idéale  <br/> |La réponse renverra le contenu disponible le plus riche du corps de texte. Ceci est utile s’il n’est pas connu si le contenu est du texte ou du code HTML.  <br/> Le corps renvoyé sera du texte si le corps stocké est en texte brut. Dans le cas contraire, la réponse renvoie HTML si le corps stocké est au format HTML ou RTF.  <br/> Il s’agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse renverra un corps unique au format HTML.  <br/> |
|Texte  <br/> |La réponse renverra un corps unique en tant que texte brut.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ItemShape](itemshape.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

