---
title: Contacts
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 65312428-548c-4fe9-971a-d0dab3be5ddf
description: L’élément personnes spécifie un tableau de données personnage renvoyées à la suite d’une demande FindPeople.
ms.openlocfilehash: df6f1af34872abe13a1d0f3a98b0354c55354e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828712"
---
# <a name="people"></a>Contacts

L’élément **personnes** spécifie un tableau de données personnage renvoyées à la suite d’une demande **FindPeople** . 
  
```XML
<People>
   <Persona/>
</People>
```

**ArrayOfPeopleType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Personnage](persona.md)
  
### <a name="parent-elements"></a>Éléments parents

[FindPeopleResponse](findpeopleresponse.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

