---
title: Occurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: L’élément Occurrence représente une occurrence modifiée unique d’un élément de calendrier périodique.
ms.openlocfilehash: 465c02263eadfc74629a8e21ebccf076206ec0d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518091"
---
# <a name="occurrence"></a>Occurrence

**L’élément Occurrence** représente une occurrence modifiée unique d’un élément de calendrier périodique. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Contient l’identificateur unique et la clé de modification d’une occurrence modifiée d’un élément de calendrier périodique.  <br/> |
|[Start](start.md) <br/> |Représente l’heure de début d’une occurrence modifiée d’un élément de calendrier périodique.  <br/> |
|[Fin ](end-ex15websvcsotherref.md) <br/> |Représente l’heure de fin d’une occurrence modifiée d’un élément de calendrier périodique.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Représente l’heure de début d’origine d’une occurrence modifiée d’un élément de calendrier périodique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Contient une collection d’occurrences d’éléments de calendrier périodiques qui ont été modifiées afin qu’elles soient différentes de l’élément maître de récurrence.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

