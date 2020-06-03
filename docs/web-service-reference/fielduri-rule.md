---
title: FieldUri (règle)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: L’élément FieldURI spécifie l’URI vers le champ de règle à l’origine de l’erreur de validation.
ms.openlocfilehash: 3d88efdf951af580f81b5e2e7a544dcdf70ea830
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461246"
---
# <a name="fielduri-rule"></a>FieldUri (règle)

L’élément **FieldURI** spécifie l’URI vers le champ de règle à l’origine de l’erreur de validation. 
  
```XML
<FieldURI/>
```

 **RuleFieldURIType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Erreur](error.md) <br/> |Représente une seule erreur de validation sur une valeur de propriété de règle, une valeur de propriété de prédicat ou une valeur de propriété d’action particulière.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est restreinte à l’une des chaînes suivantes :
  
- RuleId
    
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
    
- Condition : importance
    
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
    
- Condition : sensibilité
    
- Condition : WithinDateRange
    
- Condition : WithinSizeRange
    
- Exception : Categories
    
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
    
- Exception : importance
    
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
    
- Exception : Sensitivity
    
- Exception : WithinDateRange
    
- Exception : WithinSizeRange
    
- Action : AssignCategories
    
- Action : CopyToFolder,
    
- Action : supprimer
    
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

