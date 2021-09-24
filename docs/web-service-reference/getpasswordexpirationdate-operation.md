---
title: Opération GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: b0297458-58fb-4e5d-bb47-0cd17155e106
description: L’opération GetPasswordExpirationDate fournit la date d’expiration du mot de passe du compte de messagerie pour l’utilisateur actuel.
ms.openlocfilehash: 07928fd3e6fca410a292d6cd74f1240d8e81c42f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524237"
---
# <a name="getpasswordexpirationdate-operation"></a>Opération GetPasswordExpirationDate

**L’opération GetPasswordExpirationDate** fournit la date d’expiration du mot de passe du compte de messagerie pour l’utilisateur actuel. 
  
Cette opération a été introduite dans Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="getpasswordexpirationdate-operation-soap-headers"></a>En-têtes SOAP de l’opération GetPasswordExpirationDate

**L’opération GetPasswordExpirationDate** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture, telle que définie dans la RFC 3066, « Balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres. Ceci s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie le schéma de la demande d’opération. Ceci s’applique à une demande. Ceci s’applique à une demande.  <br/> |
   
## <a name="getpasswordexpirationdate-operation-request-example"></a>Exemple de demande d’opération GetPasswordExpirationDate

### <a name="description"></a>Description

L’exemple suivant d’une demande d’opération **GetPasswordExpirationDate** montre comment obtenir la date d’expiration du mot de passe d’un compte de messagerie. 
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
  </soap:Header>
  <soap:Body>
    <tns:GetPasswordExpirationDate>
      <tns:MailboxSmtpAddress>user1@DTZMZX-dom.extest.microsoft.com</tns:MailboxSmtpAddress>
    </tns:GetPasswordExpirationDate>
  </soap:Body>
</soap:Envelope>

```

### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [GetPasswordExpirationDate](getpasswordexpirationdate.md)
    
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getpasswordexpirationdate-operation-response"></a>Réponse de l’opération GetPasswordExpirationDate réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [GetPasswordExpirationDateResponse](getpasswordexpirationdateresponse.md)
    
- [PasswordExpirationDate](passwordexpirationdate.md)
    

