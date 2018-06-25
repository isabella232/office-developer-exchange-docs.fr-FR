---
title: Opération GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: L’opération GetPasswordExpirationDate fournit la date d’expiration de messagerie compte le mot de passe pour l’utilisateur actuel.
ms.openlocfilehash: c57942c88b09a910e2d529a12ea279bb2da5d693
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756700"
---
# <a name="getpasswordexpirationdate-operation"></a>Opération GetPasswordExpirationDate

L’opération **GetPasswordExpirationDate** fournit la date d’expiration de messagerie compte le mot de passe pour l’utilisateur actuel. 
  
Cette opération a été introduite dans Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>En-têtes SOAP GetPasswordExpirationDate opération

L’opération **GetPasswordExpirationDate** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres. Ceci s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie le schéma de la requête d’opération. Ceci s’applique à une demande. Ceci s’applique à une demande.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Exemple de requête d’opération GetPasswordExpirationDate

### <a name="description"></a>Description

Une demande d’opération **GetPasswordExpirationDate** l’exemple suivant montre comment obtenir la date d’expiration de mot de passe pour un compte de messagerie. 
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Réponse d’opération GetPasswordExpirationDate réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

