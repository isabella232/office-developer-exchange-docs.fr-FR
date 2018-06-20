---
title: UnresolvedEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnresolvedEntry
api_type:
- schema
ms.assetid: 5ac6116a-3b24-40f8-a877-dbe9a6935919
description: L’élément UnresolvedEntry contient le nom d’une liste de contacts ou de distribution à résoudre.
ms.openlocfilehash: 98b447cd49685b49f73f75f12d921a65749be245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838836"
---
# <a name="unresolvedentry"></a>UnresolvedEntry

L’élément **UnresolvedEntry** contient le nom d’une liste de contacts ou de distribution à résoudre. 
  
[ResolveNames](resolvenames.md)
  
[UnresolvedEntry](unresolvedentry.md)
  
```xml
<UnresolvedEntry/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResolveNames](resolvenames.md) <br/> |Définit une demande de résolution de noms ambigus.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte représente le nom d’une liste de contacts ou de distribution public. La longueur minimale de la chaîne est un caractère.
  
## <a name="remarks"></a>Remarques

La valeur de texte de cet élément est utilisée pour résoudre des noms sur les champs suivants :
  
- Prénom
    
- Nom
    
- Nom d’affichage
    
- Nom complet
    
- Office
    
- Alias
    
- adresse SMTP
    
Adresses de messagerie avec des types de routage préfixés, tel que smtp ou sip, sont enregistrés dans un tableau à valeurs multiples. L' [opération ResolveNames](resolvenames-operation.md) effectue une correspondance partielle dans chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ». Si vous ne spécifiez pas un type de routage, l’opération **ResolveNames** par défaut pour le type de routage du service smtp, faire correspondre à une propriété d’adresse SMTP principale et recherche pas dans le tableau à valeurs multiples. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération ResolveNames](resolvenames-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

