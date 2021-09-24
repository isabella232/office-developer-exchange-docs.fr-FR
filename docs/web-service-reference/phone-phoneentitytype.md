---
title: Phone (PhoneEntityType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f6925cc9-7f22-478f-b9ba-b77575772471
description: L Téléphone spécifie un numéro de téléphone unique qui résulte de l’extraction d’une entité de numéro de téléphone.
ms.openlocfilehash: a8f0404c2cb9f141bf818dfe2fd07d3f4b1dacb8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528475"
---
# <a name="phone-phoneentitytype"></a>Phone (PhoneEntityType)

**L Téléphone** spécifie un numéro de téléphone unique qui résulte de l’extraction d’une entité de numéro de téléphone. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Position](position.md)  |  [OriginalPhoneString](originalphonestring.md)  |  [PhoneString](phonestring.md)  |  [Type (chaîne)](type-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md)
  
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
   

