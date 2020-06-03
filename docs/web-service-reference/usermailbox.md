---
title: UserMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1d47141c-3c3f-45b8-90c5-33a44adb34b2
description: L’élément UserMailbox identifie une boîte aux lettres utilisateur.
ms.openlocfilehash: 9bb1b08320f5e6f4843383a8e3aff96fc3dcccad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465316"
---
# <a name="usermailbox"></a>UserMailbox

L’élément **UserMailbox** identifie une boîte aux lettres utilisateur. 
  
```XML
<UserMailbox Id="" IsArchive=""/>
```

 **UserMailboxType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de texte de l’attribut **ID** est l’identificateur de la boîte aux lettres.  <br/> |
|IsArchive  <br/> |La valeur de texte de l’attribut **IsArchive** indique si la boîte aux lettres est une boîte aux lettres d’archivage. Une valeur de texte de **true** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres d’archivage. La valeur **false** pour l’attribut **IsArchive** indique que la boîte aux lettres est une boîte aux lettres principale.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Boîtes aux lettres (ArrayOfUserMailboxesType)](mailboxes-arrayofusermailboxestype.md)  |  [MailboxStatisticsSearchResult](mailboxstatisticssearchresult.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |true  <br/> |
   

