---
title: Value (PersonaPostalAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: be838fc2-cfcb-4856-b095-a8e5366bb6c6
description: L’élément Value spécifie les informations associées à une adresse postale.
ms.openlocfilehash: 2f017cfc513b9c22d65f8437565646506f3be1ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517342"
---
# <a name="value-personapostaladdresstype"></a>Value (PersonaPostalAddressType)

**L’élément Value** spécifie les informations associées à une adresse postale. 
  
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

[Street](street.md)  |  [Ville](city.md)  |  [État](state-ex15websvcsotherref.md)  |  [Pays](country.md)  |  [PostalCode](postalcode.md)  |  [PostOfficeBox](postofficebox.md)  |  [Type (chaîne)](type-string.md)  |  [Latitude](latitude.md)  |  [Longitude](longitude.md)  |  [Précision](accuracy.md)  |  [Altitude](altitude.md)  |  [AltitudeAccuracy](altitudeaccuracy.md)  |  [FormattedAddress](formattedaddress.md)  |  [LocationUri](locationuri.md)  |  [LocationSource](locationsource.md)
  
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
   

