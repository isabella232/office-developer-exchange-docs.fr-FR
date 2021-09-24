---
title: Opération ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: L’opération ExpandDL expose l’appartenance complète aux listes de distribution.
ms.openlocfilehash: 9878ecff0eeee1ef386c7bb26a092eec47f471de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513779"
---
# <a name="expanddl-operation"></a>Opération ExpandDL

L’opération ExpandDL expose l’appartenance complète aux listes de distribution.
  
## <a name="using-the-expanddl-web-method"></a>Utilisation de la méthode Web ExpandDL

L’opération ExpandDL utilise le service Web qui se trouve dans Exchange.asmx. Cette méthode de service Web accepte un élément [Mailbox](mailbox.md) qui peut contenir un élément enfant [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) pour l’expansion d’une liste de distribution publique ou un élément enfant [ItemId](itemid.md) pour l’expansion d’une liste de distribution privée. 
  
Les listes de distribution publiques peuvent être étendues à l’aide de l’une des suivantes :
  
1. Alias de liste de distribution
    
2. Adresse du service SMTP (Simple Mail Transfer Protocol)
    
3. X400
    
4. X500
    
5. Exchange Adresse héritée
    
6. Nom de la liste de distribution
    
7. Nom d’affichage
    
> [!IMPORTANT]
> Les noms d’affichage ne sont pas uniques. Plusieurs comptes peuvent partager le même nom complet. 
  
## <a name="remarks"></a>Remarques

L’expansion récursive n’est pas prise en charge. Une seule liste de distribution peut être étendue en un seul appel. Si plusieurs listes de distribution correspondent aux critères, le service Web signale une erreur. Une application cliente peut utiliser une résolution de nom ambigu (ANR) pour rechercher des listes de distribution ambiguës, puis choisir l’adresse de messagerie correcte de la liste de distribution requise comme paramètre pour l’opération [ExpandDL](expanddl-operation.md). Pour plus d’informations, voir [l’opération ResolveNames.](resolvenames-operation.md)
  
Les listes de distribution publiques se trouvent dans Active Directory. Il peut s’y trouver dans n’importe quel groupe de distribution dynamique ou à messagerie. Le groupe ne doit pas être masqué dans la liste d’adresses et chaque membre doit avoir une adresse de messagerie non vide. Les membres de la liste de distribution peuvent être des utilisateurs et des contacts à messagerie, des dossiers publics, des listes de distribution à messagerie et des groupes dynamiques.
  
Les listes de distribution privées se trouvent dans le dossier Contacts de la boîte aux lettres d’un utilisateur. Les listes de distribution privées n’ont pas d’adresses de messagerie, de sorte que leurs identificateurs d’élément de magasin sont utilisés dans une demande ExpandDL. Les membres d’une liste de distribution privée peuvent être des utilisateurs à messagerie, des contacts ou des listes de distribution d’Active Directory, des contacts ou des listes de distribution privées provenant du dossier Contacts d’un utilisateur.
  
Pour les contacts ou les listes de distribution privées, les identificateurs d’élément sont renvoyés dans la réponse. Cela peut être utilisé pour obtenir des informations sur l’objet ou pour développer l’appartenance à une liste de distribution privée.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Exemple de demande de liste de distribution privée ExpandDL

### <a name="description"></a>Description

L’exemple suivant d’une demande ExpandDL montre comment former une demande pour développer une liste de distribution privée.
  
### <a name="code"></a>Code

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Pour développer une liste de distribution privée, l’élément [Mailbox](mailbox.md) contient l’élément [ItemId](itemid.md) qui identifie une liste de distribution privée dans la boîte aux lettres de l’utilisateur. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Exemple de demande de liste de distribution publique ExpandDL

### <a name="description"></a>Description

L’exemple suivant d’une demande ExpandDL montre comment former une demande pour développer une liste de distribution publique. L’exemple illustre l’utilisation d’un nom complet pour développer une liste de distribution.
  
### <a name="code"></a>Code

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La réponse à cette demande contient des éléments **de** boîte aux lettres qui identifient chaque boîte aux lettres dans la liste de distribution. Si une liste de distribution est contenue dans une liste de distribution, une extension de liste de distribution distincte doit être effectuée sur la liste de distribution incorporée. Si la liste de distribution n’a pas de membres ou si la liste de distribution demandée n’existe pas, l’attribut **ResponseClass** contient une valeur égale à Success. 
  
### <a name="request-elements"></a>Éléments de demande

Les éléments suivants sont utilisés dans la demande :
  
- [ExpandDL](expanddl.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est utilisé pour identifier les listes de distribution publiques. [L’élément ItemId](itemid.md) est utilisé pour identifier les listes de distribution privées. 
    
> [!NOTE]
> Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
## <a name="successful-expanddl-response-example"></a>Exemple de réponse ExpandDL réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse ExpandDL montre une réponse à la demande décrite ci-dessus. L’extension de la liste de distribution décrit ce qui suit : 
  
- Nombre de membres de la liste de distribution renvoyés dans la réponse.
    
- Si la réponse contient tous les membres de la liste de distribution.
    
- Nom de la boîte aux lettres.
    
- Adresse de messagerie de la boîte aux lettres.
    
- Type de routage pour la boîte aux lettres.
    
- Type de boîte aux lettres.
    
> [!NOTE]
> Le nom de la liste de distribution n’est pas inclus dans la réponse . par conséquent, vous devez suivre le nom de la demande. 
  
### <a name="code"></a>Code

```xml
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
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Éléments de réponse réussis

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [Name (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Pour rechercher d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma. Commencez par [l’élément ExpandDLResponse.](expanddlresponse.md) 
  
## <a name="expanddl-error-response"></a>Réponse d’erreur ExpandDL

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande ExpandDL.
  
### <a name="code"></a>Code

```xml
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
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour rechercher d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma. Commencez par [l’élément ExpandDLResponse.](expanddlresponse.md) 
  
## <a name="see-also"></a>Voir aussi

- [Opération ResolveNames](resolvenames-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

