---
title: Opération ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: L’opération ResolveNames résout des adresses de messagerie ambiguës et des noms d’affichage.
ms.openlocfilehash: f5ab0e3ee23cc085d8aa425c6eeb0ac7c392b9bb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509447"
---
# <a name="resolvenames-operation"></a>Opération ResolveNames

**L’opération ResolveNames** résout des adresses de messagerie ambiguës et des noms d’affichage. 
  
## <a name="using-the-resolvenames-operation"></a>Utilisation de l’opération ResolveNames

Cette opération permet de vérifier les alias et de résoudre les noms d’affichage pour l’utilisateur de boîte aux lettres approprié. S’il existe des noms ambigus, la réponse **de l’opération ResolveNames** fournit des informations sur chaque utilisateur de boîte aux lettres afin que l’application cliente puisse résoudre les noms. 
  
## <a name="remarks"></a>Remarques

La réponse ResolveNames renvoie un maximum de 100 candidats. Les 100 candidats renvoyés sont les 100 premiers qui sont rencontrés dans l’opération de recherche.
  
Les adresses de messagerie avec des types de routage préfixés, tels que smtp ou sip, sont enregistrées dans un tableau à valeurs multiples. **L’opération ResolveNames** effectue une correspondance partielle par rapport à chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ». Si vous ne spécifiez pas de type de routage, **ResolveNames** sera par défaut le type de routage de smtp, le mettre en correspondance avec une propriété d’adresse smtp principale et ne pas effectuer de recherche dans le tableau à valeurs multiples. 
  
Un seul nom ambigu peut être spécifié dans une seule requête. Active Directory est recherché en premier, puis le dossier de contacts de l’utilisateur est recherché. Les entrées résolues à partir du dossier de contacts d’un utilisateur ont une propriété **ItemId** non null, qui peut ensuite être utilisée dans une demande GetItem. S’il s’agit de l’ID d’une liste de distribution privée, il peut être utilisé dans une [opération ExpandDL](expanddl-operation.md). Si **l’attribut ReturnFullContactData** est définie sur **true,** alors les entrées Active Directory trouvées avec l’opération **ResolveNames** retournent des propriétés supplémentaires qui décrivent un [contact](contact.md). **L’attribut ReturnFullContactData** n’affecte pas les données renvoyées pour les contacts et les listes de distribution privées à partir du dossier de contacts de l’utilisateur. 
  
## <a name="resolvenames-request-example"></a>Exemple de requête ResolveNames

### <a name="description"></a>Description

L’exemple suivant **d’une requête ResolveNames** montre comment résoudre l’entrée de User.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La réponse à cette demande retourne toutes les entrées qui commencent par « Jo » ou « Mi ». Les éléments renvoyés sont les boîtes aux lettres publiques, les listes de distribution publiques et privées et les contacts.
  
> [!NOTE]
> Seuls les contacts du dossier Contacts personnels par défaut sont recherchés. 
  
Voici les résultats possibles pour une **demande ResolveNames** : 
  
- Les réponses qui ne contiennent pas une entité résolue retournent une valeur d’attribut **ResponseClass** égale à **Error**. **L’élément MessageText** contiendra « **Aucun résultat n’est trouvé**».
    
- Les réponses qui contiennent une seule entité résolue retournent une valeur d’attribut **ResponseClass** égale à **Success**.
    
- Les réponses qui contiennent plusieurs entités possibles retournent une valeur d’attribut **ResponseClass** égale à **Warning**. Dans ce cas, l’entité n’a pas pu être résolue en une identité unique. **L’élément MessageText** contiendra « Plusieurs résultats sont trouvés ». 
    
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [ResolveNames](resolvenames.md)
    
- [UnresolvedEntry](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a>Exemple de réponse d’opération ResolveNames réussie

### <a name="description"></a>Description

L’exemple suivant montre une réponse réussie à **une demande ResolveNames.** 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-resolvenames-response-elements"></a>Éléments de réponse ResolveNames réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ResolveNamesResponse](resolvenamesresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [ResolutionSet](resolutionset.md)
    
- [Solution](resolution.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
- [Contact](contact.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entrée (EmailAddress)](entry-emailaddress.md)
    
- [ContactSource](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a>Réponse d’erreur d’opération ResolveNames

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à **une demande ResolveNames.** L’erreur est due à la tentative de résolution d’un nom qui ne peut pas être résolu. 
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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


[Utilisation de la résolution de noms](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

