---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: L’élément MessageTrackingReport contient un seul message est retourné dans une opération GetMessageTrackingReport.
ms.openlocfilehash: d01e0fbf099d096c7f255a8e94070e330577e6ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828457"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

L’élément **MessageTrackingReport** contient un seul message est retourné dans une [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).
  
```XML
<MessageTrackingReport>
   <Sender/>
   <PurportedSender/>
   <Subject/>
   <SubmitTime/>
   <OriginalRecipients/>
   <RecipientTrackingEvents/>
   <Properties/>
</MessageTrackingReport>
```

 **MessageTrackingReportType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Expéditeur (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contient des informations de contact pour l’expéditeur du message électronique.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contient des informations de contact pour l’expéditeur présumé d’un message électronique.  <br/> |
|[Objet](subject.md) <br/> |Contient l’objet du message électronique.  <br/> |
|[SubmitTime](submittime.md) <br/> |Indique l’heure du jour à laquelle le message électronique a été envoyé.  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |Contient une liste des destinataires du message électronique.  <br/> |
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contient une liste d’un ou plusieurs événements de suivi pour les destinataires.  <br/> |
|[Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’un ou plusieurs des propriétés de suivi.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contient le résultat d’une seule demande [d’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

