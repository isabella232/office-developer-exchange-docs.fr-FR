---
title: Téléphone (PhoneEntityType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6925cc9-7f22-478f-b9ba-b77575772471
description: L’élément téléphone spécifie un numéro de téléphone unique qui résulte d’une extraction d’entité numérique de téléphone.
ms.openlocfilehash: 654e8fc378ce3483cb3ebd9be33f3737ddd86bcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828754"
---
# <a name="phone-phoneentitytype"></a>Téléphone (PhoneEntityType)

L’élément **téléphone** spécifie un numéro de téléphone unique qui résulte d’une extraction d’entité numérique de téléphone. 
  
```XML
<Phone>
   <Position/>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 **PhoneEntityType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Position](position.md) | [OriginalPhoneString](originalphonestring.md) | [PhoneString](phonestring.md) | [Type (chaîne)](type-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md)
  
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
   

