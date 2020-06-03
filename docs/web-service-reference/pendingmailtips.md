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
description: L’élément PendingMailTips indique que les conseils de messagerie de cet élément n’ont pas pu être évalués avant l’expiration du délai de traitement du serveur.
ms.openlocfilehash: 715d68b367c3b7251c7406c10c1ec52dcd992a59
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529965"
---
# <a name="pendingmailtips"></a>PendingMailTips

L’élément **PendingMailTips** indique que les conseils de messagerie de cet élément n’ont pas pu être évalués avant l’expiration du délai de traitement du serveur. 
  
```XML
<PendingMailTips>All | OutOfOfficeMessage | MailboxFullStatus | CustomMailTip | ExternalMemberCount | TotalMemberCount | MaxMessageSize | DeliveryRestriction | ModerateStatus | InvalidRecipient</PendingMailTips>
```

 **MailTipTypes**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Infos-courrier](mailtips.md) <br/> |Représente les valeurs de différents types de conseils de courrier.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **PendingMailTips** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Représente tous les conseils de courrier disponibles.  <br/> |
|OutOfOfficeMessage  <br/> |Représente le message absent (e) du bureau.  <br/> |
|MailboxFullStatus  <br/> |Représente l’état d’une boîte aux lettres en cours de remplissage.  <br/> |
|CustomMailTip  <br/> |Représente une info-bulle personnalisée.  <br/> |
|ExternalMemberCount  <br/> |Représente le nombre de membres externes.  <br/> |
|TotalMemberCount  <br/> |Représente le décompte de tous les membres.  <br/> |
|MaxMessageSize  <br/> |Représente la taille maximale des messages qu’un destinataire peut accepter.  <br/> |
|DeliveryRestriction  <br/> |Indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.  <br/> |
|ModerationStatus  <br/> |Indique si le message de l’expéditeur est examiné par un modérateur.  <br/> |
|InvalidRecipient  <br/> |Indique si le destinataire n’est pas valide.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

