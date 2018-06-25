---
title: AltitudeAccuracy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: aadc1f90-e9ab-4411-b51f-2d43e5e22f2a
description: L’élément AltitudeAccuracy spécifie la précision de la propriété altitude pour une adresse postale.
ms.openlocfilehash: 09ec86e4913327feb47067f5e5de7a60efc47bc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755197"
---
# <a name="altitudeaccuracy"></a>AltitudeAccuracy

L’élément **AltitudeAccuracy** spécifie la précision de la propriété altitude pour une adresse postale. 
  
```XML
<AltitudeAccuracy></AltitudeAccuracy>
```

 **xs : double**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |Spécifie l’adresse postale de l’emplacement.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **AltitudeAccuracy** est l’estimation de la précision de la propriété altitude d’une adresse postale. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

