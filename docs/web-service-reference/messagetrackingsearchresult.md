---
title: MessageTrackingSearchResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingSearchResult
api_type:
- schema
ms.assetid: 8ea77aa8-b93f-4287-be36-0a9da06e0946
description: L’élément MessageTrackingSearchResult contient un seul résultat de message pour un élément FindMessageTrackingReportResponse.
ms.openlocfilehash: 27e70cd9e11b480ab6bbb9b28275f142da7c76ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466681"
---
# <a name="messagetrackingsearchresult"></a>MessageTrackingSearchResult

L’élément **MessageTrackingSearchResult** contient un seul résultat de message pour un élément [FindMessageTrackingReportResponse](findmessagetrackingreportresponse.md) . 
  
```xml
<MessageTrackingSearchResult>
   <Subject/>
   <Sender/>
   <PurportedSender/>
   <Recipients/>
   <SubmittedTime/>
   <MessageTrackingReportId/>
   <PreviousHopServer/>
   <FirstHopServer/>
   <Properties/>
</MessageTrackingSearchResult>
```

 **FindMessageTrackingSearchResultType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Subject](subject.md) <br/> |Contient l’objet du message électronique.  <br/> |
|[Expéditeur (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contient l’adresse de l’expéditeur du message électronique.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contient les informations de contact pour l’expéditeur allégué d’un message électronique.  <br/> |
|[Destinataires (ArrayOfRecipientsType)](recipients-arrayofrecipientstype.md) <br/> |Contient une liste des adresses de messagerie qui ont reçu ce message.  <br/> |
|[SubmittedTime](submittedtime.md) <br/> |Contient l’heure à laquelle le message a été soumis.  <br/> |
|[MessageTrackingReportId](messagetrackingreportid.md) <br/> |Contient un ID interne qui identifie le message dans la base de données de transport.  <br/> |
|[PreviousHopServer](previoushopserver.md) <br/> |Contient le nom du serveur dans la forêt qui a précédemment accepté le message.  <br/> |
|[FirstHopServer](firsthopserver.md) <br/> |Contient le nom du serveur dans la forêt qui a accepté le message en premier.  <br/> |
|[Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’une ou plusieurs propriétés de suivi.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MessageTrackingSearchResults](messagetrackingsearchresults.md) <br/> |Contient une liste de messages qui correspondent aux critères de recherche.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

