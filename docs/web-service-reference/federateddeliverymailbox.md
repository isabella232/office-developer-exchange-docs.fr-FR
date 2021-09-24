---
title: FederatedDeliveryMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FederatedDeliveryMailbox
api_type:
- schema
ms.assetid: cd56bcc0-d24a-4e8b-87bd-999bf69234b7
description: L’élément FederatedDeliveryMailbox représente la boîte aux lettres à laquelle un message entre les locaux a été envoyé.
ms.openlocfilehash: 41224f9d630bb0b98b27a2d969ec490c3379eee2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513737"
---
# <a name="federateddeliverymailbox"></a>FederatedDeliveryMailbox

**L’élément FederatedDeliveryMailbox représente** la boîte aux lettres à laquelle un message entre les locaux a été envoyé. 
  
```XML
<FederatedDeliveryMailbox>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</FederatedDeliveryMailbox>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Name (EmailAddressType)](name-emailaddresstype.md) <br/> |Définit le nom de l’utilisateur de la boîte aux lettres. Cet élément est facultatif.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Définit le routage utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Définit le type de boîte aux lettres d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[ItemId](itemid.md) <br/> |Définit l’identificateur d’élément d’un contact ou d’une liste de distribution privée pour les destinataires du dossier Contacts d’un utilisateur. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |Contient des critères pour les types de messages à rechercher.  <br/> |
   
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



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

