---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: L’élément FindMessageTrackingReport spécifie les critères pour les types de messages.
ms.openlocfilehash: 77545121aa056992248c045af3f3d36566678b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756410"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

L’élément **FindMessageTrackingReport** spécifie les critères pour les types de messages. 
  
```xml
<FindMessageTrackingReport>
   <Scope/>
   <Domain/>
   <Sender/>
   <PurportedSender/>
   <Recipient/>
   <Subject/>
   <StartDateTime/>
   <EndDateTime/>
   <MessageId/>
   <FederatedDeliveryMailbox/>
   <DiagnosticsLevel/>
   <ServerHint/>
   <Properties/>
</FindMessageTrackingReport>
```

 **FindMessageTrackingReportRequestType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Étendue (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Représente le rapport de suivi des messages l’étendue doivent être.  <br/> |
|[Domaine (le suivi des messages)](domain-message-tracking.md) <br/> |Contient le nom du domaine où le suivi des messages est exécutée.  <br/> |
|[Expéditeur (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contient des informations de contact pour l’expéditeur du message électronique.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contient des informations de contact pour l’expéditeur présumé d’un message électronique.  <br/> |
|[Recipient](recipient.md) <br/> |Contient l’adresse de messagerie du destinataire du message.  <br/> |
|[Objet](subject.md) <br/> |Contient l’objet du message électronique.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Contient la date et l’heure pour la recherche de départ.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Contient la date et l’heure de la recherche.  <br/> |
|[MessageId](messageid.md) <br/> |Contient l’identificateur de message pour la recherche.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Contient le nom de la boîte aux lettres dans laquelle le message cross-site a été envoyé.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Représente le niveau de détail des rapports de diagnostic.  <br/> |
|[ServerHint](serverhint.md) <br/> |Représente le point de départ pour le suivi d’un message dans un site distant ou d’une forêt.  <br/> |
|[Propriétés (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’un ou plusieurs des propriétés de suivi. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

