---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: L’élément Position spécifie la position d’une entité extraite d’un message.
ms.openlocfilehash: 4bd8f3088891e918e13d5ef1ec8e3e5217cb3fa1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828853"
---
# <a name="position"></a>Position

L’élément **Position** spécifie la position d’une entité extraite d’un message. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[UrlEntity](urlentity.md) | [AddressEntity](addressentity.md) | [EmailAddressEntity](emailaddressentity.md) | [MeetingSuggestion](meetingsuggestion.md) | [Contact (TypeContact)](contact-contacttype.md) | [téléphone (PhoneEntityType)](phone-phoneentitytype.md)  |  [ TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **Position** est l’emplacement où une entité extraite à l’origine dans le message source. Les valeurs de texte de l’élément **Position** sont : 
  
- **LatestReply** - l’entité extraite provient de la réponse au message le plus récent. 
    
- **Autres** - l’entité extraite provient d’une partie du message non définie. 
    
- **Objet** : l’entité extraite provient de l’objet du message. 
    
- **Signature** - l’entité extraite provient de la signature du message. 
    
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

