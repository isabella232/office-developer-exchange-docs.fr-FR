---
title: Exceptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Exceptions
api_type:
- schema
ms.assetid: 7cd63ac2-3441-4ed4-915b-6f90af4b28fc
description: L’élément Exceptions identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception.
ms.openlocfilehash: 5c92613aa871a200cf790e0709ba71280b226807
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524265"
---
# <a name="exceptions"></a>Exceptions

**L’élément Exceptions** identifie les exceptions qui représentent toutes les conditions d’exception de règle disponibles pour une règle de boîte de réception. 
  
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient les catégories qui doivent être appliquées à un message entrant afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indicule les chaînes qui doivent apparaître dans les en-têtes des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans les **propriétés ToRecipients** ou **CcRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans la propriété **From** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans l’objet des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Spécifie l’indicateur de valeur d’action qui doit apparaître sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indique les adresses de messagerie à partir des lesquelles les messages entrants doivent être envoyés afin que la condition ou l’exception s’applique.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Représente les noms des comptes de messagerie à partir des lesquels les messages entrants doivent avoir été agrégés afin que la condition ou l’exception s’applique.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indique si les messages entrants doivent avoir des pièces jointes pour que la condition ou l’exception s’applique.  <br/> |
|[Importance](importance.md) <br/> |Spécifie l’importance qui est estampillée sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indique si les messages entrants doivent être des demandes d’approbation pour que la condition ou l’exception s’applique.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indique si les messages entrants doivent être des transferts automatiques pour que la condition ou l’exception s’applique.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indique si les messages entrants doivent être des réponses automatiques pour que la condition ou l’exception s’applique.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indique si les messages entrants doivent être chiffrés S/MIME pour que la condition ou l’exception s’applique.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indique si les messages entrants doivent être des demandes de réunion pour que la condition ou l’exception s’applique.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indique si les messages entrants doivent être des réponses à une réunion pour que la condition ou l’exception s’applique.  <br/> |
|[IsNDR](isndr.md) <br/> |Indique si les messages entrants doivent être des rapports de non-remise (NDR) pour que la condition ou l’exception s’applique.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indique si les messages entrants doivent être contrôlés par des autorisations (protégées par RMS) pour que la condition ou l’exception s’applique  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indique si les messages entrants doivent être des reçus de lecture pour que la condition ou l’exception s’applique.  <br/> |
|[IsSigned](issigned.md) <br/> |Indique si les messages entrants doivent être signés S/MIME pour que la condition ou l’exception s’applique.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Indique si les messages entrants doivent être des messages vocaux pour que la condition ou l’exception s’applique.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Représente les classes d’éléments qui doivent être marqués sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Représente les classifications de messages qui doivent être marqués sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres ne doit pas se trouver dans la propriété **ToRecipients** des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CcRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit être le seul dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indique les adresses de messagerie à qui les messages entrants doivent avoir été envoyés afin que la condition ou l’exception s’applique.  <br/> |
|[SentToMe](senttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans une propriété **ToRecipients** ou **CcRecipients** des messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indique le niveau de sensibilité qui doit être marqué sur les messages entrants afin que la condition ou l’exception s’applique.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Spécifie la plage de dates dans laquelle les messages entrants doivent avoir été reçus afin que la condition ou l’exception s’applique.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie la taille minimale et maximale des messages entrants pour que la condition ou l’exception s’applique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Contient une règle unique et représente une règle dans la boîte aux lettres d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Les prédicats de règle sont utilisés comme conditions ou exceptions de règle.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Conditions](conditions.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

