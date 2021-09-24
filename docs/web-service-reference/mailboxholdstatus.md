---
title: MailboxHoldStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 92608b77-8aa4-403b-a4de-01e3a60af3e0
description: L’élément MailboxHoldStatus spécifie l’état de la boîte aux lettres.
ms.openlocfilehash: de63acb14862e9f8cefded7130318c7f8cbd685f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540768"
---
# <a name="mailboxholdstatus"></a>MailboxHoldStatus

**L’élément MailboxHoldStatus** spécifie l’état de la boîte aux lettres. 
  
```XML
<MailboxHoldStatus>
   <Mailbox/>
   <Status/>
   <AdditionalInfo/>
</MailboxHoldStatus>
```

**MailboxHoldStatusType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[Boîte aux lettres (chaîne)](mailbox-string.md)  |  [Status (HoldStatusType)](status-holdstatustype.md)  |  [AdditionalInfo](additionalinfo.md)
  
### <a name="parent-elements"></a>Éléments parents

[MailboxHoldStatuses](mailboxholdstatuses.md)
  
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
   

