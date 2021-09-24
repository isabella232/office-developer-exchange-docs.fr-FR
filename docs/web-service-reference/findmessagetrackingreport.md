---
title: FindMessageTrackingReport
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindMessageTrackingReport
api_type:
- schema
ms.assetid: 7ca6e2f7-aae1-4920-b839-73513ba8d4d8
description: L’élément FindMessageTrackingReport spécifie des critères pour les types de messages à rechercher.
ms.openlocfilehash: ec2ab16c6649d85edd86b9438e00ea7cfb9841ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513688"
---
# <a name="findmessagetrackingreport"></a>FindMessageTrackingReport

**L’élément FindMessageTrackingReport** spécifie des critères pour les types de messages à rechercher. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Étendue (NonEmptyStringType)](scope-nonemptystringtype.md) <br/> |Représente l’étendue du rapport de suivi des messages.  <br/> |
|[Domain (Message Tracking)](domain-message-tracking.md) <br/> |Contient le nom du domaine dans lequel le suivi des messages est exécuté.  <br/> |
|[Sender (EmailAddressType)](sender-emailaddresstype.md) <br/> |Contient les informations de contact de l’expéditeur du message électronique.  <br/> |
|[PurportedSender](purportedsender.md) <br/> |Contient les informations de contact de l’expéditeur supposé d’un message électronique.  <br/> |
|[Destinataire](recipient.md) <br/> |Contient l’adresse de messagerie du destinataire du message.  <br/> |
|[Sujet](subject.md) <br/> |Contient l’objet du message électronique.  <br/> |
|[StartDateTime](startdatetime.md) <br/> |Contient la date et l’heure de début de la recherche.  <br/> |
|[EndDateTime](enddatetime.md) <br/> |Contient la date et l’heure de fin de la recherche.  <br/> |
|[MessageId](messageid.md) <br/> |Contient l’identificateur de message pour la recherche.  <br/> |
|[FederatedDeliveryMailbox](federateddeliverymailbox.md) <br/> |Contient le nom de la boîte aux lettres dans laquelle le message entre les locaux a été envoyé.  <br/> |
|[DiagnosticsLevel](diagnosticslevel.md) <br/> |Représente le niveau de détail des rapports de diagnostic.  <br/> |
|[ServerHint](serverhint.md) <br/> |Représente le point de départ pour le suivi d’un message dans un site distant ou une forêt.  <br/> |
|[Properties (ArrayOfTrackingPropertiesType)](properties-arrayoftrackingpropertiestype.md) <br/> |Contient une liste d’une ou plusieurs propriétés de suivi. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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



[Opération FindMessageTrackingReport](findmessagetrackingreport-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

