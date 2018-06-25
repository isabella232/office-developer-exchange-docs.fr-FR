---
title: InPlaceHoldConfigurationOnly
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 921ecc73-b7e2-40a7-8458-68f18dd5a13b
description: L’élément InPlaceHoldConfigurationOnly Spécifie si pour inclure le blocage sur place configuration.
ms.openlocfilehash: 3ad020a10e43d8f54e3d603906c856e01b1956eb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827934"
---
# <a name="inplaceholdconfigurationonly"></a>InPlaceHoldConfigurationOnly

L’élément **InPlaceHoldConfigurationOnly** Spécifie si pour inclure le blocage sur place configuration. 
  
```XML
<InPlaceHoldConfigurationOnly>true | false</InPlaceHoldConfigurationOnly>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de **la valeur true** pour l’élément **InPlaceHoldConfigurationOnly** indique que la configuration dans une archive permanente est incluse. La valeur **false** indique que la configuration dans une archive permanente n’est pas incluse. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

