---
title: LocationSource
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fc4d77d5-6200-4cf3-848a-1088fec0e0d6
description: L’élément LocationSource spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique.
ms.openlocfilehash: f3569494d3e662fbc46060944c8bd399b62d656b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543260"
---
# <a name="locationsource"></a>LocationSource

**L’élément LocationSource** spécifie des informations sur l’origine de l’adresse postale associée, par exemple, un contact ou un annuaire téléphonique. 
  
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

[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  |  [PostalAddress (PersonaPostalAddressType)](postaladdress-personapostaladdresstype.md)
  
## <a name="text-value"></a>Valeur texte

Les valeurs de texte de **l’élément LocationSource** sont répertoriées dans le tableau suivant : 
  
**Valeurs de texte de l’élément LocationSource**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Il n’existe aucune source d’emplacement.  <br/> |
|LocationServices  <br/> |Les informations ont été obtenues à partir des services de localisation.  <br/> |
|PhonebookServices  <br/> |Les informations ont été obtenues à partir des services de phonébook.  <br/> |
|Appareil  <br/> |Les informations ont été obtenues à partir de l’appareil.  <br/> |
|Contact  <br/> |Les informations ont été obtenues auprès d’un contact.  <br/> |
|Ressource  <br/> |Les informations ont été obtenues à partir d’une ressource.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  

