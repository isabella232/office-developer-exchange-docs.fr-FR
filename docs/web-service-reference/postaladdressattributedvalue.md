---
title: PostalAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f92aa41-1499-4d96-a973-24529ec64d24
description: L’élément PostalAddressAttributedValue spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.
ms.openlocfilehash: f2b8b9818e39780b934522910d016875dbe5af2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828854"
---
# <a name="postaladdressattributedvalue"></a>PostalAddressAttributedValue

L’élément **PostalAddressAttributedValue** spécifie une instance d’un tableau d’adresses postales et leurs attributions associées. 
  
```XML
<PostalAddressAttributedValue>
   <Value/>
   <Attributions/>
</PostalAddressAttributedValue>
```

 **PostalAddressAttributedValueType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
  
### <a name="parent-elements"></a>Éléments parents

[BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

