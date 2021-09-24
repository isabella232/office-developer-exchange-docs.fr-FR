---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: L’élément GetPasswordExpirationDate définit une demande d’obtenir la date d’expiration du mot de passe d’un compte de messagerie. Cet élément est l’élément de base pour l’opération d’opération GetPasswordExpirationDate.
ms.openlocfilehash: e5c74cc773438780fad0448cd2ae449dae07738f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520513"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

**L’élément GetPasswordExpirationDate** définit une demande d’obtenir la date d’expiration du mot de passe d’un compte de messagerie. Cet élément est l’élément de base pour [l’opération d’opération GetPasswordExpirationDate.](getpasswordexpirationdate-operation.md) 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Nom de l'élément**|**Description**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Représente l’adresse e-mail du compte de messagerie pour lequel la date d’expiration du mot de passe doit être renvoyée.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 2 (SP2).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

