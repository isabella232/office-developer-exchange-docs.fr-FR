---
title: Point de terminaison (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 630cdbb5-d1c7-422c-924a-abf5738e9e5e
description: L’élément de point de terminaison Spécifie le point de terminaison de service d’émission de jeton de sécurité.
ms.openlocfilehash: 85e1ad785b35649238ac3944f51472addf617c20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756179"
---
# <a name="endpoint-soap"></a>Point de terminaison (SOAP)

L’élément de **point de terminaison** Spécifie le point de terminaison de service d’émission de jeton de sécurité. 
  
```XML
<Endpoint/>
```

 **xs : anyURI**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun
  
### <a name="child-elements"></a>Éléments enfants

Aucun
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[TokenIssuer (SOAP)](tokenissuer-soap.md) <br/> |Spécifie l’URI et le point de terminaison pour le service d’émission de jeton de sécurité.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le point de terminaison pour le service web d’émission de jeton de sécurité.
  
## <a name="remarks"></a>Remarques

Le point de terminaison est utilisé pour communiquer avec le service web d’émission de jeton de sécurité.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

