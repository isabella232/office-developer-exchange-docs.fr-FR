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
description: L’élément Conditions identifie les conditions qui, lorsque remplies, déclenchent des actions de règle d’une règle.
ms.openlocfilehash: f66777e82892122c4c7dac45bdef3c42f5c4a577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755534"
---
# <a name="conditions"></a>Conditions

L’élément **Conditions** identifie les conditions qui, lorsque remplies, déclenchent des actions de règle d’une règle. 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Contient les catégories qui doivent être appliquées à un message entrant afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsBodyStrings](containsbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsHeaderStrings](containsheaderstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans les en-têtes des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsRecipientStrings](containsrecipientstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans les **ToRecipients** **CcRecipients** propriétés ou des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsSenderStrings](containssenderstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans la propriété **From** des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsSubjectOrBodyStrings](containssubjectorbodystrings.md) <br/> |Indique les chaînes qui doivent apparaître dans le corps ou l’objet des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[ContainsSubjectStrings](containssubjectstrings.md) <br/> |Indique les chaînes qui doivent apparaître dans l’objet des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[FlaggedForAction](flaggedforaction.md) <br/> |Spécifie l’indicateur pour la valeur d’action qui doit apparaître dans les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[FromAddresses](fromaddresses.md) <br/> |Indique les adresses de messagerie à partir de laquelle les messages entrants doivent être envoyés afin que l’exception ou la condition à appliquer.  <br/> |
|[FromConnectedAccounts](fromconnectedaccounts.md) <br/> |Représente les noms de compte de messagerie à partir de laquelle les messages entrants doivent avoir été agrégées afin que l’exception ou la condition à appliquer.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Indique si les messages entrants ont pour que les pièces jointes afin que l’exception ou la condition à appliquer.  <br/> |
|[Importance](importance.md) <br/> |Spécifie l’importance est marqué sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[IsApprovalRequest](isapprovalrequest.md) <br/> |Indique si les messages entrants doivent être des demandes d’approbation afin que l’exception ou la condition à appliquer.  <br/> |
|[IsAutomaticForward](isautomaticforward.md) <br/> |Indique si les messages entrants doivent être des transferts automatiques afin que l’exception ou la condition à appliquer.  <br/> |
|[IsAutomaticReply](isautomaticreply.md) <br/> |Indique si les messages entrants doivent être des réponses automatiques afin que l’exception ou la condition à appliquer.  <br/> |
|[IsEncrypted](isencrypted.md) <br/> |Indique si les messages entrants doivent être chiffré afin que l’exception ou la condition à appliquer S/MIME.  <br/> |
|[IsMeetingRequest](ismeetingrequest.md) <br/> |Indique si les messages entrants doivent être les demandes de réunion dans l’ordre de l’exception ou la condition à appliquer.  <br/> |
|[IsMeetingResponse](ismeetingresponse.md) <br/> |Indique si les messages entrants doivent être réponses de réunion afin que l’exception ou la condition à appliquer.  <br/> |
|[IsNDR](isndr.md) <br/> |Indique si les messages entrants doivent être des rapports de non remise (NDR) afin que l’exception ou la condition à appliquer.  <br/> |
|[IsPermissionControlled](ispermissioncontrolled.md) <br/> |Indique si les messages entrants doivent être sous contrôlée de l’autorisation (protégés par RMS) afin que l’exception ou la condition à appliquer.  <br/> |
|[IsReadReceipt](isreadreceipt.md) <br/> |Indique si les messages entrants doivent être des confirmations de lecture afin que l’exception ou la condition à appliquer.  <br/> |
|[IsSigned](issigned.md) <br/> |Indique si les messages entrants doivent être signés S/MIME afin que l’exception ou la condition à appliquer.  <br/> |
|[IsVoicemail](isvoicemail.md) <br/> |Indique si les messages entrants doivent être des messages vocaux afin que l’exception ou la condition à appliquer.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Représente les classes d’élément qui doivent être marqués sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Représente les classifications de messages qui doivent être marquées sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[NotSentToMe](notsenttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres ne doit pas être dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[SentCcMe](sentccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **CcRecipients** des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[SentOnlyToMe](sentonlytome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit être le seul à la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[SentToAddresses](senttoaddresses.md) <br/> |Indique les adresses de messagerie dont les messages entrants ont été envoyées aux afin que l’exception ou la condition à appliquer.  <br/> |
|[SentToMe](senttome.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété **ToRecipients** des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[SentToOrCcMe](senttoorccme.md) <br/> |Indique si le propriétaire de la boîte aux lettres doit se trouver dans la propriété un **CcRecipients** **ToRecipients** ou des messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Indique le critère de diffusion qui doit être marqué sur les messages entrants afin que l’exception ou la condition à appliquer.  <br/> |
|[WithinDateRange](withindaterange.md) <br/> |Spécifie la plage de dates dans laquelle les messages entrants ont reçue dans l’ordre de l’exception ou la condition à appliquer.  <br/> |
|[WithinSizeRange](withinsizerange.md) <br/> |Spécifie les tailles minimales et maximales des messages entrants doivent être dans l’ordre de l’exception ou la condition à appliquer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Règle (RuleType)](rule-ruletype.md) <br/> |Contient une règle unique et représente une règle de boîte aux lettres d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Exceptions](exceptions.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

