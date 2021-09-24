---
title: Opération FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: L’opération FindFolder utilise Exchange Web Services pour rechercher les sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent l’ensemble des sous-dossiers.
ms.openlocfilehash: 8c2776a9d60244fe77b6012a09ffbad230d86f63
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518469"
---
# <a name="findfolder-operation"></a>Opération FindFolder

**L’opération FindFolder** utilise Exchange Web Services pour rechercher les sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent l’ensemble des sous-dossiers. 
  
## <a name="remarks"></a>Remarques

FindFolder renvoie uniquement les 512 premiers octets d’une propriété streamable. Pour Unicode, elle renvoie les 255 premiers caractères à l’aide d’une chaîne Unicode terminée par null.
  
Les requêtes de traversée approfondies ne peuvent pas être effectuées sur des dossiers publics.
  
Les restrictions sont autorisées et doivent utiliser uniquement les propriétés de dossier, et non les propriétés d’élément. La fonctionnalité de tri n’est pas disponible pour **les réponses FindFolder.** Les requêtes groupées ne sont pas disponibles **pour les requêtes FindFolder.** 
  
 **Remarque** **L’opération FindFolder** permet également de rechercher des dossiers gérés. 
  
### <a name="soap-headers"></a>En-têtes SOAP

**L’opération FindFolder** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant. 
  
|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|Emprunt d’identité  <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité.  <br/> |
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération.  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande.  <br/> |
|TimeZoneContext  <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.  <br/> |
   
## <a name="findfolder-request-example"></a>Exemple de requête FindFolder

### <a name="description"></a>Description

L’exemple suivant **d’une requête FindFolder** montre comment former une demande pour rechercher tous les dossiers situés dans une boîte de réception. 
  
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

À l’aide de la valeur Par défaut de la [forme](baseshape.md)de base, la réponse renvoie le nom du dossier, l’ID du dossier, le nombre de sous-dossiers, le nombre de dossiers enfants trouvés dans le dossier et le nombre d’éléments non lus.
  
### <a name="request-elements"></a>Éléments de demande

Cette **requête FindFolder inclut** les éléments suivants : 
  
- [FindFolder](findfolder.md)
    
- [FolderShape](foldershape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
 Pour obtenir **d’autres éléments de requête FindFolder,** consultez le schéma. 
  
## <a name="findfolder-response-example"></a>Exemple de réponse FindFolder

### <a name="description"></a>Description

L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la **demande FindFolder.** La réponse contient les éléments qui sont renvoyés lorsque la valeur Par défaut de [la forme de](baseshape.md) base est utilisée. 
  
> [!NOTE]
> L’ID de dossier et la touche de modification ont été raccourcis pour préserver la lisibilité. 
  
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

### <a name="response-elements"></a>Éléments de réponse

Les propriétés renvoyées dans la réponse sont déterminées par [baseshape](baseshape.md) et [AdditionalProperties si](additionalproperties.md) elles sont utilisées. Une réponse **FindFolder réussie inclut** les éléments suivants : 
  
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

 **Les réponses FindFolder** à une demande avec la forme de réponse **AllProperties** ne retourneront pas les éléments [TotalCount](totalcount.md) et [UnreadCount](unreadcount.md) pour les recherches de dossiers publics. 
  
## <a name="findfolder-error-response-example"></a>Exemple de réponse d’erreur FindFolder

### <a name="description"></a>Description

L’exemple de corps SOAP suivant montre une réponse d’erreur qui se produit lorsque vous recherchez un dossier identifié par un identificateur de dossier malformé.
  
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

La **réponse d’erreur FindFolder** inclut les éléments suivants : 
  
- [FindFolderResponse](findfolderresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="additional-information"></a>Informations complémentaires

- [L’élément DisplayName (string)](displayname-string.md) du dossier est toujours inclus dans la forme par défaut. 
    
- [L’élément UnreadCount](unreadcount.md) est inclus dans les dossiers Tâches et Notes. 
    
- Utilisez la **valeur PropertyTag** de 0x672D avec un type de propriété **Integer** pour identifier un dossier géré à l’aide de l’élément [ExtendedFieldURI.](extendedfielduri.md) 
    
## <a name="see-also"></a>Voir aussi



[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

