---
title: ConvertHtmlCodePageToUTF8
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f02c8331-0a4e-4d01-adc2-2b93ed838a42
description: L’élément ConvertHtmlCodePageToUTF8 indique si le corps HTML de l’élément est converti en UTF8.
ms.openlocfilehash: e43de22b6d8050c14eb18d0fdd5a72f463335189
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545572"
---
# <a name="converthtmlcodepagetoutf8"></a>ConvertHtmlCodePageToUTF8

**L’élément ConvertHtmlCodePageToUTF8** indique si le corps HTML de l’élément est converti en UTF8. 
  
```XML
<ConvertHtmlCodePageToUTF8/>
```

 **xs:boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie un ensemble de propriétés à renvoyer dans une réponse.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de **texte true** pour l’élément **ConvertHtmlCodePageToUTF8** indique que le corps HTML est converti en UTF8. Une valeur de texte **false** indique que le corps HTML n’est pas converti en UTF8. 
  
## <a name="remarks"></a>Remarques

La valeur par défaut **true** est utilisée si **l’élément ConvertHtmlCodePageToUTF8** n’est pas spécifié dans une requête. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

