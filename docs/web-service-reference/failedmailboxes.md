---
title: FailedMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: L’élément FailedMailboxes spécifie un tableau de boîtes aux lettres ayant échoué sur la recherche.
ms.openlocfilehash: f68cc29dc9da3b1b74369aa21cde65866e42f3b8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756347"
---
# <a name="failedmailboxes"></a>FailedMailboxes

L’élément **FailedMailboxes** spécifie un tableau de boîtes aux lettres ayant échoué sur la recherche. 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 **ArrayOfFailedSearchMailboxesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FailedMailbox](failedmailbox.md) <br/> |Spécifie le message d’erreur pour une boîte aux lettres ayant échoué sur la recherche.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SearchMailboxesResult](searchmailboxesresult.md) <br/> |Contient le résultat de la demande **SearchMailboxes** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

