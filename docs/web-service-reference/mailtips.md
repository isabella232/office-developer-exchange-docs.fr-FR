---
title: MailTips
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
description: L’élément infos-courrier représente les valeurs de différents types de conseils de courrier.
ms.openlocfilehash: 9bacdea7b4f3108f700ed102025445e01a73e69d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447595"
---
# <a name="mailtips"></a>MailTips

L’élément **infos-courrier** représente les valeurs de différents types de conseils de courrier. 
  
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

 **Infos-courrier**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[RecipientAddress](recipientaddress.md) <br/> |Représente la boîte aux lettres du destinataire.  <br/> |
|[PendingMailTips](pendingmailtips.md) <br/> |Indique que les conseils de messagerie de cet élément n’ont pas pu être évalués avant l’expiration du délai de traitement du serveur.  <br/> |
|[OutOfOffice](outofoffice.md) <br/> |Représente le message de réponse et la durée d’envoi du message de réponse.  <br/> |
|[MailboxFull](mailboxfull.md) <br/> |Indique si la boîte aux lettres du destinataire est complète.  <br/> |
|[CustomMailTip](custommailtip.md) <br/> |Représente un message personnalisé de Conseil de messagerie.  <br/> |
|[TotalMemberCount](totalmembercount.md) <br/> |Représente le décompte de tous les membres d’un groupe.  <br/> |
|[ExternalMemberCount](externalmembercount.md) <br/> |Représente le nombre de membres externes d’un groupe.  <br/> |
|[MaxMessageSize](maxmessagesize.md) <br/> |Représente la taille maximale des messages que le destinataire peut accepter.  <br/> |
|[DeliveryRestricted](deliveryrestricted.md) <br/> |Indique si les restrictions de remise empêchent le message de l’expéditeur d’atteindre le destinataire.  <br/> |
|[IsModerated](ismoderated.md) <br/> |Indique si la boîte aux lettres du destinataire est modérée.  <br/> |
|[InvalidRecipient (infos-courrier)](invalidrecipient-mailtips.md) <br/> |Indique si le destinataire n’est pas valide.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailTipsResponseMessageType](mailtipsresponsemessagetype.md) <br/> |Représente les paramètres des conseils de messagerie.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
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

