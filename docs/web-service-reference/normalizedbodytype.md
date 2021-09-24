---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: L’élément NormalizedBodyType spécifie si le corps normalisé est renvoyé au format texte ou HTML.
ms.openlocfilehash: 69ce440e30d921b052782af60057fff2d9e9d68f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59537565"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

**L’élément NormalizedBodyType spécifie** si le corps normalisé est renvoyé au format texte ou HTML. 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
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

La valeur de texte de **l’élément NormalizedBodyType** indique le format dans le corps normalisé est renvoyé. Le tableau suivant répertorie les valeurs possibles pour cet élément. 
  
****

|**Valeur**|**Description**|
|:-----|:-----|
|Idéale  <br/> |La réponse retourne le contenu disponible le plus riche du corps de texte. Cela est utile s’il est inconnu si le contenu est du texte ou du code HTML.  <br/> Le corps renvoyé sera du texte si le corps stocké est en texte simple. Sinon, la réponse retourne du code HTML si le corps stocké est au format HTML ou RTF.  <br/> Il s’agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse retourne un corps normalisé au format HTML.  <br/> |
|Texte  <br/> |La réponse retourne un corps normal sous forme de texte simple.  <br/> |
   
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

