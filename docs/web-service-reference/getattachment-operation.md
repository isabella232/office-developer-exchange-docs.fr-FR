---
title: Opération GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: L’opération GetAttachment est utilisée pour récupérer les pièces jointes existantes sur des éléments de la banque d’informations Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756527"
---
# <a name="getattachment-operation"></a>Opération GetAttachment

L’opération GetAttachment est utilisée pour récupérer les pièces jointes existantes sur des éléments de la banque d’informations Exchange.
  
## <a name="getattachment-request-example"></a>Exemple de requête GetAttachment

### <a name="description"></a>Description

L’exemple de requête GetAttachment suivant montre comment obtenir une pièce jointe.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’élément [AttachmentShape](attachmentshape.md) vous permet de vous permet de spécifier les informations de pièce jointe doivent être retournées. Un élément [AttachmentShape](attachmentshape.md) vide est valide et affiche votre les pièces jointes sans contenu MIME des pièces jointes d’élément, avec un type de corps de texte et sans les propriétés supplémentaires. 
  
La collection [AttachmentIds](attachmentids.md) vous permet de spécifier un ou plusieurs identificateurs de pièce jointe à renvoyer. Notez qu’il s’agit du type RequestAttachmentIdType, n’importe quel AttachmentIds que vous recevez **CreateAttachment** doit avoir les attributs **RootItemId** et **RootItemChangeKey** supprimé avant de les transmettre à **GetAttachment**.
  
> [!NOTE]
> L’identificateur de pièce jointe et modifier la clé ont été réduits afin de préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Exemple de réponse GetAttachment

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à une demande GetAttachment. Cet exemple renvoie une pièce jointe.
  
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
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les messages de réponse pour GetAttachment contient toujours la pièce jointe complet ; Autrement dit, toutes les propriétés sera toujours incluses. Pour les pièces jointes, ces propriétés sont [nom (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)et [contenu](content.md). Les pièces jointes d’élément, ces propriétés sont [nom (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) et toutes les propriétés de l’élément, comme si la forme **AllProperties** a été utilisée dans un appel GetItem. L’élément [AttachmentShape](attachmentshape.md) , le cas échéant, permettra une application consommateur demander les propriétés étendues supplémentaires pour les pièces jointes de l’élément. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Pièces jointes](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Nom (AttachmentType)](name-attachmenttype.md)
    
- [Content](content.md)
    
## <a name="see-also"></a>Voir aussi



[Opération CreateAttachment](createattachment-operation.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)

