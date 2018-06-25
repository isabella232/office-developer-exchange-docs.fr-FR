---
title: MailboxQuery
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e4b496f7-63fa-479a-b045-73276573f64f
description: L’élément MailboxQuery spécifie une requête et l’étendue d’une recherche de découverte.
ms.openlocfilehash: 371cddd8c4f01525b654f0ad9788cf9dd62ac888
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828295"
---
# <a name="mailboxquery"></a>MailboxQuery

L’élément **MailboxQuery** spécifie une requête et l’étendue d’une recherche de découverte. 
  
```XML
<MailboxQuery>
   <Query/>
   <MailboxSearchScopes/>
</MailboxQuery>
```

**MailboxQueryType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[Requête](query.md) | [MailboxSearchScopes](mailboxsearchscopes.md)
  
### <a name="parent-elements"></a>Éléments parents

[SearchQueries](searchqueries.md)
  
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
   

