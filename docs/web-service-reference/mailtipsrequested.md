---
title: MailTipsRequested
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsRequested
api_type:
- schema
ms.assetid: 8037bbe5-a37f-4f77-8209-27a94f9095ef
description: L’élément MailTipsRequested contient les types de conseils de messagerie demandées à partir du service.
ms.openlocfilehash: fa2bef394ea8473aa65bdc2f1d39c0794186fdc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828348"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

L’élément **MailTipsRequested** contient les types de conseils de messagerie demandées à partir du service. 
  
```XML
<MailTipsRequested/>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetMailTips](getmailtips.md) <br/> |Contient les destinataires et les types de conseils de messagerie à récupérer.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **MailTipsRequested** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Représente tous les conseils de messagerie disponibles.  <br/> |
|OutOfOfficeMessage  <br/> |Représente le message d’absence du bureau (OOF).  <br/> |
|MailboxFullStatus  <br/> |Représente l’état d’une boîte aux lettres est saturée.  <br/> |
|CustomMailTip  <br/> |Représente une info-bulle de messagerie personnalisé.  <br/> |
|ExternalMemberCount  <br/> |Représente le nombre de membres externes.  <br/> |
|TotalMemberCount  <br/> |Représente le nombre de tous les membres.  <br/> |
|MaxMessageSize  <br/> |Représente la taille maximale des messages que le destinataire peut accepter.  <br/> |
|DeliveryRestriction  <br/> |Indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.  <br/> |
|ModerationStatus  <br/> |Indique si le message de l’expéditeur s’être révisé par un modérateur.  <br/> |
|InvalidRecipient  <br/> |Indique si le destinataire n’est pas valide.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

