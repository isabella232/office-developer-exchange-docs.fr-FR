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
description: L’élément MailTipsRequested contient les types de conseils de messagerie demandés par le service.
ms.openlocfilehash: bcb2ebf15e628a04e8507f938d385cf113f2f2a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465897"
---
# <a name="mailtipsrequested"></a>MailTipsRequested

L’élément **MailTipsRequested** contient les types de conseils de messagerie demandés par le service. 
  
```XML
<MailTipsRequested/>
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
|[GetMailTips](getmailtips.md) <br/> |Contient les destinataires et les types de conseils de messagerie à récupérer.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **MailTipsRequested** . 
  
|**Valeur**|**Description**|
|:-----|:-----|
|Tous  <br/> |Représente tous les conseils de courrier disponibles.  <br/> |
|OutOfOfficeMessage  <br/> |Représente le message absent (e) du bureau.  <br/> |
|MailboxFullStatus  <br/> |Représente l’état d’une boîte aux lettres qui est saturée.  <br/> |
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
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

