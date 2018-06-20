---
title: Opération ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: Adresses de messagerie ambiguë ResolveNames opération résout les noms d’affichage.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829162"
---
# <a name="resolvenames-operation"></a>Opération ResolveNames

Adresses de messagerie ambiguë **ResolveNames** opération résout les noms d’affichage. 
  
## <a name="using-the-resolvenames-operation"></a>Utilisation de l’opération ResolveNames

Cette opération peut être utilisée pour vérifier les alias et résoudre les noms d’affichage à l’utilisateur de boîte aux lettres appropriée. Si des noms ambigus existent, la réponse d’opération **ResolveNames** fournit des informations sur chaque utilisateur de boîte aux lettres afin que l’application cliente peut résoudre les noms. 
  
## <a name="remarks"></a>Remarques

La réponse ResolveNames renvoie un maximum de 100 candidats. Les 100 candidats qui sont retournées sont les 100 premières lors de l’opération de recherche.
  
Adresses de messagerie avec des types de routage préfixés, tel que smtp ou sip, sont enregistrés dans un tableau à valeurs multiples. L’opération **ResolveNames** effectue une correspondance partielle dans chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ». Si vous ne spécifiez pas un type de routage, **ResolveNames** par défaut pour le type de routage du service smtp, faire correspondre à une propriété d’adresse smtp principale et recherche pas dans le tableau à valeurs multiples. 
  
Qu’un seul nom ambigu peut être spécifié dans une demande unique. Active Directory est recherché en premier, puis le dossier de contacts de l’utilisateur est recherché. Résolu les entrées de dossier de contacts d’un utilisateur dont la propriété **ItemId** non null, qui peut ensuite être utilisée dans une requête GetItem. S’il s’agit de l’ID d’une liste de distribution privée, il peut être utilisé dans une [opération ExpandDL](expanddl-operation.md). Si l’attribut **ReturnFullContactData** est défini sur **true**, les entrées Active Directory avec l’opération **ResolveNames** renverra des propriétés supplémentaires qui décrivent un [Contact](contact.md). L’attribut **ReturnFullContactData** n’affecte pas les données qui sont retournées pour les contacts et privées des listes de distribution à partir du dossier de contacts de l’utilisateur. 
  
## <a name="resolvenames-request-example"></a>Exemple de requête ResolveNames

### <a name="description"></a>Description

L’exemple suivant d’une demande **ResolveNames** indique comment faire pour résoudre l’entrée de l’utilisateur.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La réponse à cette demande retournera toutes les entrées qui commencent par « Jo » ou « Mi ». Les éléments retournés sont publics boîtes aux lettres, les listes de distribution publiques et privées et les contacts.
  
> [!NOTE]
> Seuls les contacts dans le dossier Contacts personnel sont recherchés. 
  
Les résultats d’une requête **ResolveNames** possibles sont les suivantes : 
  
- Réponses qui ne contiennent pas une entité résolue renvoie une valeur d’attribut **ResponseClass** égale à **l’erreur**. L’élément **MessageText** contiendra « **aucun résultat n’est trouvé**. »
    
- Réponses qui contiennent une seule entité résolue renvoie une valeur d’attribut **ResponseClass** égale à la **Réussite**.
    
- Réponses qui contiennent plusieurs entités possibles renvoie une valeur d’attribut **ResponseClass** égale à **Avertissement**. Dans ce cas, l’entité pas pu être résolue vers une identité unique. L’élément **MessageText** contiendra « plusieurs résultats sont trouvent. » 
    
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Exemple de réponse opération ResolveNames réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse positive à une demande **ResolveNames** . 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a>Éléments de réponse ResolveNames réussies

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Solution](resolution.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [Nom (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contact](contact.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entrée (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Réponse d’erreur ResolveNames opération

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande **ResolveNames** . L’erreur est provoquée par tente de résoudre un nom qui ne peut pas être résolu. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>Voir aussi



[Opération ExpandDL](expanddl-operation.md)


[À l’aide de la résolution de noms](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

