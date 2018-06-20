---
title: NormalizedBodyType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c6973aee-ec7b-44c1-b328-f2204d9de5d1
description: L’élément NormalizedBodyType Spécifie si le corps normalisé est retourné dans le format HTML ou texte.
ms.openlocfilehash: 33575594b22f972a9eb762dfac884fa91459f04a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828554"
---
# <a name="normalizedbodytype"></a>NormalizedBodyType

L’élément **NormalizedBodyType** Spécifie si le corps normalisé est retourné dans le format HTML ou texte. 
  
```XML
<NormalizedBodyType> Best | HTML | Text </NormalizedBodyType>
```

 **BodyTypeResponseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ItemShape](itemshape.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **NormalizedBodyType** indique le format du corps normalisé est renvoyée dans. Le tableau suivant répertorie les valeurs possibles de cet élément. 
  
****

|**Valeur**|**Description**|
|:-----|:-----|
|Recommandé  <br/> |La réponse renvoie le contenu disponible plus riche du corps de texte. Cela est utile si elle est inconnue ou non le contenu est texte ou HTML.  <br/> Le corps retourné sera texte si le corps stocké est en texte brut. Dans le cas contraire, la réponse renverra HTML si le corps stocké est au format HTML ou RTF.  <br/> Il s'agit de la valeur par défaut.  <br/> |
|HTML  <br/> |La réponse renvoie un corps normalisé au format HTML.  <br/> |
|Texte  <br/> |La réponse renvoie un corps normalisé sous forme de texte brut.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ItemShape](itemshape.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

