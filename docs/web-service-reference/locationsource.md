---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: L’élément LocationSource spécifie les informations relatives à l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.
ms.openlocfilehash: ceba52c43d1c798bb8f5492b779c7c45d7d00b0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467101"
---
# <a name="locationsource"></a>LocationSource

L’élément **LocationSource** spécifie les informations relatives à l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Valeur texte

Les valeurs de texte de l’élément **LocationSource** sont répertoriées dans le tableau suivant : 
  
**Valeurs de texte de l’élément LocationSource**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Il n’y a pas de source d’emplacement.  <br/> |
|LocationServices  <br/> |Les informations proviennent des services de localisation.  <br/> |
|PhonebookServices  <br/> |Les informations proviennent des services d’annuaire.  <br/> |
|Device  <br/> |Les informations ont été obtenues à partir de l’appareil.  <br/> |
|Contact  <br/> |Les informations ont été obtenues à partir d’un contact.  <br/> |
|Resource  <br/> |Les informations ont été obtenues à partir d’une ressource.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

