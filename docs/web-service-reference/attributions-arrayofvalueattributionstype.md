---
title: Attributions (ArrayOfValueAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 7f36b6ee-8ecf-48c9-8cb6-dfb2da0ce2a2
description: L’élément Attributions spécifie un tableau d’attributions pour son élément Value associé.
ms.openlocfilehash: e5483e8e7ef4745e8025106ae1f1c52e91987183
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529327"
---
# <a name="attributions-arrayofvalueattributionstype"></a>Attributions (ArrayOfValueAttributionsType)

**L’élément Attributions** spécifie un tableau d’attributions pour son élément **Value** associé. 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attribution>
```

 **ArrayOfValueAttributionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Attribution (String)](attribution-string.md) <br/> |Spécifie une chaîne utilisée pour identifier un attribut.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[BodyContentAttributedValue](bodycontentattributedvalue.md) <br/> |Spécifie le contenu du corps d’un élément.  <br/> |
|[EmailAddressAttributedValue](emailaddressattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’adresses de messagerie et leurs attributions associées.  <br/> |
|[ExtendedPropertyAttributedValue](extendedpropertyattributedvalue.md) <br/> |Spécifie les propriétés étendues d’un personnage.  <br/> |
|[PhoneNumberAttributedValue](phonenumberattributedvalue.md) <br/> |Spécifie une instance d’un tableau de numéros de téléphone et leurs attributions associées.  <br/> |
|[PostalAddressAttributedValue](postaladdressattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’adresses postales et leurs attributions associées.  <br/> |
|[StringArrayAttributedValue](stringarrayattributedvalue.md) <br/> |Spécifie une instance d’un tableau de données de chaîne pour un élément persona.  <br/> |
|[StringAttributedValue](stringattributedvalue.md) <br/> |Spécifie une instance dans un tableau d’attributs associés à un élément persona.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

