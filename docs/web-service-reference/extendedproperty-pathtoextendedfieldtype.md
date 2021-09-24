---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: L’élément ExtendedProperty spécifie une propriété étendue pour le magasin de contacts unifié.
ms.openlocfilehash: 5cb320e15d3a01c542907048357d1ef0cc78f96a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530758"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

**L’élément ExtendedProperty** spécifie une propriété étendue pour le magasin de contacts unifié. 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |Indique l’identificateur de jeu de propriétés unique. Cet attribut est facultatif.  <br/> |
|PropertySetId  <br/> |Indique l’identificateur de jeu de propriétés GUID. Cet attribut est facultatif.  <br/> |
|PropertyTag  <br/> | Représente la balise de propriété moins la partie de type.<br/><br/>Il existe deux options de représentation :  <br/><br/>- Hexadécimal : 0x3fa4  <br/>- Décimal : 0-65535<br/><br/>  Cet attribut est facultatif.  <br/> |
|PropertyName  <br/> |Chaîne qui indique le nom de la propriété. Cet attribut est facultatif.  <br/> |
|PropertyId  <br/> |Integer qui indique l’identificateur de propriété. Cet attribut est facultatif.  <br/> |
|PropertyType  <br/> |Indique le type de propriété. Cet attribut est obligatoire.  <br/> |
|FieldURI  <br/> |Indique le champ Uniform Resource Identifier (URI). Cet attribut est obligatoire. Pour les valeurs possibles, voir [l’élément FieldURI.](fielduri.md)  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Valeur**|**Description**|
|:-----|:-----|
|Réunion  <br/> |Indique une réunion.  <br/> |
|Rendez-vous  <br/> |Indique un rendez-vous.  <br/> |
|Courant  <br/> |Indique le jeu de propriétés commun.  <br/> |
|PublicStrings  <br/> |Indique des chaînes publiques.  <br/> |
|Adresse  <br/> |Indique une adresse.  <br/> |
|InternetHeaders  <br/> |Indique les en-têtes Internet.  <br/> |
|CalendarAssistant  <br/> |Indique l’Assistant Calendrier.  <br/> |
|UnifiedMessaging  <br/> |Indique la messagerie unifiée.  <br/> |
|Tâche  <br/> |Indique une tâche.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Valeur**|**Description**|
|:-----|:-----|
|ApplicationTime  <br/> |Indique l’heure de l’application.  <br/> |
|ApplicationTimeArray  <br/> |Indique un tableau des heures d’application.  <br/> |
|Binaire  <br/> |Indique une valeur binaire.  <br/> |
|BinaryArray  <br/> |Indique un tableau de valeurs binaires.  <br/> |
|Valeur booléenne  <br/> |Indique une valeur boolé américaine.  <br/> |
|CLSID  <br/> |Indique un CLSID.  <br/> |
|CLSIDArray  <br/> |Indique un tableau de CLSID.  <br/> |
|Devise  <br/> |Indique une valeur monétaire.  <br/> |
|CurrencyArray  <br/> |Indique un tableau de valeurs monétaires.  <br/> |
|Double  <br/> |Indique un **double**.  <br/> |
|DoubleArray  <br/> |Indique un tableau de **valeurs doubles.**  <br/> |
|Erreur  <br/> |Indique une erreur. Ceci est à des fins de rapport d’erreurs. Elle ne peut pas être utilisée dans des restrictions ou pour obtenir ou définir des valeurs.  <br/> |
|Flottant  <br/> |Indique un **flottant**.  <br/> |
|FloatArray  <br/> |Indique un tableau de valeurs **flottantes.**  <br/> |
|Entier  <br/> |Indique un integer.  <br/> |
|IntegerArray  <br/> |Indique un tableau d’nombres integers.  <br/> |
|Entier long  <br/> |Indique un **long**.  <br/> |
|LongArray  <br/> |Indique un tableau de valeurs **longues.**  <br/> |
|Null  <br/> |Indique une valeur null. Ceci est à des fins de rapport d’erreurs. Elle ne peut pas être utilisée dans des restrictions ou pour obtenir ou définir des valeurs.  <br/> |
|Objet  <br/> |Indique un objet. Ceci est à des fins de rapport d’erreurs. Elle ne peut pas être utilisée dans des restrictions ou pour obtenir ou définir des valeurs.  <br/> |
|ObjectArray  <br/> |Indique un tableau d’objets. Ceci est à des fins de rapport d’erreurs. Elle ne peut pas être utilisée dans des restrictions ou pour obtenir ou définir des valeurs.  <br/> |
|Nom court  <br/> |Indique un **court**.  <br/> |
|ShortArray  <br/> |Indique un tableau de valeurs **courtes.**  <br/> |
|SystemTime  <br/> |Indique une valeur d’heure système.  <br/> |
|SystemTimeArray  <br/> |Indique un tableau de valeurs d’heure système.  <br/> |
|Chaîne  <br/> |Indique une chaîne.  <br/> |
|StringArray  <br/> |Indique un tableau de chaînes.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Identifie une propriété MAPI étendue.  <br/> |
   
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

