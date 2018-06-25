---
title: PendingMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PendingMailTips
api_type:
- schema
ms.assetid: 0cd70eea-8d36-4b1b-bf80-5edf359e7ba7
description: L’élément PendingMailTips indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur.
ms.openlocfilehash: 73d597f6534ea29f7d26d6526c48631251521ae5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828704"
---
# <a name="pendingmailtips"></a>PendingMailTips

L’élément **PendingMailTips** indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur. 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
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
|[Les infos-courrier](mailtips.md) <br/> |Représente les valeurs pour les différents types d’astuces de la messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **PendingMailTips** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Représente tous les conseils de messagerie disponibles.  <br/> |
|OutOfOfficeMessage  <br/> |Représente le message d’absence du bureau (OOF).  <br/> |
|MailboxFullStatus  <br/> |Représente l’état d’une boîte aux lettres en cours complète.  <br/> |
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
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

