---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: L’élément UserMailbox identifie une boîte aux lettres de l’utilisateur.
ms.openlocfilehash: 9f359a2b0ba315c236d4bf189c3de321417bd390
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838961"
---
# <a name="usermailbox"></a>UserMailbox

L’élément **UserMailbox** identifie une boîte aux lettres de l’utilisateur. 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **UserMailboxType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de texte de l’attribut **Id** est l’identificateur de la boîte aux lettres.  <br/> |
|IsArchive  <br/> |La valeur de texte de l’attribut **IsArchive** indique si la boîte aux lettres est une boîte aux lettres d’archive. Une valeur de texte de **la valeur true** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres d’archive. La valeur **false** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres principale.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Boîtes aux lettres (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md) | [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |true  <br/> |
   

