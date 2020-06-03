---
title: État (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: L’élément Status spécifie l’état de conservation d’une boîte aux lettres.
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459986"
---
# <a name="status-holdstatustype"></a>État (HoldStatusType)

L’élément **Status** spécifie l’état de conservation d’une boîte aux lettres. 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **Status** est l’état de conservation d’une boîte aux lettres. L’élément **Status** peut avoir les valeurs répertoriées dans la liste suivante. 
  
> NotOnHold-la boîte aux lettres n’est pas en attente.
    
> En attente : la boîte aux lettres est en attente d’être placée ou libérée en conservation. 
    
> OnHold-la suspension a été appliquée à la boîte aux lettres. 
    
> PartialHold-la conservation a été appliquée avec succès à certaines boîtes aux lettres, mais pas à toutes les boîtes aux lettres.
    
> Failed : la conservation n’a pas pu s’appliquer à la boîte aux lettres.
    
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
   

