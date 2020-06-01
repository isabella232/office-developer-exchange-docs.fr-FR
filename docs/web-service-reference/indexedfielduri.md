---
title: IndexedFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedFieldURI
api_type:
- schema
ms.assetid: 5c9cd0b5-7eca-480a-8730-fe98b1779afa
description: L’élément IndexedFieldURI identifie les membres individuels d’un dictionnaire.
ms.openlocfilehash: f794d9970590417d916925f7258b28d4f0920d0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467017"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

L’élément **IndexedFieldURI** identifie les membres individuels d’un dictionnaire. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**FieldURI** <br/> |Identifie le dictionnaire qui contient le membre à renvoyer. Cet attribut est obligatoire.  <br/> |
|**FieldIndex** <br/> |Identifie le membre du dictionnaire à renvoyer. Cet attribut est obligatoire.  <br/> |
   
#### <a name="fielduri-attribute"></a>Attribut FieldURI

|**Valeur**|**Description**|
|:-----|:-----|
|élément : InternetMessageHeader  <br/> |Représente l’en-tête de message d’un élément.  <br/> |
|contacts : IMAddress  <br/> |Représente l’adresse de messagerie instantanée d’un contact.  <br/> |
|contacts : PhysicalAddress : rue  <br/> |Représente l’adresse postale d’un contact.  <br/> |
|contacts : PhysicalAddress : City  <br/> |Représente la ville d’un contact.  <br/> |
|contacts : PhysicalAddress : état  <br/> |Représente l’état d’un contact.  <br/> |
|contacts : PhysicalAddress : pays  <br/> |Représente le pays/la région d’un contact.  <br/> |
|contacts : PhysicalAddress : CodePostal  <br/> |Représente le code postal d’un contact.  <br/> |
|contacts : PhoneNumber  <br/> |Représente le numéro de téléphone d’un contact.  <br/> |
|contacts : EmailAddress  <br/> |Représente l’adresse de messagerie d’un contact.  <br/> |
|DistributionList : membres : membre  <br/> |Représente un membre d’une liste de distribution.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires à obtenir, définir ou créer.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Représente la propriété qui est utilisée pour déterminer l’ordre des éléments groupés pour un jeu de résultats FindItem groupé.  <br/> |
|[GroupBy](groupby.md) <br/> |Spécifie un regroupement arbitraire pour les requêtes FindItem.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

