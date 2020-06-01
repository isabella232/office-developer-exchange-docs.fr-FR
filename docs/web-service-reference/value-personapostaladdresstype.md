---
title: Valeur (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: L’élément Value spécifie les informations associées à une adresse postale.
ms.openlocfilehash: 2d644ff45fe89061ccd90279773f3a5a5b7fe7cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466471"
---
# <a name="value-personapostaladdresstype"></a>Valeur (PersonaPostalAddressType)

L’élément **value** spécifie les informations associées à une adresse postale. 
  
```XML
<Value>
   <Street/>
   <City/>
   <State/>
   <Country/>
   <PostalCode/>
   <PostOfficeBox/>
   <Type/>
   <Latitude/>
   <Longitude/>
   <Accuracy/>
   <Altitude/>
   <AltitudeAccuracy/>
   <FormattedAddress/>
   <LocationUri/>
   <LocationSource/>
</Value>
```

**PersonaPostalAddressType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Rue](street.md)  |  [Ville](city.md)  |  [État](state-ex15websvcsotherref.md)  |  [Pays](country.md)  |  [CodePostal](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Type (chaîne)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Précision](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [LocationSource](locationsource.md)
  
### <a name="parent-elements"></a>Éléments parents

[PostalAddressAttributedValue](postaladdressattributedvalue.md)
  
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
   

