---
title: Expéditeur (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Sender
api_type:
- schema
ms.assetid: 717eb6d0-d167-4b20-92e2-5d08b96186c4
description: L’élément de l’expéditeur représente l’adresse de messagerie de l’expéditeur du message.
ms.openlocfilehash: bac62412caf1044c13015f1d9d7ef63552747c1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829320"
---
# <a name="sender-emailaddresstype"></a>Expéditeur (EmailAddressType)

L’élément de **l’expéditeur** représente l’adresse de messagerie de l’expéditeur du message. 
  
```XML
<Sender>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</Sender>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Nom (EmailAddressType)](name-emailaddresstype.md) <br/> |Représente le nom de l’utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP Simple Mail Transfer Protocol () principal d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Représente le protocole de routage pour le destinataire. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Représente le type de boîte aux lettres qui est représenté par l’adresse de messagerie. Cet élément est facultatif.  <br/> |
|[ID d’élément](itemid.md) <br/> |Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires à partir du dossier de Contacts d’un utilisateur. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Spécifie les critères pour les types de messages.  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |Contient un résultat de message unique d’un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) .  <br/> |
|[MessageTrackingReport](messagetrackingreport.md) <br/> |Contient un seul message renvoyé dans un [Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md).  <br/> |
   
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
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

