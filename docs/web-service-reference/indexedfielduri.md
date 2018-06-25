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
ms.openlocfilehash: 6a75e8855ecabf15ca31bb1e05d569c258a43b0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827909"
---
# <a name="indexedfielduri"></a>IndexedFieldURI

L’élément **IndexedFieldURI** identifie les membres individuels d’un dictionnaire. 
  
```xml
<IndexedFieldURI FieldURI="" FieldIndex="" />
```

 **PathToIndexedFieldType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**FieldURI** <br/> |Identifie le dictionnaire qui contient le membre à renvoyer. Cet attribut est requis.  <br/> |
|**FieldIndex** <br/> |Identifie le membre du dictionnaire à renvoyer. Cet attribut est requis.  <br/> |
   
#### <a name="fielduri-attribute"></a>Attribut FieldURI

|**Valeur**|**Description**|
|:-----|:-----|
|élément : InternetMessageHeader  <br/> |Représente l’en-tête de message d’un élément.  <br/> |
|contacts : ImAddress  <br/> |Représente l’adresse d’un contact de messagerie instantanée.  <br/> |
|contacts : PhysicalAddress:Street  <br/> |Représente l’adresse d’un contact.  <br/> |
|contacts : PhysicalAddress:City  <br/> |Représente la ville d’un contact.  <br/> |
|contacts : PhysicalAddress:State  <br/> |Représente l’état d’un contact.  <br/> |
|contacts : PhysicalAddress:Country  <br/> |Représente la pays/la région d’un contact.  <br/> |
|contacts : PhysicalAddress:PostalCode  <br/> |Représente le code postal du contact.  <br/> |
|contacts : PhoneNumber  <br/> |Représente le numéro de téléphone d’un contact.  <br/> |
|contacts : EmailAddress  <br/> |Représente l’adresse de messagerie d’un contact.  <br/> |
|DistributionList:members:Member  <br/> |Représente un membre d’une liste de distribution.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires pour obtenir, définir ou créer.  <br/> |
|[AggregateOn](aggregateon.md) <br/> |Représente la propriété qui est utilisée pour déterminer l’ordre des éléments regroupés pour un jeu de résultats FindItem groupé.  <br/> |
|[GroupBy](groupby.md) <br/> |Spécifie un regroupement pour les requêtes FindItem arbitraire.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

