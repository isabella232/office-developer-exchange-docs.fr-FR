---
title: Opération FindFolder
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
description: L’opération FindFolder utilise les services Web Exchange pour rechercher des sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent le jeu de sous-dossiers.
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462583"
---
# <a name="findfolder-operation"></a>Opération FindFolder

L’opération **FindFolder** utilise les services Web Exchange pour rechercher des sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent le jeu de sous-dossiers. 
  
## <a name="remarks"></a>Remarques

FindFolder renvoie uniquement les premiers 512 octets de toutes les propriétés transmises en continu. Pour Unicode, elle renvoie les premiers caractères 255 à l’aide d’une chaîne Unicode terminée par un caractère null.
  
Les requêtes de parcours approfondi ne peuvent pas être exécutées sur les dossiers publics.
  
Les restrictions sont autorisées et doivent utiliser uniquement les propriétés du dossier, pas les propriétés de l’élément. La fonctionnalité de tri n’est pas disponible pour les réponses **FindFolder** . Les requêtes regroupées ne sont pas disponibles pour les requêtes **FindFolder** . 
  
 **Note** L’opération **FindFolder** est également utilisée pour rechercher des dossiers gérés. 
  
### <a name="soap-headers"></a>En-têtes SOAP

L’opération **FindFolder** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.  <br/> |
   
## <a name="findfolder-request-example"></a>Exemple de requête FindFolder

### <a name="description"></a>Description

L’exemple de requête **FindFolder** suivant montre comment créer une requête pour rechercher tous les dossiers situés dans une boîte de réception. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

À l’aide de la valeur par défaut de l' [BaseShape](baseshape.md), la réponse renvoie le nom du dossier, l’ID du dossier, le nombre de sous-dossiers, le nombre de dossiers enfants trouvés dans le dossier et le nombre d’éléments non lus.
  
### <a name="request-elements"></a>Demander des éléments

Cette requête **FindFolder** inclut les éléments suivants : 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Pour d’autres éléments de requête **FindFolder** , voir le schéma. 
  
## <a name="findfolder-response-example"></a>Exemple de réponse FindFolder

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **FindFolder** . La réponse contient les éléments qui sont renvoyés lorsque la valeur par défaut de l' [BaseShape](baseshape.md) est utilisée. 
  
> [!NOTE]
> L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a>Éléments Response

Les propriétés qui sont renvoyées dans la réponse sont déterminées par le [BaseShape](baseshape.md) et le [AdditionalProperties](additionalproperties.md) s’ils sont utilisés. Une réponse **FindFolder** réussie inclut les éléments suivants : 
  
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

 **FindFolder** les réponses à une requête avec la forme de réponse **AllProperties** ne renvoient pas les éléments [totalCount](totalcount.md) et [UnreadCount](unreadcount.md) pour les recherches de dossiers publics. 
  
## <a name="findfolder-error-response-example"></a>Exemple de réponse d’erreur FindFolder

### <a name="description"></a>Description

L’exemple de corps SOAP suivant montre une réponse d’erreur qui se produit lorsque vous recherchez un dossier identifié par un identificateur de dossier incorrect.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="additional-information"></a>Informations complémentaires

- L’élément Folder [DisplayName (String)](displayname-string.md) est toujours inclus dans la forme par défaut. 
    
- L’élément [UnreadCount](unreadcount.md) est inclus dans les dossiers tâches et notes. 
    
- Utilisez la valeur **PropertyTag** de 0x672D avec une propriété de type **Integer** pour identifier un dossier géré à l’aide de l’élément [ExtendedFieldURI](extendedfielduri.md) . 
    
## <a name="see-also"></a>Voir aussi



[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

