---
title: MailboxSearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ef4a4203-61e5-46b8-9fa4-d1a10e785aa2
description: L’élément MailboxSearchScope spécifie une boîte aux lettres et une étendue de recherche pour une recherche de découverte.
ms.openlocfilehash: 832992e4e1dcf96029be4228906b2762f11f3fbe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544121"
---
# <a name="mailboxsearchscope"></a>MailboxSearchScope

**L’élément MailboxSearchScope** spécifie une boîte aux lettres et une étendue de recherche pour une recherche de découverte. 
  
```XML
<MailboxSearchScope>
   <Mailbox/>
   <SearchScope/>
<MailboxSearchScope>
```

**MailboxSearchScopeType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Boîte aux lettres (chaîne)](mailbox-string.md)  |  [SearchScope](searchscope.md)
  
### <a name="parent-elements"></a>Éléments parents

[MailboxSearchScopes](mailboxsearchscopes.md)
  
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
   

