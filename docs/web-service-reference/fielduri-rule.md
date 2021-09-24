---
title: FieldUri (Rule)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cecdea78-de9c-48be-ae31-03877feafeec
description: L’élément FieldURI spécifie l’URI du champ de règle à l’origine de l’erreur de validation.
ms.openlocfilehash: c1390f6643614216fa86053368ba012cd0883ff7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513730"
---
# <a name="fielduri-rule"></a>FieldUri (Rule)

**L’élément FieldURI** spécifie l’URI du champ de règle à l’origine de l’erreur de validation. 
  
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
|[Erreur](error.md) <br/> |Représente une erreur de validation unique sur une valeur de propriété de règle particulière, une valeur de propriété de prédicat ou une valeur de propriété d’action.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de cet élément est limitée à l’une des chaînes suivantes :
  
- RuleId
    
- DisplayName
    
- Priorité
    
- IsNotSupported
    
- Actions
    
- Condition:Categories
    
- Condition:ContainsBodyStrings
    
- Condition:ContainsHeaderStrings
    
- Condition:ContainsRecipientStrings
    
- Condition:ContainsSenderStrings
    
- Condition:ContainsSubjectOrBodyStrings
    
- Condition:ContainsSubjectStrings
    
- Condition:FlaggedForAction
    
- Condition:FromAddresses
    
- Condition:FromConnectedAccounts
    
- Condition:HasAttachments
    
- Condition:Importance
    
- Condition:IsApprovalRequest
    
- Condition:IsAutomaticForward
    
- Condition:IsAutomaticReply
    
- Condition:IsEncrypted
    
- Condition:IsMeetingRequest
    
- Condition:IsMeetingResponse
    
- Condition:IsNDR
    
- Condition:IsPermissionControlled
    
- Condition:IsReadReceipt
    
- Condition:IsSigned
    
- Condition:IsVoicemail
    
- Condition:ItemClasses
    
- Condition:MessageClassifications
    
- Condition:NotSentToMe
    
- Condition:SentCcMe
    
- Condition:SentOnlyToMe
    
- Condition:SentToAddresses
    
- Condition:SentToMe
    
- Condition:SentToOrCcMe
    
- Condition:Sensitivity
    
- Condition:WithinDateRange
    
- Condition:WithinSizeRange
    
- Exception:Categories
    
- Exception:ContainsBodyStrings
    
- Exception:ContainsHeaderStrings
    
- Exception:ContainsRecipientStrings
    
- Exception:ContainsSenderStrings
    
- Exception:ContainsSubjectOrBodyStrings
    
- Exception:ContainsSubjectStrings
    
- Exception:FlaggedForAction
    
- Exception:FromAddresses
    
- Exception:FromConnectedAccounts
    
- Exception:HasAttachments
    
- Exception:Importance
    
- Exception:IsApprovalRequest
    
- Exception:IsAutomaticForward
    
- Exception:IsAutomaticReply
    
- Exception:IsEncrypted
    
- Exception:IsMeetingRequest
    
- Exception:IsMeetingResponse
    
- Exception:IsNDR
    
- Exception:IsPermissionControlled
    
- Exception:IsReadReceipt
    
- Exception:IsSigned
    
- Exception:IsVoicemail
    
- Exception:ItemClasses
    
- Exception:MessageClassifications
    
- Exception:NotSentToMe
    
- Exception:SentCcMe
    
- Exception:SentOnlyToMe
    
- Exception:SentToAddresses
    
- Exception:SentToMe
    
- Exception:SentToOrCcMe
    
- Exception:Sensitivity
    
- Exception:WithinDateRange
    
- Exception:WithinSizeRange
    
- Action:AssignCategories
    
- Action:CopyToFolder
    
- Action:Delete
    
- Action:ForwardAsAttachmentToRecipients
    
- Action:ForwardToRecipients
    
- Action:MarkImportance
    
- Action:MarkAsRead
    
- Action:MoveToFolder
    
- Action:PermanentDelete
    
- Action:RedirectToRecipients
    
- Action:SendSMSAlertToRecipients
    
- Action:ServerReplyWithMessage
    
- Action:StopProcessingRules
    
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
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

