---
title: Actions (RuleActionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2afba70c-65f7-458c-a4e6-a2cd9bccc0f9
description: L’élément Actions contient une liste d’actions associées aux règles de boîte de réception.
ms.openlocfilehash: 8ed8095ca8b41e037c2c0dad319c9c4ab99ed2bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755245"
---
# <a name="actions-ruleactionstype"></a>Actions (RuleActionsType)

L’élément **Actions** contient une liste d’actions associées aux règles de boîte de réception. 
  
```XML
<Actions>
   <AssignCategories/>
   <CopyToFolder/>
   <Delete/>
   <ForwardAsAttachmentToRecipients/>
   <ForwardToRecipients/>
   <MarkImportance/>
   <MarkAsRead/>
   <MoveToFolder/>
   <PermanentDelete/>
   <RedirectToRecipients/>
   <SendSMSAlertToRecipients/>
   <ServerReplyWithMessage/>
   <StopProcessingRules/>
</Actions>
```

 **RuleActionsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

[AssignCategories](assigncategories.md) | [CopyToFolder](copytofolder.md) | [Supprimer](delete.md) | [ForwardAsAttachmentToRecipients](forwardasattachmenttorecipients.md) | [ForwardToRecipients](forwardtorecipients.md) | [MarkImportance](markimportance.md) | [MarkAsRead ](markasread.md)  |  [MoveToFolder](movetofolder.md) | [PermanentDelete](permanentdelete.md) | [RedirectToRecipients](redirecttorecipients.md) | [SendSMSAlertToRecipients](sendsmsalerttorecipients.md) | [ServerReplyWithMessage](serverreplywithmessage.md)  |  [ StopProcessingRules](stopprocessingrules.md)
  
### <a name="parent-elements"></a>Éléments parents

[Règle (RuleType)](rule-ruletype.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

