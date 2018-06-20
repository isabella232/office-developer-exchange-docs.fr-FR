---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: L’élément LocationSource spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.
ms.openlocfilehash: 7f5cf5fcca0a72287593349fcf5090a74225d012
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828248"
---
# <a name="locationsource"></a>LocationSource

L’élément **LocationSource** spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique. 
  
```XML
<LocationSource> None | LocationServices | PhonebookServices | Device | Contact | Resource </LocationSource>
```

 **LocationSourceType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Valeur (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Valeur de texte

Les valeurs de texte de l’élément **LocationSource** sont répertoriées dans le tableau suivant : 
  
**Valeurs de texte des éléments LocationSource**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Il n’existe aucune source d’emplacement.  <br/> |
|LocationServices  <br/> |Les informations a été obtenues à partir des services de localisation.  <br/> |
|PhonebookServices  <br/> |Les informations ont été obtenues à partir des services d’annuaire.  <br/> |
|Appareil  <br/> |Les informations a été obtenues à partir du périphérique.  <br/> |
|Contact  <br/> |Les informations ont été obtenues à partir d’un contact.  <br/> |
|Ressource  <br/> |Les informations ont été obtenues à partir d’une ressource.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

