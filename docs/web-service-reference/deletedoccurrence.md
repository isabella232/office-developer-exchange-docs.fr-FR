---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: L’élément DeletedOccurrence représente une occurrence supprimée d’un élément de calendrier périodique.
ms.openlocfilehash: 69e77f86097fe7037fc217806e4ef1b33b99c549
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542483"
---
# <a name="deletedoccurrence"></a>DeletedOccurrence

**L’élément DeletedOccurrence** représente une occurrence supprimée d’un élément de calendrier périodique. 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 **DeletedOccurrenceInfoType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Start](start.md) <br/> |Représente l’heure de début d’une occurrence supprimée d’un élément de calendrier périodique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Contient un tableau d’occurrences supprimées d’un élément de calendrier périodique.  <br/> |
   
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
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)

