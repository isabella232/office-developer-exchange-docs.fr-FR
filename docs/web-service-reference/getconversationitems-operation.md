---
title: Opération GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: Trouvez des informations sur l’opération GetConversationItems.
ms.openlocfilehash: 0de9a380aa2f9b25e9a7ef90ebe7a9f485ca60d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513667"
---
# <a name="getconversationitems-operation"></a>Opération GetConversationItems

Trouvez des informations sur **l’opération GetConversationItems.** 
  
**L’opération GetConversationItems** obtient un ou plusieurs ensembles d’éléments organisés en des points dans une conversation. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getconversationitems-operation"></a>Utilisation de l’opération GetConversationItems

Vous pouvez utiliser **l’opération GetConversationItems** pour obtenir des éléments dans les conversations pour les boîtes aux lettres principales et d’archivage. 
  
### <a name="getconversationitems-operation-soap-headers"></a>En-têtes SOAP de l’opération GetConversationItems

**L’opération GetConversationItems peut** utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur dont l’application cliente usurpe l’identité. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma pour la demande d’opération. La valeur minimale de cet élément est **Exchange2013**. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a>Exemple de demande d’opération GetConversationItems : obtenir des éléments dans une seule conversation

L’exemple suivant d’une demande d’opération **GetConversationItems** montre comment obtenir tous les éléments de conversation dans une conversation unique, à l’exception des éléments situés dans les dossiers Éléments supprimés et Brouillons. Chaque élément renvoyé dans la réponse contient un identificateur d’élément, un objet et l’heure de réception de l’élément dans la boîte aux lettres. 
  
> [!NOTE]
> Tous les identificateurs d’élément et les touches de modification de cet article ont été raccourcis pour préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

Cet exemple de **demande GetConversationItems** n’inclut pas les options suivantes : 
  
- Élément [MaxItemsToReturn,](maxitemstoreturn.md) qui définit le nombre maximal d’éléments à renvoyer dans la réponse. 
    
- Élément [MailboxScope,](mailboxscope.md) qui définit l’étendue de la boîte aux lettres en indiquant si l’opération **GetConversationItems** doit être effectuée sur la boîte aux lettres principale, la boîte aux lettres d’archivage ou les deux boîtes aux lettres. 
    
- Élément [SyncState (base64Binary),](syncstate-base64binary.md) qui définit l’état de synchronisation pour obtenir uniquement les éléments de conversation nouveaux ou mis à jour dans la conversation. Cet élément est définie pour chaque conversation. 
    
Le corps SOAP de la requête contient les éléments suivants :
  
- [GetConversationItems](getconversationitems.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [AdditionalProperties](additionalproperties.md)
    
- [FieldURI](fielduri.md)
    
- [FoldersToIgnore](folderstoignore.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
- [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)
    
- [Conversations](conversations-ex15websvcsotherref.md)
    
- [Conversation (ConversationRequestType)](conversation-conversationrequesttype.md)
    
- [ConversationId](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a>Réponse de l’opération GetConversationItems réussie

L’exemple suivant montre une réponse réussie à une demande d’opération **GetConversationItems** pour obtenir des éléments dans une seule conversation. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

Nous vous recommandons d’enregistrer syncState pour les demandes d’opération **GetConversationItems suivantes.** 
  
Le corps SOAP de la réponse contient les éléments suivants :
  
- [GetConversationItemsResponse](getconversationitemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetConversationItemsResponseMessage](getconversationitemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Conversation (ConversationResponseType)](conversation-conversationresponsetype.md)
    
- [ConversationId](conversationid.md)
    
- [SyncState (base64Binary)](syncstate-base64binary.md)
    
- [ConversationNodes](conversationnodes.md)
    
- [ConversationNode](conversationnode.md)
    
- [InternetMessageId](internetmessageid.md)
    
- [Éléments (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [ItemId](itemid.md)
    
- [Subject](subject.md)
    
- [DateTimeReceived](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a>Réponse d’erreur d’opération GetConversationItems

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetConversationItems** pour obtenir les éléments d’une conversation qui n’existent plus dans la boîte aux lettres ou pour lesquels tous les éléments de conversation se trouvent dans des dossiers ignorés. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération de ApplyConversationAction](applyconversationaction-operation.md)
    
- [Opération FindConversation](findconversation-operation.md)
    

