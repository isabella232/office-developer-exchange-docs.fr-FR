---
title: Adresses (ArrayOfAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e
description: L’élément addresses spécifie un tableau d’éléments AddressEntity.
ms.openlocfilehash: 48cf8c0fda6a8ef894ef8d3a4c154f7255b218bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463628"
---
# <a name="addresses-arrayofaddressentitiestype"></a>Adresses (ArrayOfAddressEntitiesType)

L’élément **Addresses** spécifie un tableau d’éléments **AddressEntity** . 
  
```XML
<Addresses>
   <AddressEntity/>
</Addresses>
```

 **ArrayOfAddressEntitiesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AddressEntity](addressentity.md) <br/> |Spécifie une entité d’adresse unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[EntityExtractionResult](entityextractionresult.md) <br/> |Spécifie la propriété **EntityExtractionResult** d’un élément.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

