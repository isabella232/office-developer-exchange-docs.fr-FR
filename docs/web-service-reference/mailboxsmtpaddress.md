---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: L’élément MailboxSmtpAddress représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception sont à récupérer ou mis à jour ; ou dont la date d’expiration de mot de passe doit être récupéré.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828303"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

L’élément **MailboxSmtpAddress** représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception sont à récupérer ou mis à jour ; ou dont la date d’expiration de mot de passe doit être récupéré. 
  
```XML
<MailboxSmtpAddress/>
```

**string**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Définit une requête pour obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin du serveur.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Définit une demande pour obtenir la date d’expiration de mot de passe d’un compte de messagerie.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Définit une demande pour mettre à jour les règles de boîte de réception dans une boîte aux lettres dans le magasin du serveur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

L’élément **MailboxSmtpAddress** est un élément facultatif. Si l’élément **MailboxSmtpAddress** est omis, l’adresse de l’utilisateur connecté est utilisé. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de GetInboxRules](getinboxrules-operation.md)
- [Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Opération de UpdateInboxRules](updateinboxrules-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

