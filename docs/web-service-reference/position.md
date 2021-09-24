---
title: Position
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 46726ebb-a403-4793-8378-282aa7dc39d0
description: L’élément Position spécifie la position d’une entité extraite d’un message.
ms.openlocfilehash: 6b4e7c12bbcf12b8804619caa508f5c2c0bc4eda
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515291"
---
# <a name="position"></a>Position

**L’élément Position** spécifie la position d’une entité extraite d’un message. 
  
```XML
<Position> LatestReply | Other | Subject | Signature </Position>
```

 **EmailPositionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[UrlEntity](urlentity.md)  |  [AddressEntity](addressentity.md)  |  [EmailAddressEntity](emailaddressentity.md)  |  [MeetingSuggestion](meetingsuggestion.md)  |  [Contact (ContactType)](contact-contacttype.md)  |  [Téléphone (PhoneEntityType)](phone-phoneentitytype.md)  |  [TaskSuggestion](tasksuggestion.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément Position** est l’emplacement d’origine d’une entité extraite dans le message source. Les valeurs de texte de **l’élément Position** sont : 
  
- **LatestReply** : l’entité extraite provient de la dernière réponse au message. 
    
- **Autre** : l’entité extraite provient d’une partie non définie du message. 
    
- **Objet** : l’entité extraite provient de l’objet du message. 
    
- **Signature** : l’entité extraite provient de la signature du message. 
    
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

