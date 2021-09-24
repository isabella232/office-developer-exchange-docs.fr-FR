---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: L’élément MailboxSmtpAddress représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception doivent être récupérées ou mises à jour ; ou dont la date d’expiration du mot de passe doit être récupérée.
ms.openlocfilehash: 86a39c416b9674e1f48f0a75508c003ad9d620f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511130"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

**L’élément MailboxSmtpAddress** représente l’adresse SMTP de l’utilisateur dont les règles de boîte de réception doivent être récupérées ou mises à jour ; ou dont la date d’expiration du mot de passe doit être récupérée. 
  
```XML
<MailboxSmtpAddress/>
```

**chaîne**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Définit une demande d’obtenir les règles de boîte de réception sur une boîte aux lettres dans le magasin de serveurs.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Définit une demande d’obtenir la date d’expiration du mot de passe d’un compte de messagerie.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Définit une demande de mise à jour des règles de boîte de réception dans une boîte aux lettres du magasin de serveurs.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

**L’élément MailboxSmtpAddress** est un élément facultatif. Si **l’élément MailboxSmtpAddress est** omis, l’adresse de l’utilisateur connecté est utilisée. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération de GetInboxRules](getinboxrules-operation.md)
- [Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Opération de UpdateInboxRules](updateinboxrules-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

