---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: L’élément UnresolvedEntry contient le nom d’un contact ou d’une liste de distribution à résoudre.
ms.openlocfilehash: 77074d5aed0a799d355fd176a8c9c06f2dffec5a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538666"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

**L’élément UnresolvedEntry** contient le nom d’un contact ou d’une liste de distribution à résoudre. 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Définit une demande de résolution de noms ambigus.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente le nom d’un contact public ou d’une liste de distribution. La longueur minimale de la chaîne est d’un caractère.
  
## <a name="remarks"></a>Remarques

La valeur de texte de cet élément est utilisée pour résoudre les noms par rapport aux champs suivants :
  
- Prénom
    
- Nom de famille
    
- Nom d’affichage
    
- Nom complet
    
- Office
    
- Alias
    
- Adresse SMTP
    
Les adresses de messagerie avec des types de routage préfixés, tels que smtp ou sip, sont enregistrées dans un tableau à valeurs multiples. [L’opération ResolveNames](resolvenames-operation.md) effectue une correspondance partielle avec chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ». Si vous ne spécifiez pas de type de routage, l’opération **ResolveNames** correspondra par défaut au type de routage smtp, la fera correspondre à une propriété d’adresse SMTP principale et ne recherchera pas dans le tableau à valeurs multiples. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ResolveNames](resolvenames-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

