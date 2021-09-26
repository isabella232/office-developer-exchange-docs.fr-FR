---
title: Opération de GetInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetInboxRules
api_type:
- schema
ms.assetid: b4b2701a-4a23-4acc-8c75-19f7955ad7ae
description: L’opération GetInboxRules utilise Exchange Web Services pour récupérer les règles de boîte de réception dans la boîte aux lettres de l’utilisateur identifié.
ms.openlocfilehash: 3e312ed08494b92c212595d081454b5f2ca6117e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546251"
---
# <a name="getinboxrules-operation"></a>Opération de GetInboxRules

**L’opération GetInboxRules** utilise Exchange Web Services pour récupérer les règles de boîte de réception dans la boîte aux lettres de l’utilisateur identifié. 
  
## <a name="getinboxrules-request-example"></a>Exemple de requête GetInboxRules

### <a name="description"></a>Description

L’exemple suivant montre le XML de requête que le client envoie au serveur. La requête identifie l’utilisateur dans [l’élément MailboxSmtpAddress.](mailboxsmtpaddress.md) Toutes les règles de boîte de réception de l’utilisateur identifié doivent être renvoyées dans la réponse. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetInboxRules>
      <m:MailboxSmtpAddress>User1@Contoso.com</m:MailboxSmtpAddress>
    </m:GetInboxRules>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Éléments de demande

La requête inclut l’élément facultatif suivant :
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
## <a name="successful-getinboxrules-response-example"></a>Exemple de réponse GetInboxRules réussie

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la **demande GetInboxRules.** Dans cet exemple, la réponse inclut une règle. 
  
> [!NOTE]
> Les valeurs de **l’ID et** des attributs **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
        MinorVersion="1" MajorBuildNumber="139"
        MinorBuildNumber="0"
        Version="Exchange2010_SP1"
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetInboxRulesResponse ResponseClass="Success"
        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <OutlookRuleBlobExists>true</OutlookRuleBlobExists>
      <InboxRules>
        <Rule xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <RuleId>dCsAAABjzvA=</RuleId>
          <DisplayName>MoveInterestingToJunk</DisplayName>
          <Priority>1</Priority>
          <IsEnabled>true</IsEnabled>
          <Conditions>
            <ContainsSubjectStrings>
              <String>Interesting</String>
            </ContainsSubjectStrings>
          </Conditions>
          <Actions>
            <MoveToFolder>
              <FolderId ChangeKey="AQAAAA==" Id="AAMkAGYzZjZm" />
            </MoveToFolder>
          </Actions>
        </Rule>
      </InboxRules>
    </GetInboxRulesResponse>
  </s:Body>
</s:Envelope>
```

### <a name="response-elements"></a>Éléments de réponse

Les éléments suivants sont inclus dans la réponse :
  
- [GetInboxRulesResponse](getinboxrulesresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [OutlookRuleBlobExists](outlookruleblobexists.md)
    
- [InboxRules](inboxrules.md)
    
## <a name="see-also"></a>Voir aussi



[Opération de UpdateInboxRules](updateinboxrules-operation.md)

