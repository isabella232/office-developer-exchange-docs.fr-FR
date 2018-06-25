---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: L’élément MailboxSearchScope spécifie une boîte aux lettres et une zone de recherche pour une recherche de découverte.
ms.openlocfilehash: 657e6dfd4eb6c6c0eabb18546e7090c524e28e5e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828297"
---
# <a name="mailboxsearchscope"></a>MailboxSearchScope

L’élément **MailboxSearchScope** spécifie une boîte aux lettres et une zone de recherche pour une recherche de découverte. 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

**MailboxSearchScopeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Boîte aux lettres (string)](mailbox-string.md) | [SearchScope](searchscope.md)
  
### <a name="parent-elements"></a>Éléments parents

[MailboxSearchScopes](mailboxsearchscopes.md)
  
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
   

