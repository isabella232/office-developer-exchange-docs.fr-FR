---
title: Opération SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: L’opération SyncFolderHierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838657"
---
# <a name="syncfolderhierarchy-operation"></a>Opération SyncFolderHierarchy

L’opération SyncFolderHierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.
  
> [!NOTE]
> L’opération SyncFolderHierarchy ne renvoie pas les dossiers lorsque les propriétés [UnreadCount](unreadcount.md) ou [TotalCount](totalcount.md) ont changé. 
  
## <a name="syncfolderhierarchy-request-example"></a>Exemple de requête SyncFolderHierarchy

### <a name="description"></a>Description

L’exemple suivant d’une demande SyncFolderHierarchy montre comment synchroniser un client de hiérarchie de dossiers avec le serveur Exchange. Cet exemple montre une hiérarchie de dossiers qui a déjà été synchronisée au moins une fois. L’élément [SyncState](syncstate-ex15websvcsotherref.md) n’est pas inclus dans la demande de la première tentative de synchroniser un client avec le serveur Exchange. La première requête retournera tous les dossiers dans la boîte aux lettres. L’élément [SyncState](syncstate-ex15websvcsotherref.md) est renvoyé dans la [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md). Cet élément est utilisé pour synchroniser l’état pour les demandes SyncFolderHierarchy suivantes.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les données d’élément codée en base64 [SyncState](syncstate-ex15websvcsotherref.md) a été raccourcies afin de préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [SyncFolderHierarchy](syncfolderhierarchy.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. 
  
## <a name="successful-syncfolderhierarchy-response"></a>Réponse SyncFolderHierarchy réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à la demande SyncFolderHierarchy. Dans cet exemple, un nouveau dossier a été synchronisé.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Les données d’élément codée en base64 [SyncState](syncstate-ex15websvcsotherref.md) et les données d’identificateur de dossier ont été réduites afin de préserver la lisibilité. 
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
- [Modifications (hiérarchie)](changes-hierarchy.md)
    
- [Créer (FolderSync)](create-foldersync.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [Classe FolderClass](folderclass.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a>Réponse d’erreur SyncFolderHierarchy

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande SyncFolderHierarchy. Cette erreur a été provoquée par une SyncState non valide.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [SyncState](syncstate-ex15websvcsotherref.md)
    
- [IncludesLastFolderInRange](includeslastfolderinrange.md)
    
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

