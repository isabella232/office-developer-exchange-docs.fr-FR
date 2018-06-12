---
title: IsPermanentFailure
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 18dc3a97-cc0a-4092-934e-a6e86f52e668
description: L’élément IsPermanentFailure indique si une tentative précédente d’index de l’élément a échoué.
ms.openlocfilehash: 39592c15394a57e1c6aa1183ed0ccedeb085e6ea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828085"
---
# <a name="ispermanentfailure"></a>IsPermanentFailure

L’élément **IsPermanentFailure** indique si une tentative précédente d’index de l’élément a échoué. 
  
```XML
<IsPermanentFailure>true | false</IsPermanentFailure>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **IsPermanentFailure** indique qu’une tentative précédente d’index de l’élément de boîte aux lettres a échoué. La valeur **false** indique qu’une tentative précédente d’index de l’élément de boîte aux lettres a réussi. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

