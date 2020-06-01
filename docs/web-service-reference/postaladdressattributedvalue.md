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
ms.openlocfilehash: bf5becca8ee0f143728010c5d0b1ed5a380838ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465379"
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)
  
### <a name="parent-elements"></a>Éléments parents

[BusinessAddresses](businessaddresses.md)  |  [HomeAddresses](homeaddresses.md)  |  [OtherAddresses](otheraddresses.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

