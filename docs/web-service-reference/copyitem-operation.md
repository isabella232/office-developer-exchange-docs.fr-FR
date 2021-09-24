---
title: Opération CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: L’opération CopyItem copie les éléments et les place dans un autre dossier.
ms.openlocfilehash: 62785d9acb784bcffe7d3279de8a80abc803adf4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518644"
---
# <a name="copyitem-operation"></a>Opération CopyItem

**L’opération CopyItem** copie les éléments et les place dans un autre dossier. 
  
## <a name="copyitem-request-example"></a>Exemple de requête CopyItem

### <a name="description"></a>Description

L’exemple suivant **d’une requête CopyItem** montre comment former une demande de copie d’un élément dans la boîte de réception. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

> [!NOTE]
> L’ID de dossier et la touche de modification ont été raccourcis pour préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [CopyItem](copyitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur exécutant Microsoft Exchange Server 2010 sur qui le rôle serveur d’accès au client est installé. 
  
Pour rechercher d’autres options pour le message de demande de **l’opération CopyItem,** explorez la hiérarchie de schéma. Commencez à [l’élément CopyItem.](copyitem.md) 
  
## <a name="successful-copyitem-response"></a>Réponse CopyItem réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la **demande CopyItem.** 
  
L’identificateur d’élément du nouvel élément est renvoyé dans le message de réponse. Les identificateurs d’élément ne sont pas renvoyés dans les réponses pour les opérations **CopyItem** de dossier public entre boîtes aux lettres ou de boîtes aux lettres. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
Pour rechercher d’autres options pour le message de réponse de **l’opération CopyItem,** explorez la hiérarchie de schéma. Commencez par [l’élément CopyItemResponse.](copyitemresponse.md) 
  
## <a name="copyitem-error-response"></a>Réponse d’erreur CopyItem

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande CopyItem.** 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Items](items.md)
    
Pour rechercher d’autres options pour le message de réponse d’erreur de l’opération **CopyItem,** explorez la hiérarchie de schéma. Commencez par [l’élément CopyItemResponse.](copyitemresponse.md) 
  
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

