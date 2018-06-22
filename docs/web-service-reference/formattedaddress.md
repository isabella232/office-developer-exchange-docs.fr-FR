---
title: FormattedAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643f8663-1fab-4625-a7e9-5724e352972b
description: L’élément FormattedAddress spécifie la valeur d’affichage mise en forme de l’adresse postale associée.
ms.openlocfilehash: 14c970fcbe20567546e99e637c9c78c6003d9c0f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756465"
---
# <a name="formattedaddress"></a>FormattedAddress

L’élément **FormattedAddress** spécifie la valeur d’affichage mise en forme de l’adresse postale associée. 
  
```XML
<FormattedAddress></FormattedAddress>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md) <br/> |Spécifie les informations associées à une adresse postale.  <br/> |
|[PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md) <br/> |Spécifie l’adresse postale de l’emplacement.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **FormattedAddress** est une valeur de type string qui spécifie l’adresse mise en forme. 
  
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

