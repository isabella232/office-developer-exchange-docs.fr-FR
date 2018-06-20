---
title: FieldUri (règle)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: L’élément FieldURI Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation.
ms.openlocfilehash: 88ba54994625d3a950b58e900f28c986c31eddac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756353"
---
# <a name="fielduri-rule"></a>FieldUri (règle)

L’élément **FieldURI** Spécifie l’URI pour le champ règle qui a provoqué l’erreur de validation. 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Erreur](error.md) <br/> |Représente une seule erreur de validation sur une valeur de la propriété règle particulière, la valeur de propriété prédicat ou la valeur de la propriété action.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte pour cet élément est limitée à une des chaînes suivantes :
  
- ID de la règle
    
- DisplayName
    
- Priority
    
- IsNotSupported
    
- Actions
    
- Condition : catégories
    
- Condition : ContainsBodyStrings
    
- Condition : ContainsHeaderStrings
    
- Condition : ContainsRecipientStrings
    
- Condition : ContainsSenderStrings
    
- Condition : ContainsSubjectOrBodyStrings
    
- Condition : ContainsSubjectStrings
    
- Condition : FlaggedForAction
    
- Condition : FromAddresses
    
- Condition : FromConnectedAccounts
    
- Condition : HasAttachments
    
- Condition : Importance
    
- Condition : IsApprovalRequest
    
- Condition : IsAutomaticForward
    
- Condition : IsAutomaticReply
    
- Condition : IsEncrypted
    
- Condition : IsMeetingRequest
    
- Condition : IsMeetingResponse
    
- Condition : IsNDR
    
- Condition : IsPermissionControlled
    
- Condition : IsReadReceipt
    
- Condition : IsSigned
    
- Condition : IsVoicemail
    
- Condition : ItemClasses
    
- Condition : MessageClassifications
    
- Condition : NotSentToMe
    
- Condition : SentCcMe
    
- Condition : SentOnlyToMe
    
- Condition : SentToAddresses
    
- Condition : SentToMe
    
- Condition : SentToOrCcMe
    
- Condition : critère de diffusion
    
- Condition : WithinDateRange
    
- Condition : WithinSizeRange
    
- Exception : catégories
    
- Exception : ContainsBodyStrings
    
- Exception : ContainsHeaderStrings
    
- Exception : ContainsRecipientStrings
    
- Exception : ContainsSenderStrings
    
- Exception : ContainsSubjectOrBodyStrings
    
- Exception : ContainsSubjectStrings
    
- Exception : FlaggedForAction
    
- Exception : FromAddresses
    
- Exception : FromConnectedAccounts
    
- Exception : HasAttachments
    
- Exception : Importance
    
- Exception : IsApprovalRequest
    
- Exception : IsAutomaticForward
    
- Exception : IsAutomaticReply
    
- Exception : IsEncrypted
    
- Exception : IsMeetingRequest
    
- Exception : IsMeetingResponse
    
- Exception : IsNDR
    
- Exception : IsPermissionControlled
    
- Exception : IsReadReceipt
    
- Exception : IsSigned
    
- Exception : IsVoicemail
    
- Exception : ItemClasses
    
- Exception : MessageClassifications
    
- Exception : NotSentToMe
    
- Exception : SentCcMe
    
- Exception : SentOnlyToMe
    
- Exception : SentToAddresses
    
- Exception : SentToMe
    
- Exception : SentToOrCcMe
    
- Exception : critère de diffusion
    
- Exception : WithinDateRange
    
- Exception : WithinSizeRange
    
- Action : AssignCategories
    
- Action : CopyToFolder
    
- Suppression de l’action :
    
- Action : ForwardAsAttachmentToRecipients
    
- Action : ForwardToRecipients
    
- Action : MarkImportance
    
- Action : MarkAsRead
    
- Action : MoveToFolder
    
- Action : PermanentDelete
    
- Action : RedirectToRecipients
    
- Action : SendSMSAlertToRecipients
    
- Action : ServerReplyWithMessage
    
- Action : StopProcessingRules
    
- IsEnabled
    
- IsInError
    
- Conditions
    
- Exceptions
    
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

