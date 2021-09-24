---
title: Name (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Name
api_type:
- schema
ms.assetid: 98c58c53-9acc-4e89-9fcf-03f1b05abee1
description: L’élément Name représente le nom d’un utilisateur de boîte aux lettres.
ms.openlocfilehash: 096b5db4f7bc2de7d1d7355e4e0dba2684bd06d8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515515"
---
# <a name="name-emailaddresstype"></a>Name (EmailAddressType)

**L’élément Name** représente le nom d’un utilisateur de boîte aux lettres. 
  
```xml
<Name/>
```

**chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie une adresse de messagerie entièrement résolue.  <br/> |
|[RoomList](roomlist.md) <br/> |Identifie une liste de salles de réunion.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif. **L’élément Name** existe dans les types **AttachmentType,** **EmailAddressType** et **EmailAddress.** **L’élément Name** dans le type **EmailAddress** est décrit dans la rubrique [d’élément Name (EmailAddress).](name-emailaddress.md) 
  
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

