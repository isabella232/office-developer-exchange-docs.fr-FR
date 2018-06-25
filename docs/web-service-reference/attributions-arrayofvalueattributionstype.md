---
title: Attributions (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: L’élément Attributions spécifie un tableau des affectations pour sa valeur de l’élément associé.
ms.openlocfilehash: a64510cacb9923682418ca8a9b203c765a129bdd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755355"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Attributions (ArrayOfValueAttributionsType)

L’élément **Attributions** spécifie un tableau des affectations pour sa **valeur** de l’élément associé. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Attribution (chaîne)](attribution-string.md) <br/> |Spécifie une chaîne utilisée pour identifier un attribut.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Spécifie le contenu du corps d’un élément.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Spécifie les propriétés étendues pour un personnage.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Spécifie une instance d’un tableau de numéros de téléphone et leurs attributions associées.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Spécifie une instance d’un tableau de données de chaîne d’un élément personnage.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’attributs associés à un élément personnage.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

