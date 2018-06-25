---
title: Opération ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: L’opération ExpandDL expose tous les membres des listes de distribution.
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756263"
---
# <a name="expanddl-operation"></a>Opération ExpandDL

L’opération ExpandDL expose tous les membres des listes de distribution.
  
## <a name="using-the-expanddl-web-method"></a>À l’aide de la méthode Web ExpandDL

L’opération ExpandDL utilise le service Web qui se trouve dans Exchange.asmx. Cette méthode de service Web accepte un élément de [boîte aux lettres](mailbox.md) qui peut contenir un élément enfant de [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) pour une extension d’une liste de distribution publique ou un élément enfant de [ItemId](itemid.md) pour le développement de privé liste de distribution. 
  
Listes de distribution publiques peuvent être développés à l’aide d’une des options suivantes :
  
1. Alias de liste de distribution
    
2. L’adresse SMTP Simple Mail Transfer Protocol)
    
3. X400
    
4. X500
    
5. Adresse Exchange hérité
    
6. Nom de la liste de distribution
    
7. Le nom complet
    
> [!IMPORTANT]
> Noms complets ne sont pas uniques. Comptes multiples peuvent partager le même nom complet. 
  
## <a name="remarks"></a>Remarques

Le développement récursive n’est pas pris en charge. Liste de distribution qu’un seul peut être développée dans un seul appel. Si plusieurs listes de distribution correspondant aux critères, le service Web signale une erreur. Une application cliente permet la résolution de nom ambigu (ANR) pour trouver distribution ambigüe répertorie, puis sur l’adresse de messagerie de la liste de distribution requis en tant que paramètre de l' [opération ExpandDL](expanddl-operation.md). Pour plus d’informations, voir [opération ResolveNames](resolvenames-operation.md).
  
Listes de distribution publiques sont situés dans Active Directory. Ils peuvent être n’importe quel groupe de distribution dynamique ou à extension messagerie. Le groupe ne doit pas être masqué à partir de la liste d’adresses et chaque membre doit avoir une adresse de messagerie non vides. Membres de la liste de distribution peuvent être des utilisateurs à extension messagerie et de contacts, les dossiers publics et les listes de distribution à extension messagerie et groupes dynamiques.
  
Listes de distribution privée se trouvent dans le dossier Contacts de boîte aux lettres d’un utilisateur. Listes de distribution privée n’ont pas d’adresses de messagerie pour leurs identificateurs d’élément de magasin sont utilisés dans une requête ExpandDL. Membres d’une liste de distribution privée peuvent être n’importe quel utilisateur à extension messagerie, les contacts ou les listes de distribution à partir d’Active Directory ou les listes de contacts ou distribution privée à partir du dossier de Contacts d’un utilisateur.
  
Pour des contacts ou des listes de distribution privée, les identificateurs d’élément sont retournés dans la réponse. Cela peut servir à obtenir des informations sur l’objet ou de développer l’appartenance à une liste de distribution privée.
  
## <a name="expanddl-private-distribution-list-request-example"></a>Exemple de requête de liste de Distribution privée ExpandDL

### <a name="description"></a>Description

L’exemple suivant d’une demande ExpandDL indique comment former une demande pour développer une liste de distribution privée.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Pour développer une liste de distribution privée, l’élément de [boîte aux lettres](mailbox.md) contient l’élément [ItemId](itemid.md) qui identifie une liste de distribution privée dans la boîte aux lettres de l’utilisateur. 
  
## <a name="expanddl-public-distribution-list-request-example"></a>Exemple de requête de liste de Distribution publique ExpandDL

### <a name="description"></a>Description

L’exemple suivant d’une demande ExpandDL indique comment former une demande pour développer une liste de distribution publique. L’exemple illustre l’utilisation d’un nom d’affichage pour développer une liste de distribution.
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La réponse à cette demande contient des éléments de **boîte aux lettres** qui identifient chaque boîte aux lettres dans la liste de distribution. Si une liste de distribution est contenue dans une liste de distribution, une extension de la liste de distribution doit être effectuée sur la liste de distribution incorporées. Si la liste de distribution ne possède aucun membre ou la liste de distribution demandée n’existe pas, l’attribut **ResponseClass** contient une valeur égale à la réussite. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [ExpandDL](expanddl.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est utilisé pour identifier les listes de distribution publiques. L’élément [ItemId](itemid.md) est utilisé pour identifier les listes de distribution privée. 
    
> [!NOTE]
> Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé. 
  
## <a name="successful-expanddl-response-example"></a>Exemple de réponse ExpandDL réussie

### <a name="description"></a>Description

L’exemple suivant d’une réponse ExpandDL montre une réponse à la demande décrite ci-dessus. Le développement de listes de distribution décrit les éléments suivants : 
  
- Le nombre de membres de la liste de distribution qui sont retournés dans la réponse.
    
- Si la réponse contient tous les membres de la liste de distribution.
    
- Nom de la boîte aux lettres.
    
- L’adresse de messagerie de la boîte aux lettres.
    
- Le type de routage pour la boîte aux lettres.
    
- Le type de boîte aux lettres.
    
> [!NOTE]
> Nom de la liste de distribution n’est pas inclus dans la réponse ; Par conséquent, vous devez garder une trace du nom à partir de la demande. 
  
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
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [ExpandDLResponse](expanddlresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [DLExpansion](dlexpansion.md)
    
- [Boîte aux lettres](mailbox.md)
    
- [Nom (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [MailboxType](mailboxtype.md)
    
Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="expanddl-error-response"></a>Réponse d’erreur ExpandDL

### <a name="description"></a>Description

L’exemple suivant montre une réponse d’erreur à une demande de ExpandDL.
  
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
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [ExpandDLResponse](expanddlresponse.md) . 
  
## <a name="see-also"></a>Voir aussi

- [Opération ResolveNames](resolvenames-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

