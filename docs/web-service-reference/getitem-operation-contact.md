---
title: Opération de GetItem (contacts)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: 6b96dace-1260-4b83-869a-7c31c5583daa
description: L'opération GetItem est utilisée pour obtenir des éléments de contact à partir de la banque d'informations Exchange.
ms.openlocfilehash: 8d7436421f0c54a49345e8ef6b37cb442bca4277
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756658"
---
# <a name="getitem-operation-contact"></a>Opération de GetItem (contacts)

Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'opération GetItem est utilisée pour obtenir des éléments de contact à partir de la banque d'informations Exchange.
  
## <a name="getitem-contact-request-example"></a>Exemple de requête GetItem (contacts)

### <a name="description"></a>Description

L'exemple suivant montre comment obtenir un élément à partir de la banque d'informations Exchange.
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABY" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

La demande pour obtenir un élément à partir de la banque d'informations Exchange prend la même forme pour tous les types d'élément. Les réponses aux demandes de différents éléments sera différents, car les différents éléments renvoient des informations différentes selon les formes de la réponse.
  
> [!NOTE]
> [!REMARQUE] Identificateur de l'élément a été raccourcie afin de préserver la lisibilité. 
  
### <a name="request-elements"></a>Éléments de la demande

Les éléments suivants sont utilisés dans la demande :
  
- [GetItem](getitem.md)
    
- [ItemShape](itemshape.md)
    
- [BaseShape](baseshape.md)
    
- [ItemId](itemids.md)
    
- [ID d’élément](itemid.md)
    
## <a name="successful-getitem-contact-response"></a>Réponse de réussite GetItem (contacts)

### <a name="description"></a>Description

L'exemple de code suivant montre une réponse positive de GetItem pour l' **AllProperties**[BaseShape](baseshape.md).
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAEA=" ChangeKey="EQAAABYq" />
              <t:ParentFolderId Id="AQAtAEFk==" ChangeKey="AQAAAA==" />
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text" />
              <t:DateTimeReceived>2006-08-18T17:31:18Z</t:DateTimeReceived>
              <t:Size>382</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>true</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-08-18T17:31:18Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-08-18T17:31:18Z</t:DateTimeCreated>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en</t:Culture>
              <t:FileAs>SampleContact</t:FileAs>
              <t:FileAsMapping>None</t:FileAsMapping>
              <t:DisplayName>Tanja Plate</t:DisplayName>
              <t:GivenName>Tanja</t:GivenName>
              <t:Initials>T.P.</t:Initials>
              <t:CompleteName>
                <t:FirstName>Tanja</t:FirstName>
                <t:LastName>Plate</t:LastName>
                <t:Initials>T.P.</t:Initials>
                <t:FullName>Tanja Plate</t:FullName>
              </t:CompleteName>
              <t:CompanyName>Northwind Traders</t:CompanyName>
              <t:EmailAddresses>
                <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
                <t:Entry Key="EmailAddress2">tplate@example.com</t:Entry>
              </t:EmailAddresses>
              <t:PhysicalAddresses>
                <t:Entry Key="Business">
                  <t:Street>12345 67th Ave</t:Street>
                  <t:City>Whittier</t:City>
                  <t:State>CA</t:State>
                  <t:Country>USA</t:Country>
                </t:Entry>
              </t:PhysicalAddresses>
              <t:PhoneNumbers>
                <t:Entry Key="BusinessPhone">5625550199</t:Entry>
              </t:PhoneNumbers>
              <t:JobTitle>Project Manager</t:JobTitle>
              <t:Surname>Plate</t:Surname>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.
  
### <a name="successful-response-elements"></a>Éléments de réponse réussie

Les éléments suivants sont utilisés dans la réponse à une demande de GetItem avec une forme de réponse de **AllProperties** pour un élément de contact. 
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetItemResponse](getitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetItemResponseMessage](getitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Items](items.md)
    
- [Contact](contact.md)
    
- [ID d’élément](itemid.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [ItemClass](itemclass.md)
    
- [Sensitivity](sensitivity.md)
    
- [Corps](body.md)
    
- [DateTimeReceived](datetimereceived.md)
    
- [Taille](size.md)
    
- [Importance](importance.md)
    
- [IsSubmitted](issubmitted.md)
    
- [IsDraft](isdraft.md)
    
- [IsFromMe](isfromme.md)
    
- [IsResend](isresend.md)
    
- [IsUnmodified](isunmodified.md)
    
- [DateTimeSent](datetimesent.md)
    
- [DateTimeCreated](datetimecreated.md)
    
- [HasAttachments](hasattachments.md)
    
- [Culture](culture.md)
    
- [Classer sous](fileas.md)
    
- [FileAsMapping](fileasmapping.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [Prénom](givenname.md)
    
- [Initials](initials.md)
    
- [CompleteName](completename.md)
    
- [Prénom](firstname.md)
    
- [LastName](lastname.md)
    
- [FullName](fullname.md)
    
- [CompanyName](companyname.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Entrée (EmailAddress)](entry-emailaddress.md)
    
- [PhysicalAddresses](physicaladdresses.md)
    
- [Entrée (PhysicalAddress)](entry-physicaladdress.md)
    
- [Street](street.md)
    
- [Ville](city.md)
    
- [State](state-ex15websvcsotherref.md)
    
- [Countryorregion définit](countryorregion.md)
    
- [PhoneNumbers](phonenumbers.md)
    
- [Entrée (PhoneNumber)](entry-phonenumber.md)
    
- [JobTitle](jobtitle.md)
    
- [Surname](surname.md)
    
## <a name="invalid-getitem-contact-request-example"></a>Exemple de requête non valide GetItem (contacts)

### <a name="description"></a>Description

L'exemple de code suivant illustre une demande non valide.
  
### <a name="code"></a>Code

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABq" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Commentaires

Identificateurs d'éléments ont été raccourcies afin de préserver la lisibilité.
  
## <a name="getitem-contact-error-response"></a>Réponse d’erreur GetItem (contacts)

### <a name="description"></a>Description

L'exemple de code suivant montre une réponse d'erreur à une demande de GetItem (contacts).
  
### <a name="code"></a>Code

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Mime conversion is not supported for this item type.</m:MessageText>
          <m:ResponseCode>ErrorUnsupportedMimeConversion</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Éléments de réponse d’erreur

Les éléments suivants sont utilisés dans la réponse d'erreur :
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetItemResponse](getitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetItemResponseMessage](getitemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [Items](items.md)
    
## <a name="see-also"></a>Voir aussi



[GetItem Operation](getitem-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

