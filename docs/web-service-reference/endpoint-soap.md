---
title: Point de terminaison (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: L’élément Endpoint spécifie le point de terminaison du service d’émission de jeton de sécurité.
ms.openlocfilehash: 93659bbefa4a95063304cf3abad81cb61767070a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458396"
---
# <a name="endpoint-soap"></a>Point de terminaison (SOAP)

L’élément **Endpoint** spécifie le point de terminaison du service d’émission de jeton de sécurité. 
  
```XML
<Endpoint/>
```

 **XS : anyURI**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Spécifie l’URI et le point de terminaison pour le service d’émission de jeton de sécurité.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le point de terminaison pour le service Web de jeton de sécurité.
  
## <a name="remarks"></a>Remarques

Le point de terminaison est utilisé pour communiquer avec le service Web de jeton de sécurité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

