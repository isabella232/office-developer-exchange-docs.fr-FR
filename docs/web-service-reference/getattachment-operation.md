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
description: L’opération GetAttachment est utilisée pour récupérer des pièces jointes existantes sur des éléments de la Banque d’Exchange.
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461288"
---
# <a name="getattachment-operation"></a>Opération GetAttachment

L’opération GetAttachment est utilisée pour récupérer des pièces jointes existantes sur des éléments de la Banque d’Exchange.
  
## <a name="getattachment-request-example"></a>Exemple de requête GetAttachment

### <a name="description"></a>Description

L’exemple de requête GetAttachment suivant montre comment obtenir une pièce jointe.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

L’élément [AttachmentShape](attachmentshape.md) vous permet de spécifier les informations de pièce jointe à renvoyer. Un élément [AttachmentShape](attachmentshape.md) vide est valide et affiche vos pièces jointes sans contenu MIME pour les pièces jointes d’éléments, avec un type de corps de texte et sans propriétés supplémentaires. 
  
La collection [AttachmentIds](attachmentids.md) vous permet de spécifier un ou plusieurs identificateurs de pièce jointe à renvoyer. Notez que ces éléments sont de type RequestAttachmentIdType, de sorte que les AttachmentIds que vous recevez de **CreateAttachment** doivent être supprimés des attributs **RootItemId** et **RootItemChangeKey** avant de les transmettre à **GetAttachment**.
  
> [!NOTE]
> L’identificateur de pièce jointe et la clé de modification ont été raccourcies afin de préserver la lisibilité. 
  
### <a name="request-elements"></a>Demander des éléments

Les éléments suivants sont utilisés dans la demande :
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Exemple de réponse GetAttachment

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à une demande GetAttachment. Cet exemple renvoie une pièce jointe de fichier.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Les messages de réponse pour GetAttachment contiennent toujours la pièce jointe complète ; autrement dit, toutes les propriétés sont toujours incluses. Pour les pièces jointes, ces propriétés sont [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [contentid](contentid.md), [ContentLocation](contentlocation.md)et [content](content.md). Pour les pièces jointes d’éléments, ces propriétés sont [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [contentid](contentid.md), [ContentLocation](contentlocation.md) et toutes les propriétés de l’élément, comme si la forme **AllProperties** avait été utilisée dans un appel de GetItem. L’élément [AttachmentShape](attachmentshape.md) , s’il est présent, permet à une application consommateur de demander des propriétés étendues supplémentaires pour les pièces jointes d’éléments. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Attachments](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Nom (AttachmentType)](name-attachmenttype.md)
    
- [Content](content.md)
    
## <a name="see-also"></a>Voir aussi



[Opération CreateAttachment](createattachment-operation.md)
  
[Opération DeleteAttachment](deleteattachment-operation.md)

