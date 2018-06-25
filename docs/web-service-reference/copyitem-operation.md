---
title: CopyItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: L’opération CopyItem copie des éléments et place les éléments dans un autre dossier.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755667"
---
# <a name="copyitem-operation"></a>CopyItem Operation

L’opération **CopyItem** copie des éléments et place les éléments dans un autre dossier. 
  
## <a name="copyitem-request-example"></a>Exemple de requête CopyItem

### <a name="description"></a>Description

Une demande **CopyItem** l’exemple suivant montre comment créer une requête pour copier un élément dans la boîte de réception. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [CopyItem](copyitem.md)
    
- [ToFolderId](tofolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [ItemId](itemids.md)
    
- [ID d’élément](itemid.md)
    
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé. 
  
Pour trouver d’autres options pour le message de demande de l’opération **CopyItem** , explorez la hiérarchie de schéma. Commencer à l’élément [CopyItem](copyitem.md) . 
  
## <a name="successful-copyitem-response"></a>Réponse CopyItem réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à la demande **CopyItem** . 
  
L’identificateur d’élément du nouvel élément est retournée dans le message de réponse. Identificateurs d’éléments ne sont pas retournés dans les réponses pour cross-boîte aux lettres ou aux opérations **CopyItem** de dossier public. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CopyItemResponse](copyitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CopyItemResponseMessage](copyitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
Pour trouver d’autres options pour le message de réponse de l’opération **CopyItem** , explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="copyitem-error-response"></a>Réponse d’erreur CopyItem

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande de **CopyItem** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
Pour trouver d’autres options pour le message de réponse de l’opération **CopyItem** , explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [CopyItemResponse](copyitemresponse.md) . 
  
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

