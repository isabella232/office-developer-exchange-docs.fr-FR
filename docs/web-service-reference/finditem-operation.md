---
title: FindItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Opération de recherche plus d’informations sur la EWS FindItem.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756405"
---
# <a name="finditem-operation"></a>FindItem Operation

Trouvez des informations sur l’opération EWS **FindItem** . 
  
L’opération **FindItem** recherche des éléments qui sont trouvent dans la boîte aux lettres d’un utilisateur. Cette opération fournit de nombreuses façons de filtrer et comment les résultats de la recherche sont renvoyés à l’appelant de format. 
  
## <a name="using-the-finditem-operation"></a>Utilisation de l’opération FindItem

La requête d’opération **FindItem** offre de nombreux moyens pour rechercher une boîte aux lettres et le format comment les données sont retournées dans une réponse. Vous pouvez spécifier ce qui suit dans une requête **FindItem** : 
  
- Si la recherche est un parcours superficiel ou supprimée. Cette spécification est requis. Notez qu’un parcours récupérable combiné à une restriction de recherche entraînera zéro éléments retournés, même s’il existe des éléments qui correspondent aux critères de recherche.
    
- La forme de réponse d’éléments. Ces informations identifient les propriétés qui sont retournées dans la réponse. Cette spécification est requis.
    
- Les dossiers à partir de laquelle effectuer la recherche. Cette spécification est requis.
    
- Les types de mécanisme et affichage de pagination pour le renvoi d’afficher des données dans les pages. Cette spécification est facultative.
    
- Options de regroupement et de tri des éléments qui sont retournés. Cette spécification est facultative.
    
- Restrictions de recherche ou des chaînes de syntaxe de requête avancée (AQS) pour filtrer les éléments qui sont retournés. Pour plus d’informations sur l’utilisation de AQS pour les recherches de l’index de contenu, voir [QueryString (chaîne)](querystring-string.md). Cette spécification est facultative.
    
- L’ordre de tri des éléments retournés dans la réponse. Cette spécification est facultative.
    
L’opération **FindItem** renvoie uniquement les 512 octets de n’importe quelle propriété lisible en continu. Pour le format Unicode, elle renvoie les 255 premiers caractères à l’aide d’une chaîne Unicode terminée par null. Elle ne renvoie pas les formats de corps de message ou les listes de destinataires. **FindItem** renverra un destinataire résumé. Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les détails d’un élément. 
  
 **FindItem** renvoie uniquement l’élément [nom (EmailAddressType)](name-emailaddresstype.md) et ne retourne pas l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) dans l’élément de [boîte aux lettres](mailbox.md) pour les champs suivants : 
  
- Le champ [](from.md) des messages 
    
- Le champ de [l’expéditeur](sender.md) pour les messages 
    
- Le champ [organisateur](organizer.md) des éléments de calendrier 
    
> [!NOTE]
> L’opération **FindItem** peut retourner des résultats dans un élément [CalendarView](calendarview.md) . L’élément **CalendarView** renvoie les éléments de calendrier unique et toutes les occurrences des réunions périodiques. Si un élément **CalendarView** n’est pas utilisé, les éléments de calendrier et les éléments de calendrier principal périodiques sont renvoyés. Si un élément **CalendarView** n’est pas utilisé, les occurrences doivent être développées à partir de la forme de base périodique. 
  
L’opération **FindItem** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
**Le tableau 1. En-têtes SOAP FindItem opération**

|**Header**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**DateTimePrecision** <br/> |[DateTimePrecision](datetimeprecision.md) <br/> |Spécifie la résolution des valeurs de date/heure dans les réponses à partir du serveur, en secondes ou en millisecondes. Ceci s’applique à une demande.  <br/> |
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Ceci s’applique à une demande.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres. Ceci s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Ceci s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cela s’applique à une réponse.  <br/> |
|**TimeZoneContext** <br/> |[TimeZoneContext](timezonecontext.md) <br/> |Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur. Ceci s’applique à une demande.  <br/> |
   
## <a name="finditem-operation-request-example"></a>Exemple de requête d’opération FindItem

Une demande **FindItem** l’exemple suivant montre comment obtenir l’identificateur d’élément qui est définie par l’énumération **IdOnly** de l’élément [BaseShape](baseshape.md) pour les éléments qui se trouvent dans le dossier éléments supprimés. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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
    
Pour plus d’options pour un message de demande **FindItem** , explorez la hiérarchie de schéma. Commencer à l’élément [FindItem](finditem.md) . 
  
## <a name="successful-finditem-operation-response"></a>Réponse d’opération FindItem réussie

L’exemple suivant montre une réponse positive à la demande **FindItem** . 
  
Éléments de [message](message-ex15websvcsotherref.md) représentent des messages électroniques et tous les autres éléments qui ne sont pas fortement typées dans le schéma EWS. Éléments tels que IPM. Partage et IPM.InfoPath sont renvoyés en tant qu’éléments du [Message](message-ex15websvcsotherref.md) . Exchange ne renvoie pas de [l’élément de base](item.md) des réponses. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
- [ID d’élément](itemid.md)
    
Pour plus d’options pour un message de réponse **FindItem** , explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [FindItemResponse](finditemresponse.md) . 
  
## <a name="finditem-operation-error-response"></a>Réponse d’erreur FindItem opération

L’exemple suivant montre une réponse d’erreur à une demande **FindItem** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
Pour plus d’options pour un message de réponse d’erreur **FindItem** , explorez la hiérarchie de schéma. Démarrez au niveau de l’élément [FindItemResponse](finditemresponse.md) . 
  
## <a name="version-differences"></a>Différences entre les versions

Versions d’Exchange depuis la version majeure 15 et se terminant par créer 15.0.898.11 retour une valeur ErrorInvalidOperation dans l’élément [ResponseCode](responsecode.md) lors de l’opération **FindItem** est utilisée pour rechercher plusieurs dossiers dans une boîte aux lettres d’archive. 
  
## <a name="see-also"></a>Voir aussi

- [Recherche d’éléments](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
    
- **FindItemType**
    

