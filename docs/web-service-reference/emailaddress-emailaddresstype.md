---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: L’élément EmailAddress spécifie l’adresse SMTP entièrement résolue pour la boîte aux lettres de site ou le personnage associé.
ms.openlocfilehash: 76b279a82f6f277d9f231866437359ceae46df59
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545257"
---
# <a name="emailaddress-emailaddresstype"></a>EmailAddress (EmailAddressType)

**L’élément EmailAddress** spécifie l’adresse SMTP entièrement résolue pour la boîte aux lettres de site ou le personnage associé. 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Name (String)](name-string.md) <br/> |Spécifie un nom ou une clé d’affinement de recherche ou le nom d’un utilisateur de messagerie.  <br/> |
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP principale d’un utilisateur de boîte aux lettres.  <br/> |
|[RoutingType (EmailAddressType)](routingtype-emailaddresstype.md) <br/> |Spécifie le type de routage d’une adresse de messagerie.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Représente le type de boîte aux lettres représenté par l’adresse de messagerie.  <br/> |
|[ItemId](itemid.md) <br/> |Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Persona](persona.md) <br/> |Spécifie un ensemble de données de personnage renvoyées par une **demande GetPersona.**  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
**L’élément EmailAddress** s’applique aux clients qui ciblent Exchange Online et les versions de Microsoft Exchange Server à partir de Exchange 2013. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

