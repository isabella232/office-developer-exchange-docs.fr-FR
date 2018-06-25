---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: L’élément GetPasswordExpirationDate définit une demande pour obtenir la date d’expiration de mot de passe pour un compte de messagerie. Cet élément est l’élément de base pour l’opération GetPasswordExpirationDate.
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756703"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

L’élément **GetPasswordExpirationDate** définit une demande pour obtenir la date d’expiration de mot de passe pour un compte de messagerie. Cet élément est l’élément de base pour l’opération [GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) . 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Nom de l'élément**|**Description**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Représente l’adresse de messagerie du compte de messagerie pour lequel la date d’expiration de mot de passe doit être retourné.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

