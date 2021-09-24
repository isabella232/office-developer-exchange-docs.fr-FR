---
title: ToRecipients
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ToRecipients
api_type:
- schema
ms.assetid: 72dc3be8-30bb-4ae1-acf4-fb94ff490631
description: L'élément ToRecipients contient un tableau de destinataires d'un élément. Voici les principaux destinataires d'un élément.
ms.openlocfilehash: 1e49a3113328b0573124948056f684de72f27b3f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527250"
---
# <a name="torecipients"></a>ToRecipients

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **ToRecipients** contient un tableau de destinataires d'un élément. Voici les principaux destinataires d'un élément. 
  
```xml
<ToRecipients>
   <Mailbox/>
</ToRecipients>
```

 **ArrayOfRecipientsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[RemoveItem](removeitem.md) <br/> |Supprime un élément de la banque d'informations Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Représente un message électronique Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Représente une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Représente une demande de réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Représente une réponse à une réunion dans la banque d'informations Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Représente une annulation de réunion dans la banque d'informations Exchange.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Représente une réponse à accepter à une demande de réunion.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Représente un provisoire répond à une demande de réunion.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Représente une réponse de refus à une demande de réunion.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Contient une réponse à l'auteur d'un élément dans la banque d'informations Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Contient une réponse destinée à tous les destinataires identifiés d'un élément dans la banque d'informations Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Contient un élément de la banque Exchange pour transférer à des destinataires.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Représente l'objet de réponse qui est utilisé pour annuler une réunion.  <br/> |
   
## <a name="remarks"></a>Remarques

Impossible d'obtenir **ToRecipients** à l'aide d'une demande FindItem. Utiliser une demande de GetItem pour obtenir le **ToRecipients**.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

