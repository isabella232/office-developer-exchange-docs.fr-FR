---
title: Opération SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 7f0de089-8876-47ec-a871-df118ceae75d
description: L’opération SyncFolderItems synchronise les éléments entre Exchange serveur et le client.
ms.openlocfilehash: 07915f5f9f7ae1fc6f5a743f2e0480a32cb808a7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545831"
---
# <a name="syncfolderitems-operation"></a>Opération SyncFolderItems

L’opération SyncFolderItems synchronise les éléments entre Exchange serveur et le client.
  
## <a name="remarks"></a>Remarques

L’opération SyncFolderItems retourne un maximum de 512 modifications. Les demandes SyncFolderItems suivantes doivent être effectuées pour obtenir des modifications supplémentaires. 
  
SyncFolderItems est similaire à l’opération FindItem dans la mesure où elle ne peut pas renvoyer de propriétés telles que Corps ou Pièces jointes. Si l’opération SyncFolderItems ne retourne pas les propriétés dont vous avez besoin, vous pouvez utiliser l’opération [GetItem](getitem-operation.md) pour obtenir un ensemble spécifique de propriétés pour chaque élément renvoyé par SyncFolderItems. 
  
## <a name="syncfolderitems-request-example"></a>Exemple de requête SyncFolderItems

### <a name="description"></a>Description

L’exemple suivant d’une demande SyncFolderItems montre comment synchroniser des éléments dans un dossier. Cet exemple illustre la synchronisation d’un élément de dossier qui n’est pas la première synchronisation à avoir eu lieu pour le dossier Éléments envoyés. [L’élément SyncState](syncstate-ex15websvcsotherref.md) n’est pas inclus dans la demande de la première tentative de synchronisation d’un client avec Exchange serveur. La première tentative de synchronisation des éléments dans une hiérarchie de dossiers retourne tous les éléments de la boîte aux lettres, à l’exception des éléments identifiés dans [l’élément Ignore.](ignore.md) Cette demande SyncFolderItems tentera de synchroniser toutes les modifications apportées aux éléments de dossier depuis la dernière synchronisation. Cette demande ignore la tentative de synchronisation de l’élément identifié dans [l’élément Ignore.](ignore.md) 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderItems xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
      </ItemShape>
      <SyncFolderId>
        <t:DistinguishedFolderId Id="sentitems"/>
      </SyncFolderId>
      <SyncState>AEbJ94eMOAAA=</SyncState>
      <Ignore>
        <t:ItemId Id="AQApAHRAA==" ChangeKey="CQAAABY"/>
      </Ignore>
      <MaxChangesReturned>100</MaxChangesReturned>
    </SyncFolderItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les [données codées](syncstate-ex15websvcsotherref.md) en base 64 de l’élément SyncState et l’attribut **id** de l’élément [ItemId](itemid.md) ont été raccourcis pour préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [SyncFolderItems](syncfolderitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncFolderId](syncfolderid.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [Ignore](ignore.md)
    
- [ItemId](itemid.md)
    
- [MaxChangesReturned](maxchangesreturned.md)
    
## <a name="successful-syncfolderitems-response"></a>Réponse SyncFolderItems réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à la demande SyncFolderItems. Dans cet exemple, une demande de réunion est synchronisée à partir du dossier Éléments envoyés.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAAAA=</m:SyncState>
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
          <m:Changes>
            <t:Create>
              <t:MeetingRequest>
                <t:ItemId Id="AQApAHRwA==" ChangeKey="CwAAABYA" />
                <t:Subject>Budget Q3</t:Subject>
                <t:Sensitivity>Normal</t:Sensitivity>
                <t:IsOutOfDate>false</t:IsOutOfDate>
                <t:HasBeenProcessed>true</t:HasBeenProcessed>
                <t:ResponseType>NoResponseReceived</t:ResponseType>
                <t:IntendedFreeBusyStatus>Busy</t:IntendedFreeBusyStatus>
                <t:Start>2006-08-02T17:30:00Z</t:Start>
                <t:End>2006-08-02T19:30:00Z</t:End>
                <t:Location>Conference Room 2</t:Location>
                <t:Organizer>
                  <t:Mailbox>
                    <t:Name>Dan Park</t:Name>
                    <t:EmailAddress>dpark@example.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                  </t:Mailbox>
                </t:Organizer>
              </t:MeetingRequest>
            </t:Create>
          </m:Changes>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les [données codées](syncstate-ex15websvcsotherref.md) en base 64 de l’élément SyncState et l’attribut **id** de l’élément [ItemId](itemid.md) ont été raccourcis pour préserver la lisibilité. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
- [Modifications (éléments)](changes-items.md)
    
- [Créer (ItemSync)](create-itemsync.md)
    
- [MeetingRequest](meetingrequest.md)
    
- [ItemId](itemid.md)
    
- [Sujet](subject.md)
    
- [Sensitivity](sensitivity.md)
    
- [IsOutOfDate](isoutofdate.md)
    
- [HasBeenProcessed](hasbeenprocessed.md)
    
- [ResponseType](responsetype.md)
    
- [IntendedFreeBusyStatus](intendedfreebusystatus.md)
    
- [Start](start.md)
    
- [Fin ](end-ex15websvcsotherref.md)
    
- [Location](location.md)
    
- [Organizer](organizer.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
## <a name="syncfolderitems-error-response"></a>Réponse d’erreur SyncFolderItems

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande SyncFolderItems. Cette erreur a été causée par un SyncState non valide.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderItemsResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupt or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastItemInRange>true</m:IncludesLastItemInRange>
        </m:SyncFolderItemsResponseMessage>
      </m:ResponseMessages>
    </SyncFolderItemsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderItemsResponse](syncfolderitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastItemInRange](includeslastiteminrange.md)
    
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

