---
title: Ispermanentfailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: L’élément IsPermanentFailure indique si une tentative précédente d’indexer l’élément a échoué.
ms.openlocfilehash: e5ed20de3c3de9c39d1487e3177c1b6ec358d990
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532719"
---
# <a name="ispermanentfailure"></a>Ispermanentfailure

**L’élément IsPermanentFailure** indique si une tentative précédente d’indexer l’élément a échoué. 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **IsPermanentFailure** indique qu’une tentative précédente d’indexation de l’élément de boîte aux lettres a échoué. La valeur **false indique** qu’une tentative précédente d’indexation de l’élément de boîte aux lettres a réussi. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

