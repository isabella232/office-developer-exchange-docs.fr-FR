---
title: ExtendedProperty (PathToExtendedFieldType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fa620b48-2ce3-437d-b51e-541247eea1d9
description: L’élément ExtendedProperty spécifie une propriété étendue pour le magasin de contacts unifié.
ms.openlocfilehash: 7541fa6330ee96f7791febfabc672dbcf0e95b54
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756303"
---
# <a name="extendedproperty-pathtoextendedfieldtype"></a>ExtendedProperty (PathToExtendedFieldType)

L’élément **ExtendedProperty** spécifie une propriété étendue pour le magasin de contacts unifié. 
  
```xml
<ExtendedProperty DistinguishedPropertySetId="" PropertySetId="" PropertyTag="" PropertyName="" PropertyId="" PropertyType="" FieldURI="">
</ExtendedProperty>
```

**PathToExtendedFieldType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|DistinguishedPropertySetId  <br/> |Indique l’identificateur unique de propriété. Cet attribut est facultatif.  <br/> |
|PropertySetId  <br/> |Indique l’identificateur GUID propriété. Cet attribut est facultatif.  <br/> |
|PropertyTag  <br/> | Représente la balise de propriété moins le composant de type.<br/><br/>Il existe deux options pour la représentation sous forme de :  <br/><br/>-Hexadécimal : 0x3fa4  <br/>-Décimale : 0-65535<br/><br/>  Cet attribut est facultatif.  <br/> |
|PropertyName  <br/> |Chaîne qui indique le nom de propriété. Cet attribut est facultatif.  <br/> |
|PropertyId  <br/> |Entier qui indique l’identificateur de propriété. Cet attribut est facultatif.  <br/> |
|PropertyType  <br/> |Indique le type de propriété. Cet attribut est requis.  <br/> |
|FieldURI  <br/> |Indique le champ identificateur URI (Uniform Resource). Cet attribut est requis. Pour les valeurs possibles, voir l’élément [FieldURI](fielduri.md) .  <br/> |
   
#### <a name="distinguishedpropertysetid"></a>DistinguishedPropertySetId

|**Valeur**|**Description**|
|:-----|:-----|
|Réunion  <br/> |Indique une réunion.  <br/> |
|Rendez-vous  <br/> |Indique un rendez-vous.  <br/> |
|Common  <br/> |Indique le jeu de propriétés courantes.  <br/> |
|PublicStrings  <br/> |Indique les chaînes publics.  <br/> |
|Address  <br/> |Indique une adresse.  <br/> |
|InternetHeaders  <br/> |Indique les en-têtes Internet.  <br/> |
|CalendarAssistant  <br/> |Indique l’Assistant Calendrier.  <br/> |
|UnifiedMessaging  <br/> |Indique que la messagerie unifiée.  <br/> |
|Tâche  <br/> |Indique une tâche.  <br/> |
   
#### <a name="propertytype"></a>PropertyType

|**Valeur**|**Description**|
|:-----|:-----|
|ApplicationTime  <br/> |Indique l’heure de l’application.  <br/> |
|ApplicationTimeArray  <br/> |Indique un tableau de temps de l’application.  <br/> |
|Binaire  <br/> |Indique une valeur binaire.  <br/> |
|BinaryArray  <br/> |Indique un tableau de valeurs binaires.  <br/> |
|Bool�en  <br/> |Indique une valeur de type Boolean.  <br/> |
|CLSID  <br/> |Indique un CLSID.  <br/> |
|CLSIDArray  <br/> |Indique un tableau de CLSID.  <br/> |
|Monnaie  <br/> |Indique une valeur monétaire.  <br/> |
|CurrencyArray  <br/> |Indique un tableau de valeurs monétaires.  <br/> |
|Double  <br/> |Indique un **double**.  <br/> |
|DoubleArray  <br/> |Indique un tableau de valeurs de **type double** .  <br/> |
|Erreur  <br/> |Indique une erreur. Il s’agit à des fins de rapport d’erreurs. Il ne peut pas être utilisé dans les restrictions pour l’obtention ou la définition des valeurs.  <br/> |
|Virgule flottante  <br/> |Indique un **float**.  <br/> |
|FloatArray  <br/> |Indique un tableau de valeurs **float** .  <br/> |
|Entier  <br/> |Indique un nombre entier.  <br/> |
|IntegerArray  <br/> |Indique un tableau d’entiers.  <br/> |
|Long  <br/> |Indique un **type long**.  <br/> |
|LongArray  <br/> |Indique un tableau de valeurs de **type long** .  <br/> |
|Null  <br/> |Indique une valeur nulle. Il s’agit à des fins de rapport d’erreurs. Il ne peut pas être utilisé dans les restrictions pour l’obtention ou la définition des valeurs.  <br/> |
|Objet  <br/> |Indique un objet. Il s’agit à des fins de rapport d’erreurs. Il ne peut pas être utilisé dans les restrictions pour l’obtention ou la définition des valeurs.  <br/> |
|ObjectArray  <br/> |Indique un tableau d’objets. Il s’agit à des fins de rapport d’erreurs. Il ne peut pas être utilisé dans les restrictions pour l’obtention ou la définition des valeurs.  <br/> |
|Nom court  <br/> |Indique un **court**.  <br/> |
|ShortArray  <br/> |Indique un tableau de valeurs **courtes** .  <br/> |
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

