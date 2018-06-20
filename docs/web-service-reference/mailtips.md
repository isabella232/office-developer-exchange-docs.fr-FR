---
title: Les infos-courrier
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTips
api_type:
- schema
ms.assetid: c1cba493-bccc-4b8e-be8e-bfa8a8b10882
description: L’élément Infos-courrier représente les valeurs pour les différents types d’astuces de la messagerie.
ms.openlocfilehash: 3a2e95225b09fd2d81db32f821ea3069ab7e7852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828311"
---
# <a name="mailtips"></a>Les infos-courrier

L’élément **Infos-courrier** représente les valeurs pour les différents types d’astuces de la messagerie. 
  
```XML
<MailTips>
   <RecipientAddress/>
   <PendingMailTips/>
   <OutOfOffice/>
   <MailboxFull/>
   <CustomMailTip/>
   <TotalMemberCount/>
   <ExternalMemberCount/>
   <MaxMessageSize/>
   <DeliveryRestricted/>
   <IsModerated/>
   <InvalidRecipient/>
</MailTips>
```

 **Les infos-courrier**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Représente la boîte aux lettres du destinataire.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Indique que les conseils de messagerie de cet élément ne peuvent pas être évaluées avant l’expiration du délai d’attente de traitement du serveur.  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Représente le message de réponse et un délai d’expiration pour l’envoi du message de réponse.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Indique si la boîte aux lettres du destinataire est complète.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Représente un message d’info-bulle personnalisée.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Représente le nombre de tous les membres d’un groupe.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Représente le nombre de membres externes dans un groupe.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Représente la taille maximale des messages que le destinataire peut accepter.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Indique si les restrictions de remise empêche le message de l’expéditeur d’atteindre le destinataire.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Indique si la boîte aux lettres du destinataire est en cours modéré.  <br/> |
|[InvalidRecipient (Infos-courrier)](invalidrecipient-mailtips.md) <br/> |Indique si le destinataire n’est pas valide.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Représente les paramètres de conseils de messagerie.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

