---
title: Opération UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. UpdateInboxRules est utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception ou pour supprimer une règle de boîte de réception.
ms.openlocfilehash: 08f46219bcb01f5f1c9d69cfaa8b4934e82ff5bd
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510714"
---
# <a name="updateinboxrules-operation"></a>Opération UpdateInboxRules

L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. **UpdateInboxRules est** utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception ou pour supprimer une règle de boîte de réception. 
  
Lorsque vous utilisez **l’opération UpdateInboxRules,** Exchange Web Services supprime les règles d’envoi côté client. Les règles d’envoi côté client sont stockées sur le client dans le message FAI (Folder Associated Information) de la règle et en de toute autre nature. EWS supprime ce message FAI de règle par défaut, en fonction des attentes Outlook le recréera. Toutefois, Outlook ne peut pas recréer des règles qui n’existent pas également en tant que règle étendue, et les règles d’envoi côté client n’existent pas en tant que règles étendues. Par conséquent, ces règles sont perdues. Nous vous suggérons d’y penser lors de la conception de votre solution. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Exemple de requête UpdateInboxRules (Créer une règle)

Vous pouvez utiliser Exchange Web Services pour créer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans Exchange store. Utilisez [l’élément UpdateInboxRules](updateinboxrules.md) conjointement avec [l’élément CreateRuleOperation](createruleoperation.md) pour créer une règle. 
  
### <a name="description"></a>Description

Le client construit le XML de demande et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:CreateRuleOperation>
            <t:Rule>
              <t:DisplayName>MoveInterestingToJunk</t:DisplayName>
              <t:Priority>1</t:Priority>
              <t:IsEnabled>true</t:IsEnabled>
              <t:Conditions>
                <t:ContainsSubjectStrings>
                  <t:String>Interesting</t:String>
                </t:ContainsSubjectStrings>
              </t:Conditions>
              <t:Exceptions />
              <t:Actions>
                <t:MoveToFolder>
                  <t:DistinguishedFolderId Id="junkemail" />
                </t:MoveToFolder>
              </t:Actions>
            </t:Rule>
          </t:CreateRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Commentaires

Cet exemple crée une règle qui déplace un message électronique vers le dossier Courrier indésirable si l’objet du message électronique contient une chaîne égale à « Interesting ».
  
### <a name="request-elements"></a>Éléments de demande

La **demande UpdateInboxRules** inclut les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[L’élément Operations](operations.md) contient [l’élément CreateRuleOperation](createruleoperation.md) pour créer une règle. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Exemple de réponse UpdateInboxRules (Créer une règle)

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui crée une règle. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Exemple de requête UpdateInboxRules (Définir la règle)

Vous pouvez utiliser Exchange Web Services web pour modifier une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans Exchange store. Utilisez [l’élément UpdateInboxRules](updateinboxrules.md) conjointement avec l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle. 
  
### <a name="description"></a>Description

Le client construit le XML de demande et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <Rule>
              <RuleId>Nh8AAAAwW/w=</RuleId>
              <DisplayName>(Modified) This is Junk</DisplayName>
              <Priority>1</Priority>
              <IsEnabled>true</IsEnabled>
              <Conditions>
                <ContainsSubjectStrings>
                  <String>Interesting</String>
                </ContainsSubjectStrings>
              </Conditions>
              <Actions>
                <MoveToFolder>
                  <FolderId Id="AAMkADQ1YTE1" ChangeKey="AQAAAA==" />
                </MoveToFolder>
              </Actions>
            </Rule>
          </SetRuleOperation>
        </Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Commentaires

Cet exemple modifie le nom complet en « (Modified) This is Junk ».
  
> [!NOTE]
> Les valeurs des **attributs Id** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité. 
  
### <a name="request-elements"></a>Éléments de demande

La **demande UpdateInboxRules** inclut les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[L’élément Operations](operations.md) contient [l’élément SetRuleOperation](setruleoperation.md) pour modifier une règle. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Exemple de réponse UpdateInboxRules (Définir la règle)

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui modifie une règle. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Exemple de requête UpdateInboxRules (Règle de suppression)

Vous pouvez utiliser Exchange Web Services pour supprimer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans Exchange store. Utilisez [UpdateInboxRules conjointement](updateinboxrules.md) avec [l’élément DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle. 
  
### <a name="description"></a>Description

Le client construit le XML de demande et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <m:Operations>
          <t:DeleteRuleOperation>
            <t:RuleId>Nh8AAAAwW/U=</t:RuleId>
          </t:DeleteRuleOperation>
        </m:Operations>
      </m:UpdateInboxRules>
  </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a>Commentaires

Cet exemple supprime la règle identifiée existante.
  
### <a name="request-elements"></a>Éléments de demande

La **demande UpdateInboxRules** inclut les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Operations](operations.md)
    
[L’élément Operations](operations.md) contient [l’élément DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Exemple de réponse UpdateInboxRules (Règle de suppression)

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **UpdateInboxRules** qui supprime une règle. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" 
        Version="Exchange2010_SP1" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>Voir aussi



[Opération de GetInboxRules](getinboxrules-operation.md)

