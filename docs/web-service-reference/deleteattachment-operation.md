---
title: Opération DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: L’opération DeleteAttachment est utilisée pour supprimer le fichier et élément de pièces jointes à partir d’un élément existant dans la banque d’informations Exchange.
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755848"
---
# <a name="deleteattachment-operation"></a>Opération DeleteAttachment

L’opération DeleteAttachment est utilisée pour supprimer le fichier et élément de pièces jointes à partir d’un élément existant dans la banque d’informations Exchange.
  
## <a name="remarks"></a>Remarques

Cette opération vous permet de supprimer une ou plusieurs pièces jointes par ID.
  
## <a name="deleteattachment-request-example"></a>Exemple de requête DeleteAttachment

### <a name="description"></a>Description

Une demande DeleteAttachment l’exemple suivant montre comment supprimer la pièce jointe d’un élément.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Identificateur de pièce jointe a été raccourcie afin de préserver la lisibilité.
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>Exemple de réponse DeleteAttachment

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à une demande DeleteAttachment.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’opération CreateAttachment renvoie un élément de type AttachmentIdType qui inclut un **RootItemId** et le **RootItemChangeKey**. Ces attributs ne sont pas autorisés pour les identificateurs dans une demande DeleteAttachment. DeleteAttachment utilise des éléments de type RequestAttachmentIdType, qui n’inclut pas ces attributs.
  
La réponse DeleteAttachment inclut l’ID de l’élément parent. Lorsque les pièces jointes sont supprimés d’un élément, modifier la clé de l’élément est modifiée. La nouvelle clé de modification d’élément peut être obtenue à partir de la réponse DeleteAttachment.
  
> [!NOTE]
> L’identificateur [RootItemId](rootitemid.md) et ChangeKey ont été réduite afin de préserver la lisibilité. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteAttachmentResponse](deleteattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootItemId](rootitemid.md)
    
## <a name="see-also"></a>Voir aussi

- [Opération CreateAttachment](createattachment-operation.md) 
- [Opération GetAttachment](getattachment-operation.md)

