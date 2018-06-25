---
title: Occurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: L’élément Occurrence représente une seule occurrence de modification d’un élément de calendrier périodique.
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828653"
---
# <a name="occurrence"></a>Occurrence

L’élément **Occurrence** représente une seule occurrence de modification d’un élément de calendrier périodique. 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

**OccurrenceInfoType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID d’élément](itemid.md) <br/> |Contient la clé unique identificateur et modification d’une occurrence de modification d’un élément de calendrier périodique.  <br/> |
|[Début](start.md) <br/> |Représente l’heure de début d’une occurrence de modification d’un élément de calendrier périodique.  <br/> |
|[Fin](end-ex15websvcsotherref.md) <br/> |Représente l’heure de fin d’une occurrence de modification d’un élément de calendrier périodique.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Représente l’heure de début d’origine d’une occurrence de modification d’un élément de calendrier périodique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Contient une collection d’occurrences d’élément calendrier périodiques qui ont été modifiés afin qu’ils soient différents de celui de l’élément maître de périodicité.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

