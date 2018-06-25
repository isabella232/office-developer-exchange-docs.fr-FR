---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: L’élément ConvertHtmlCodePageToUTF8 indique si l’élément corps HTML est converti en UTF-8.
ms.openlocfilehash: aff6579835097a273101188c02a9919003b71b58
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755657"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

L’élément **ConvertHtmlCodePageToUTF8** indique si l’élément corps HTML est converti en UTF-8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs : Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie un ensemble de propriétés à retourner dans une réponse.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **ConvertHtmlCodePageToUTF8** indique que le corps HTML est converti en UTF-8. Texte la valeur **false** indique que le corps HTML n’est pas converti en UTF-8. 
  
## <a name="remarks"></a>Remarques

La valeur par défaut **true** est utilisée si l’élément **ConvertHtmlCodePageToUTF8** n’est pas spécifié dans une requête. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

