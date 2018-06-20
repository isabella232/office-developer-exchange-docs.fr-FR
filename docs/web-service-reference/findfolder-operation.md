---
title: FindFolder Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: L’opération FindFolder utilise les Services Web Exchange pour rechercher les sous-dossiers d’un dossier donné et retourne un ensemble de propriétés qui décrivent l’ensemble de sous-dossiers.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756386"
---
# <a name="findfolder-operation"></a>FindFolder Operation

L’opération **FindFolder** utilise les Services Web Exchange pour rechercher les sous-dossiers d’un dossier donné et retourne un ensemble de propriétés qui décrivent l’ensemble de sous-dossiers. 
  
## <a name="remarks"></a>Remarques

FindFolder renvoie uniquement les 512 octets de n’importe quelle propriété lisible en continu. Pour le format Unicode, elle renvoie les 255 premiers caractères à l’aide d’une chaîne Unicode terminée par null.
  
Impossible d’effectuer des requêtes approfondies sur les dossiers publics.
  
Restrictions sont autorisées et doivent utiliser uniquement les propriétés du dossier, pas les propriétés d’élément. Les fonctionnalités de tri n’est pas disponible pour les réponses **FindFolder** . Requêtes groupées ne sont pas disponibles pour les requêtes **FindFolder** . 
  
 **Remarque** L’opération **FindFolder** est également utilisée pour rechercher les dossiers gérés. 
  
### <a name="soap-headers"></a>En-têtes SOAP

L’opération **FindFolder** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur.  <br/> |
   
## <a name="findfolder-request-example"></a>Exemple de requête FindFolder

### <a name="description"></a>Description

L’exemple suivant d’une demande **FindFolder** indique comment former une requête pour rechercher tous les dossiers situés dans une boîte de réception. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La réponse à l’aide de la valeur par défaut pour le [BaseShape](baseshape.md), cette propriété renvoie le nom du dossier, l’ID de dossier, le nombre de sous-dossiers, le nombre de dossiers enfants qui que se trouve dans le dossier et le nombre d’éléments non lus.
  
### <a name="request-elements"></a>Éléments de la demande

Cette demande **FindFolder** comprend les éléments suivants : 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Pour les éléments de demande **FindFolder** supplémentaires, voir le schéma. 
  
## <a name="findfolder-response-example"></a>Exemple de réponse FindFolder

### <a name="description"></a>Description

L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **FindFolder** . La réponse contient les éléments qui sont renvoyées lorsque la valeur par défaut pour la [BaseShape](baseshape.md) est utilisée. 
  
> [!NOTE]
> L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a>Éléments de réponse

Les propriétés qui sont retournées dans la réponse sont déterminées par le [BaseShape](baseshape.md) et [AdditionalProperties](additionalproperties.md) si elles sont utilisées. Une réponse positive de **FindFolder** comprend les éléments suivants : 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindFolderResponseMessage](findfolderresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Dossiers](folders-ex15websvcsotherref.md)
    
- [Folder](folder.md)
    
- [FolderId](folderid.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [TotalCount](totalcount.md)
    
- [ChildFolderCount](childfoldercount.md)
    
- [UnreadCount](unreadcount.md)
    
### <a name="comments"></a>Commentaires

 **FindFolder** réponses à une demande de la forme de réponse **AllProperties** ne renvoient pas [TotalCount](totalcount.md) et éléments [UnreadCount](unreadcount.md) pour les recherches de dossier public. 
  
## <a name="findfolder-error-response-example"></a>Exemple de réponse d’erreur FindFolder

### <a name="description"></a>Description

L’exemple de corps SOAP suivante montre une réponse d’erreur qui se produit lorsque vous recherchez un dossier identifié par un identificateur de dossier incorrect.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

La réponse d’erreur **FindFolder** comprend les éléments suivants : 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Informations supplémentaires

- L’élément [DisplayName (string)](displayname-string.md) de dossier est toujours inclus dans la forme par défaut. 
    
- L’élément [UnreadCount](unreadcount.md) est inclus dans les dossiers de tâches et de Notes. 
    
- Utilisez la valeur de **PropertyTag** de 0x672D avec un type de propriété de **nombre entier** pour identifier un dossier géré à l’aide de l’élément [ExtendedFieldURI](extendedfielduri.md) . 
    
## <a name="see-also"></a>Voir aussi



[Recherche de dossiers](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

