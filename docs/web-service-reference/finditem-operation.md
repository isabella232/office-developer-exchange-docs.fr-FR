---
title: Opération FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Trouvez des informations sur l’opération EWS FindItem.
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462555"
---
# <a name="finditem-operation"></a>Opération FindItem

Trouvez des informations sur l’opération EWS **FindItem** . 
  
L’opération **FindItem** recherche les éléments qui se trouvent dans la boîte aux lettres d’un utilisateur. Cette opération offre plusieurs façons de filtrer et de mettre en forme le mode de renvoi des résultats de la recherche à l’appelant. 
  
## <a name="using-the-finditem-operation"></a>Utilisation de l’opération FindItem

La demande d’opération **FindItem** vous permet d’effectuer des recherches dans une boîte aux lettres et de mettre en forme les données renvoyées dans une réponse de plusieurs façons. Vous pouvez spécifier ce qui suit dans une requête **FindItem** : 
  
- Indique si la recherche est une traversée partielle ou supprimée de manière récupérable. Cette spécification est requise. Notez qu’une traversée supprimée de manière récupérable combinée à une restriction de recherche entraîne zéro élément renvoyé, même si des éléments correspondent aux critères de recherche.
    
- Forme de la réponse des éléments. Cela identifie les propriétés qui sont renvoyées dans la réponse. Cette spécification est requise.
    
- Dossiers à partir desquels effectuer la recherche. Cette spécification est requise.
    
- Le mécanisme de pagination et les types d’affichage pour retourner les données d’affichage dans les pages. Cette spécification est facultative.
    
- Options de regroupement et de tri des éléments qui sont renvoyés. Cette spécification est facultative.
    
- Restrictions de recherche ou chaînes de syntaxe de requête avancée (AQS) pour le filtrage des éléments qui sont renvoyés. Pour plus d’informations sur l’utilisation de AQS pour les recherches d’index de contenu, voir [QueryString (String)](querystring-string.md). Cette spécification est facultative.
    
- Ordre de tri des éléments renvoyés dans la réponse. Cette spécification est facultative.
    
L’opération **FindItem** renvoie uniquement les premiers 512 octets de toutes les propriétés transmises en continu. Pour Unicode, elle renvoie les premiers caractères 255 à l’aide d’une chaîne Unicode terminée par un caractère null. Il ne renvoie aucun des formats de corps de message ou des listes de destinataires. **FindItem** renverra un résumé des destinataires. Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les détails d’un élément. 
  
 **FindItem** renvoie uniquement l’élément [Name (EmailAddressType)](name-emailaddresstype.md) et ne renvoie pas l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) dans l’élément [Mailbox](mailbox.md) pour les champs suivants : 
  
- Champ [de](from.md) pour les messages 
    
- Champ [expéditeur](sender.md) pour les messages 
    
- Champ [organisateur](organizer.md) des éléments de calendrier 
    
> [!NOTE]
> L’opération **FindItem** peut renvoyer des résultats dans un élément [CalendarView](calendarview.md) . L’élément **CalendarView** renvoie des éléments de calendrier uniques et toutes les occurrences de réunions périodiques. Si un élément **CalendarView** n’est pas utilisé, les éléments de calendrier uniques et les éléments de calendrier maître périodiques sont renvoyés. Les occurrences doivent être étendues à partir de la forme de base périodique si aucun élément **CalendarView** n’est utilisé. 
  
L’opération **FindItem** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
**Tableau 1. En-têtes SOAP d’opération FindItem**

|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Spécifie la résolution des valeurs de données/temps dans les réponses du serveur, soit en secondes, soit en millisecondes. Ceci s’applique à une demande.  <br/> |
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur qui emprunte l’identité de l’application cliente. Ceci s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres. Ceci s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Ceci s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Ceci s’applique à une réponse.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur. Ceci s’applique à une demande.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Exemple de requête d’opération FindItem

L’exemple de requête **FindItem** suivant montre comment obtenir l’identificateur d’élément défini par l’énumération **IdOnly** de l’élément [BaseShape](baseshape.md) pour les éléments qui se trouvent dans le dossier éléments supprimés. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

Les éléments suivants sont utilisés dans la demande : 
  
- [FindItem](finditem.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ParentFolderIds](parentfolderids.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
Pour plus d’options pour un message de demande **FindItem** , explorez la hiérarchie de schéma. Commencez par l’élément [FindItem](finditem.md) . 
  
## <a name="successful-finditem-operation-response"></a>Réponse de l’opération FindItem réussie

L’exemple suivant montre une réponse réussie à la demande **FindItem** . 
  
Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma EWS. Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments [message](message-ex15websvcsotherref.md) . Exchange ne retourne pas l’élément [élément](item.md) de base dans les réponses. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Les éléments suivants sont utilisés dans la réponse :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootFolder (FindItemResponseMessage)](rootfolder-finditemresponsemessage.md)
    
- [Items](items.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
Pour plus d’options pour un message de réponse **FindItem** , explorez la hiérarchie de schéma. Commencez par l’élément [FindItemResponse](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Réponse d’erreur d’opération FindItem

L’exemple suivant montre une réponse d’erreur à une requête **FindItem** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [FindItemResponse](finditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [FindItemResponseMessage](finditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour plus d’options pour un message de réponse d’erreur **FindItem** , explorez la hiérarchie de schéma. Commencez par l’élément [FindItemResponse](finditemresponse.md) . 
  
## <a name="version-differences"></a>Différences entre les versions

Les versions d’Exchange commençant par la version principale 15 et se terminant par Build 15.0.898.11 renvoient une valeur ErrorInvalidOperation dans l’élément [ResponseCode](responsecode.md) lorsque l’opération **FindItem** est utilisée pour rechercher plusieurs dossiers dans une boîte aux lettres d’archivage. 
  
## <a name="see-also"></a>Voir aussi

- [Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

