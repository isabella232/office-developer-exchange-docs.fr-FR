---
title: Opération UpdateInboxRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRules
api_type:
- schema
ms.assetid: f982a237-471e-45c5-a2b5-468cfc53150b
description: L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. UpdateInboxRules est utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception, ou pour supprimer une règle de boîte de réception.
ms.openlocfilehash: 6e979421d619fed6625fe05db86c1f8c6a7418c9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838879"
---
# <a name="updateinboxrules-operation"></a>Opération UpdateInboxRules

L’opération UpdateInboxRules met à jour les règles de boîte de réception de l’utilisateur authentifié en appliquant les opérations spécifiées. **UpdateInboxRules** est utilisé pour créer une règle de boîte de réception, pour définir une règle de boîte de réception, ou pour supprimer une règle de boîte de réception. 
  
Lorsque vous utilisez l’opération **UpdateInboxRules** , Services Web Exchange supprime les règles d’envoi côté client. Règles d’envoi côté client sont stockées sur le client dans la règle de Message dossier associé informations (FAI) et nulle part ailleurs. EWS supprime cette règle message FAI par défaut, en fonction de l’attente qu’Outlook va le recréer. Toutefois, Outlook ne peut pas recréer les règles qui n’existent pas également en tant qu’une règle d’étendue, et les règles côté client send n’existent pas sous forme de règles d’étendue. Par conséquent, ces règles sont perdues. Nous vous suggérons Voici lors de la conception de votre solution. 
  
## <a name="updateinboxrules-create-rule-request-example"></a>Exemple de requête UpdateInboxRules (créer une règle)

Vous pouvez utiliser les Services Web Exchange pour créer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange. Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle. 
  
### <a name="description"></a>Description

Le client construit la requête XML et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Cet exemple crée une règle qui va déplacer un message électronique dans le dossier courrier indésirable si l’objet du message électronique contient une chaîne qui est égale à « Intéressant ».
  
### <a name="request-elements"></a>Éléments de la demande

La demande **UpdateInboxRules** comprend les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Opérations](operations.md)
    
L’élément [opérations](operations.md) contient l’élément [CreateRuleOperation](createruleoperation.md) pour créer une règle. 
  
## <a name="updateinboxrules-create-rule-response-example"></a>Exemple de réponse UpdateInboxRules (créer une règle)

### <a name="description"></a>Description

L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui crée une règle. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
        MinorVersion="1" 
        MajorBuildNumber="139" 
        MinorBuildNumber="0" Version="Exchange2010_SP1" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
         ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-set-rule-request-example"></a>Exemple de requête UpdateInboxRules (définir les règles)

Vous pouvez utiliser les Services Web Exchange pour modifier une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange. Utilisez l’élément [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle. 
  
### <a name="description"></a>Description

Le client construit la requête XML et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
      <m:UpdateInboxRules>
        <m:RemoveOutlookRuleBlob>true</m:RemoveOutlookRuleBlob>
        <Operations xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
          <SetRuleOperation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

Cet exemple modifie le nom complet « (modifié) il s’agit indésirable ».
  
> [!NOTE]
> Les valeurs de l' **Id** et les attributs de l’élément [FolderId](folderid.md) **ChangeKey** ont été raccourcies pour des raisons de lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

La demande **UpdateInboxRules** comprend les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Opérations](operations.md)
    
L’élément [opérations](operations.md) contient l’élément [SetRuleOperation](setruleoperation.md) pour modifier une règle. 
  
## <a name="updateinboxrules-set-rule-response-example"></a>Exemple de réponse UpdateInboxRules (définir les règles)

### <a name="description"></a>Description

L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui modifie une règle. 
  
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
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse 
          ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="updateinboxrules-delete-rule-request-example"></a>Exemple de requête UpdateInboxRules (supprimer la règle)

Vous pouvez utiliser les Services Web Exchange pour supprimer une règle de boîte de réception dans la boîte aux lettres d’un utilisateur dans la banque d’informations Exchange. Utiliser [UpdateInboxRules](updateinboxrules.md) en association avec l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle. 
  
### <a name="description"></a>Description

Le client construit la requête XML et l’envoie au serveur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Cet exemple supprime la règle existante identifiée.
  
### <a name="request-elements"></a>Éléments de la demande

La demande **UpdateInboxRules** comprend les éléments suivants : 
  
- [MailboxSmtpAddress](mailboxsmtpaddress.md)
    
- [RemoveOutlookRuleBlob](removeoutlookruleblob.md)
    
- [Opérations](operations.md)
    
L’élément [opérations](operations.md) contient l’élément [DeleteRuleOperation](deleteruleoperation.md) pour supprimer une règle. 
  
## <a name="updateinboxrules-delete-rule-response-example"></a>Exemple de réponse UpdateInboxRules (supprimer la règle)

### <a name="description"></a>Description

L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **UpdateInboxRules** qui supprime une règle. 
  
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
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <UpdateInboxRulesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </UpdateInboxRulesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateInboxRulesResponse](updateinboxrulesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="see-also"></a>Voir aussi



[Opération de GetInboxRules](getinboxrules-operation.md)

