---
title: MailboxStat
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 5f24dc30-3ac2-4c82-9dfc-be9dbdb585be
description: L’élément MailboxStat spécifie les statistiques d’une boîte aux lettres dans le cas d’une recherche de découverte.
ms.openlocfilehash: d48f033df4cfec47313ce690acd19d916b963c00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522809"
---
# <a name="mailboxstat"></a>MailboxStat

**L’élément MailboxStat** spécifie les statistiques d’une boîte aux lettres dans le cas d’une recherche de découverte. 
  
```XML
<MailboxStat>
   <MailboxId/>
   <DisplayName/>
   <ItemCount/>
   <Size/>
</MailboxStat>
```

**MailboxStatisticsItemType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[MailboxId](mailboxid.md)  |  [DisplayName (chaîne)](displayname-string.md)  |  [ItemCount](itemcount.md)  |  [Taille (longue)](size-long.md)
  
### <a name="parent-elements"></a>Éléments parents

[MailboxStats](mailboxstats.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

