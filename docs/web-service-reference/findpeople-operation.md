---
title: Opération FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Opération de recherche plus d’informations sur la FindPeople EWS.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756416"
---
# <a name="findpeople-operation"></a>Opération FindPeople

Trouvez des informations sur l’opération EWS **FindPeople** . 
  
L’opération **FindPeople** renvoie tous les objets personnage d’un dossier de Contacts spécifié ou récupère les contacts qui correspondent à une chaîne de requête spécifiée. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-findpeople-operation"></a>Utilisation de l’opération FindPeople

L’opération **FindPeople** renvoie des informations de contact agrégées. 
  
L’opération **FindPeople** s’appuie sur les fonctionnalités actuelles des [Restriction](restriction.md) et [BaseShape](baseshape.md) des types complexes en ajoutant une restriction de l’agrégation et la capacité à renvoyer des propriétés supplémentaires. En utilisant une restriction, un client peut spécifier des filtres, tels que « uniquement retourner des résultats qui ont une adresse de messagerie instantanée ». Le comportement de recherche par défaut cible de boîte aux lettres personnelle de l’utilisateur spécifié et de la liste d’adresses globale (LAG). Lors de la recherche de la liste d’adresses globale en tant que le dossier de recherche principal, vous devez spécifier une chaîne de requête au lieu d’une restriction, car cette opération ne permet pas de navigation de la liste d’adresses globale. 
  
### <a name="findpeople-operation-soap-headers"></a>En-têtes SOAP FindPeople opération

L’opération **FindPeople** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**Emprunt d’identité** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Identifie l’utilisateur emprunte l’identité de l’application cliente. Cet en-tête est applicable à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version du schéma pour la requête d’opération. Cet en-tête est applicable à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête est applicable à une réponse.  <br/> |
   
## <a name="findpeople-operation-request-example"></a>Exemple de requête d’opération FindPeople

Une demande d’opération **FindPeople** l’exemple suivant montre comment renvoyer les 100 premières contacts du dossier Contacts. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

La demande SOAP body contient les éléments suivants :
  
- [FindPeople](findpeople.md)
    
- [IndexedPageItemView](indexedpageitemview.md)
    
- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)
    
- [DistinguishedFolderId](distinguishedfolderid.md)
    
Une demande d’opération **FindPeople** l’exemple suivant montre comment renvoyer les 100 premières contacts à partir de la liste d’adresses globale à l’aide d’une chaîne de requête. Définition de la **DistinguishedFolderId** « répertoire » recherche la liste d’adresses globale comme principale source de personnages. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a>Réponse d’opération FindPeople réussie

L’exemple suivant montre une réponse positive à une demande d’opération **FindPeople** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

La réponse SOAP body contient les éléments suivants :
  
- [FindPeopleResponse](findpeopleresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [Personnes](people.md)
    
- [Personnage](persona.md)
    
- [PersonaId](personaid.md)
    
- [CreationTime](creationtime.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [DisplayNameFirstLast](displaynamefirstlast.md)
    
- [DisplayNameLastFirst](displaynamelastfirst.md)
    
- [Classer sous](fileas.md)
    
- [Prénom](givenname.md)
    
- [Surname](surname.md)
    
- [EmailAddresses (ArrayOfEmailAddressesType)](emailaddresses-arrayofemailaddressestype.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [Nom (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (EmailAddressType)](emailaddress-emailaddresstype.md)
    
- [RoutingType (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [RelevanceScore](relevancescore.md)
    
- [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a>Réponse d’erreur d’opération FindPeople

Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Personnes et contacts dans EWS dans Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Opération GetPersona](getpersona-operation.md)
    

