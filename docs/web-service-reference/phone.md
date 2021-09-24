---
title: Téléphone
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9381d8e0-b705-49fd-a822-00fb485bdbab
description: L Téléphone spécifie un numéro de téléphone unique qui résulte de l’extraction d’une entité de contact.
ms.openlocfilehash: fa9e0be88c2142b30304c3c5b758624fa73da7d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528359"
---
# <a name="phone"></a>Téléphone

**L Téléphone** spécifie un numéro de téléphone unique qui résulte de l’extraction d’une entité de contact. 
  
```XML
<Phone>
   <OriginalPhoneString/>
   <PhoneString/>
   <Type/>
</Phone>
```

 **PhoneType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[OriginalPhoneString](originalphonestring.md)  |  [PhoneString](phonestring.md)  |  [Type (chaîne)](type-string.md)
  
### <a name="parent-elements"></a>Éléments parents

[PhoneNumbers (ArrayOfPhonesType)](phonenumbers-arrayofphonestype.md)
  
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
   

