---
title: Conditions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conditions
api_type:
- schema
ms.assetid: f049a48c-9585-43f7-8549-0b8cb19a5eea
description: L’élément conditions identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle.
ms.openlocfilehash: 2c6b4794a87cca79b4c723197b57360ad0ff973d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463201"
---
# <a name="conditions"></a>Conditions

L’élément **conditions** identifie les conditions qui, lorsqu’elles sont remplies, déclencheront les actions de règle pour une règle. 
  
```XML
<Conditions>
   <Categories/>
   <ContainsBodyStrings/>
   <ContainsHeaderStrings/>
   <ContainsRecipientStrings/>
   <ContainsSenderStrings/>
   <ContainsSubjectOrBodyStrings/>
   <ContainsSubjectStrings/>
   <FlaggedForAction/>
   <FromAddresses/>
   <FromConnectedAccounts/>
   <HasAttachments/>
   <Importance/>
   <IsApprovalRequest/>
   <IsAutomaticForward/>
   <IsAutomaticReply/>
   <IsEncrypted/>
   <IsMeetingRequest/>
   <IsMeetingResponse/>
   <IsNDR/>
   <IsPermissionControlled/>
   <IsReadReceipt/>
   <IsSigned/>
   <IsVoicemail/>
   <ItemClasses/>
   <MessageClassifications/>
   <NotSentToMe/>
   <SentCcMe/>
   <SentOnlyToMe/>
   <SentToAddresses/>
   <SentToMe/>
   <SentToOrCcMe/>
   <Sensitivity/>
   <WithinDateRange/>
   <WithinSizeRange/>
</Conditions>
```

 **RulePredicatesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Catégories](categories-ex15websvcsotherref.md) <br/> |Contient les catégories qui doivent être appliquées à un message entrant afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans les propriétés **ToRecipients** ou **CCRecipients** des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans la propriété **from** des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans l’objet des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Spécifie l’indicateur de la valeur d’action qui doit apparaître dans les messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indique les adresses de messagerie à partir desquelles les messages entrants doivent être envoyés pour que la condition ou l’exception s’applique.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Représente les noms de compte de messagerie à partir desquels les messages entrants doivent être regroupés pour que la condition ou l’exception s’applique.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indique si les messages entrants doivent contenir des pièces jointes afin que la condition ou l’exception s’applique.  <br/> |
|[Importance](importance.md) <br/> |Spécifie l’importance qui est marquée sur les messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indique si les messages entrants doivent être des demandes d’approbation afin que la condition ou l’exception s’applique.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indique si les messages entrants doivent être des transferts automatiques afin que la condition ou l’exception s’applique.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indique si les messages entrants doivent être des réponses automatiques afin que la condition ou l’exception s’applique.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indique si les messages entrants doivent être chiffrés S/MIME afin que la condition ou l’exception s’applique.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indique si les messages entrants doivent être des demandes de réunion afin que la condition ou l’exception s’applique.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indique si les messages entrants doivent être des réponses à la demande de réunion afin que la condition ou l’exception s’applique.  <br/> |
|[IsNDR](isndr.md) <br/> |Indique si les messages entrants doivent être des notifications d’échec de remise pour que la condition ou l’exception s’applique.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indique si les messages entrants doivent être contrôlés par des autorisations (protection RMS) afin que la condition ou l’exception s’applique.  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indique si les messages entrants doivent être lus en confirmation de lecture afin que la condition ou l’exception s’applique.  <br/> |
|[IsSigned](issigned.md) <br/> |Indique si les messages entrants doivent être S/MIME signés pour que la condition ou l’exception s’applique.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Indique si les messages entrants doivent être des messages vocaux afin que la condition ou l’exception s’applique.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Représente les classes d’éléments qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Représente les classifications de message qui doivent être marquées sur les messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit être le seul dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indique les adresses de messagerie auxquelles les messages entrants doivent avoir été envoyés pour que la condition ou l’exception s’applique.  <br/> |
|[SentToMe](senttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété **ToRecipients** ou **CCRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indique la sensibilité qui doit être marquée sur les messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Spécifie la plage de dates au cours de laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie les tailles minimale et maximale que les messages entrants doivent être pour que la condition ou l’exception s’applique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Contient une seule règle et représente une règle dans la boîte aux lettres d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Exceptions](exceptions.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

