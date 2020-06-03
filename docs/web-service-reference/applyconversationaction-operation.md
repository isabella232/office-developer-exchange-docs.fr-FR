---
title: Opération de ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: L’opération ApplyConversationAction définit une action de suivi unique ou ponctuelle sur tous les éléments d’une conversation. L’opération ApplyConversationAction vous permet de classer, déplacer, copier, supprimer et définir l’état de lecture sur tous les éléments d’une conversation. Les actions peuvent également être définies pour les nouveaux messages d’une conversation.
ms.openlocfilehash: cdab239a5b0b1406d2ce31f4604e4737d037cd7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463502"
---
# <a name="applyconversationaction-operation"></a>Opération de ApplyConversationAction

L’opération **ApplyConversationAction** définit une action de suivi unique ou ponctuelle sur tous les éléments d’une conversation. L’opération **ApplyConversationAction** vous permet de classer, déplacer, copier, supprimer et définir l’état de lecture sur tous les éléments d’une conversation. Les actions peuvent également être définies pour les nouveaux messages d’une conversation. 
  
## <a name="applyconversationaction-request-example"></a>Exemple de requête ApplyConversationAction

### <a name="description"></a>Description

L’exemple de requête **ApplyConversationAction** suivant montre comment déplacer les éléments de la conversation spécifiée dans un autre dossier. Les éléments ajoutés à la conversation seront également déplacés vers le dossier spécifié. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a>Remarques

Les identificateurs de dossier et de conversation ont été raccourcis pour conserver la lisibilité.
  
## <a name="applyconversationaction-response-example"></a>Exemple de réponse ApplyConversationAction

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à une demande **ApplyConversationAction** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Conversations in EWS](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

