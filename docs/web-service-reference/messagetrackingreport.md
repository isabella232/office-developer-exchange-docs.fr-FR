---
title: MessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MessageTrackingReport
api_type:
- schema
ms.assetid: 2740bcf6-f86d-4756-a0f2-24ed6e9b75f7
description: L’élément MessageTrackingReport contient un seul message qui est renvoyé dans une opération GetMessageTrackingReport.
ms.openlocfilehash: aa55bb9e4f81a4cc0586d7258720aefd743923fd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539352"
---
# <a name="messagetrackingreport"></a>MessageTrackingReport

**L’élément MessageTrackingReport** contient un seul message qui est renvoyé dans une [opération GetMessageTrackingReport](getmessagetrackingreport-operation.md).
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contient les informations de contact de l’expéditeur du message électronique.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contient les informations de contact de l’expéditeur supposé d’un message électronique.  <br/> |
|[Sujet](subject.md) <br/> |Contient l’objet du message électronique.  <br/> |
|[SubmitTime](submittime.md) <br/> |Contient l’heure de la journée à l’envoi du message électronique.  <br/> |
|[OriginalRecipients](originalrecipients.md) <br/> |Contient la liste des destinataires du message électronique.  <br/> |
|[RecipientTrackingEvents](recipienttrackingevents.md) <br/> |Contient une liste d’un ou plusieurs événements de suivi pour les destinataires.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’une ou plusieurs propriétés de suivi.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetMessageTrackingReportResponse](getmessagetrackingreportresponse.md) <br/> |Contient le résultat d’une [demande d’opération GetMessageTrackingReport](getmessagetrackingreport-operation.md) unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)
  
[Opération de GetMessageTrackingReport](getmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
  
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

