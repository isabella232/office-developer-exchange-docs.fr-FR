---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: L’élément Status spécifie l’état de la boîte aux lettres en attente.
ms.openlocfilehash: a055dde61ae52c266f2349036c881d2b00557171
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521234"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

**L’élément Status** spécifie l’état de la boîte aux lettres en attente. 
  
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

La valeur de texte de **l’élément Status** est l’état de la boîte aux lettres. **L’élément Status** peut avoir les valeurs de la liste suivante. 
  
> NotOnHold : la boîte aux lettres n’est pas en attente.
    
> En attente : la boîte aux lettres est en attente d’être placée ou mise en attente. 
    
> OnHold : la boîte aux lettres a été correctement appliquée à la boîte aux lettres. 
    
> PartialHold : le hold a été appliqué avec succès à certaines boîtes aux lettres, mais pas à toutes les boîtes aux lettres.
    
> Échec : le hold n’a pas réussi à s’appliquer à la boîte aux lettres.
    
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
   

