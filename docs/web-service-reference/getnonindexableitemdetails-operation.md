---
title: Opération GetNonIndexableItemDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9279c3ad-f7c8-4bbc-b0a7-2c78416cb39a
description: Opération de recherche plus d’informations sur la GetNonIndexableItemDetails EWS.
ms.openlocfilehash: 6b0c5afd54ac98f89bc6c5199300c20862c6f207
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756683"
---
# <a name="getnonindexableitemdetails-operation"></a>Opération GetNonIndexableItemDetails

Trouvez des informations sur l’opération EWS **GetNonIndexableItemDetails** . 
  
L’opération **GetNonIndexableItemDetails** récupère plus d’informations sur les éléments qui ne peuvent pas être indexés. Cela inclut, mais n’est pas limité à l’identificateur d’élément, un code d’erreur, une description de l’erreur lors de la tentative d’index de l’élément et des informations supplémentaires sur le fichier. 
  
> [!NOTE]
> Bien que le schéma indique que plusieurs boîtes aux lettres pouvant être recherchées, dans la version initiale d’Exchange 2013, le service prend uniquement en charge les détails des éléments lors de l’obtention des éléments nonindexable dans une seule boîte aux lettres. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getnonindexableitemdetails-operation"></a>Utilisation de l’opération GetNonIndexableItemDetails

L’opération **GetNonIndexableItemDetails** identifie les éléments de boîte aux lettres qui ne peuvent pas être indexés et fournit des informations sur la raison pour laquelle les éléments ne peuvent pas être indexés. Éléments qui ne peuvent pas être indexés ne sont pas recherchés lors d’une recherche de découverte. 
  
### <a name="getnonindexableitemdetails-operation-soap-headers"></a>En-têtes SOAP GetNonIndexableItemDetails opération

L’opération **GetNonIndexableItemDetails** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="getnonindexableitemdetails-operation-request-example-get-the-details-of-an-item-that-cannot-be-indexed"></a>Exemple de requête d’opération GetNonIndexableItemDetails : obtenir les détails d’un élément qui ne peuvent pas être indexés

Une demande d’opération **GetNonIndexableItemDetails** l’exemple suivant montre comment demander les détails des éléments qui ne peuvent pas être indexés pour une boîte aux lettres unique. La recherche est effectuée sur les deux principal et d’archivage de boîtes aux lettres. 
  
> [!NOTE]
> Tous les noms de domaine hérité dans cet exemple ont être raccourcie afin de préserver la lisibilité. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetNonIndexableItemDetails>
         <m:Mailboxes>
            <t:LegacyDN>/o=First Organization/ou=Exchange Administrative Group (FYT)/cn=Recipients/cn=35-Steve</t:LegacyDN>
         </m:Mailboxes>
         <m:SearchArchiveOnly>false</m:SearchArchiveOnly>
      </m:GetNonIndexableItemDetails>
   </soap:Body>
</soap:Envelope>

```

La demande SOAP body contient les éléments suivants :
  
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [Boîtes aux lettres (NonEmptyArrayOfLegacyDNsType)](mailboxes-nonemptyarrayoflegacydnstype.md)
    
- [LegacyDN](legacydn.md)
    
- [SearchArchiveOnly](searcharchiveonly.md)
    
## <a name="successful-getnonindexableitemdetails-operation-response"></a>Réponse d’opération GetNonIndexableItemDetails réussie

L’exemple suivant montre une réponse positive à une demande d’opération **GetNonIndexableItemDetails** pour obtenir les éléments qui ne peuvent pas être indexés pour une boîte aux lettres unique. L’élément dans cet exemple ne peuvent pas être indexé est le fichier binaryfile.abc, qui est d’un format inconnu. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <NonIndexableItemDetailsResult>
            <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <NonIndexableItemDetail>
                  <ItemId Id="AQMkAGVmNDAyOQAAAY2fUAAAAA==" ChangeKey="CQAAAA=="/>
                  <ErrorCode>DocumentParserFailure</ErrorCode>
                  <ErrorDescription>The document parser encountered a processing error.</ErrorDescription>
                  <IsPartiallyIndexed>false</IsPartiallyIndexed>
                  <IsPermanentFailure>true</IsPermanentFailure>
                  <SortValue>502511175756</SortValue>
                  <AttemptCount>0</AttemptCount>
                  <LastAttemptTime>2012-11-15T01:56:11Z</LastAttemptTime>
                  <AdditionalInfo> 301002 Error parsing document 'exchange://localhost/Attachment/d987b1f4-9aa7-42b3-aa8c-9515a35dfa1a/1f3047d4-c287-41e4-910c-feb70c1a59f0/ef402830-3d33-4a0d-a4e9-d8576900060d/85b83861-0026-418f-8464-be2036696333/502511175756.0/binaryfile.abc'. Document has an undetectable format and will not be parsed.</AdditionalInfo>
               </NonIndexableItemDetail>
            </Items>
         </NonIndexableItemDetailsResult>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>

```

La réponse SOAP body contient les éléments suivants :
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [NonIndexableItemDetailsResult](nonindexableitemdetailsresult.md)
    
- [NonIndexableItemDetail](nonindexableitemdetail.md)
    
- [ID d’élément](itemid.md)
    
- [ErrorCode (ItemIndexErrorType)](errorcode-itemindexerrortype.md)
    
- [ErrorDescription](errordescription.md)
    
- [IsPartiallyIndexed](ispartiallyindexed.md)
    
- [IsPermanentFailure](ispermanentfailure.md)
    
- [SortValue](sortvalue.md)
    
- [AttemptCount](attemptcount.md)
    
- [LastAttemptTime](lastattempttime.md)
    
- [AdditionalInfo](additionalinfo.md)
    
## <a name="getnonindexableitemdetails-operation-error-response"></a>Réponse d’erreur d’opération GetNonIndexableItemDetails

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetNonIndexableItemDetails** . Il s’agit d’une réponse à une demande pour obtenir des détails des éléments pour les éléments qui ne peuvent pas être indexés à partir de plusieurs boîtes aux lettres. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetNonIndexableItemDetailsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Multiple mailboxes is currently not supported, only single mailbox is supported.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetNonIndexableItemDetailsResponse>
   </s:Body>
</s:Envelope>
```

La réponse d’erreur corps SOAP contient les éléments suivants :
  
- [GetNonIndexableItemDetailsResponse](getnonindexableitemdetailsresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [Opération GetSearchableMailboxes](getsearchablemailboxes-operation.md)
    
- [Opération SearchMailboxes](searchmailboxes-operation.md)
    
- [Opération GetHoldOnMailboxes](getholdonmailboxes-operation.md)
    
- [Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md)
    
- [Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)
    
- [Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

