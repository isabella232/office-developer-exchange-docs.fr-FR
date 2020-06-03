---
title: Opération GetSearchableMailboxes
manager: sethgros
ms.date: 01/24/2020
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Trouvez des informations sur l’opération EWS GetSearchableMailboxes.
ms.openlocfilehash: e893a66eb1b638479eeccc6bd7548cb020f37243
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530838"
---
# <a name="getsearchablemailboxes-operation"></a>Opération GetSearchableMailboxes

> [!IMPORTANT]
> À partir du 1er avril 2020, l’opération GetSearchableMailboxes ne sera plus disponible dans Exchange Online. Cette opération ne sera pas affectée dans les versions locales d’Exchange Server. Pour plus d’informations, reportez-vous à la section [retraite des outils eDiscovery hérités dans Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).

Trouvez des informations sur l’opération EWS **GetSearchableMailboxes** . 
  
L’opération **GetSearchableMailboxes** obtient un ensemble d’étendues de boîtes aux lettres pouvant faire l’objet d’une recherche pour les recherches de découverte. L’étendue des boîtes aux lettres pouvant faire l’objet d’une recherche renvoyée dans la réponse est déterminée par le filtre de recherche et par le fait que l’appartenance au groupe de distribution est développée ou non. 

> [!NOTE] 
> Cette opération est destinée à être utilisée avec le filtre de recherche et pour récupérer uniquement les quelques premières milliers ; elle n’est pas destinée à une extraction exhaustive.
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getsearchablemailboxes-operation"></a>Utilisation de l’opération GetSearchableMailboxes

L’opération **GetSearchableMailboxes** obtient des informations sur les boîtes aux lettres pouvant faire l’objet d’une recherche. Les arguments suivants peuvent être transmis dans la demande : 
  
- [Unsearchfilter](searchfilter.md) -accepte un seul alias de courrier électronique en tant qu’argument. 
    
- [ExpandGroupMembership](expandgroupmembership.md) -indique si l’appartenance au groupe de distribution est développée dans les résultats renvoyés dans la réponse. 
    
Si le jeu d’alias de messagerie du filtre de recherche est un groupe de distribution et que l’appartenance au groupe de distribution n’est pas développée, la réponse contiendra les informations de boîte aux lettres du groupe de distribution. Si le jeu d’alias de messagerie du filtre de recherche est un groupe de distribution et que l’appartenance au groupe de distribution est étendue, la réponse contient les informations de boîte aux lettres de chaque boîte aux lettres membre du groupe de distribution. Si le filtre de recherche contient l’alias d’un seul utilisateur, la réponse contiendra les informations de boîte aux lettres de l’utilisateur. La réponse contiendra toutes les boîtes aux lettres pouvant faire l’objet d’une recherche si l’élément [GetSearchableMailboxes](getsearchablemailboxes.md) est vide. Cela revient à avoir un élément [unsearchfilter](searchfilter.md) vide et l’élément [ExpandGroupMembership](expandgroupmembership.md) définis sur **false**.
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a>En-têtes SOAP d’opération GetSearchableMailboxes

L’opération **GetSearchableMailboxes** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|Nom de l’en-tête|Élément|Description|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a>Exemple de requête d’opération GetSearchableMailboxes : demander des informations sur un groupe de distribution

L’exemple suivant de demande d’opération **GetSearchableMailboxes** indique comment obtenir les informations de boîte aux lettres pour le groupe de distribution lolgroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetSearchableMailboxes>
         <m:SearchFilter>lolgroup</m:SearchFilter>
         <m:ExpandGroupMembership>false</m:ExpandGroupMembership>
      </m:GetSearchableMailboxes>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la demande contient les éléments suivants :
  
- [GetSearchableMailboxes](getsearchablemailboxes.md)   
- [Unsearchfilter](searchfilter.md)    
- [ExpandGroupMembership](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a>Réponse de l’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution

L’exemple suivant montre une réponse réussie à une demande d’opération **GetSearchableMailboxes** afin d’obtenir les informations de découverte pour le groupe de distribution lolgroup. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Guid>33a408fe-2574-4e3b-49f5-5e1e000a3035</Guid>
               <PrimarySmtpAddress>LOLgroup@contoso.com</PrimarySmtpAddress>
               <IsExternalMailbox>false</IsExternalMailbox>
               <ExternalEmailAddress/>
               <DisplayName>LOLgroup</DisplayName>
               <IsMembershipGroup>true</IsMembershipGroup>
               <ReferenceId>/o=First/ou=Exchange(FYLT)/cn=Recipients/cn=81213b958a0b5295b13b3f02b812bf1bc-LOLgroup</ReferenceId>
            </SearchableMailbox>
         </SearchableMailboxes>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)   
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)   
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (chaîne)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a>Réponse de l’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution étendu

L’exemple suivant montre une réponse réussie à une demande d’opération **GetSearchableMailboxes** pour obtenir les informations de découverte sur les membres du groupe de distribution lolgroup étendu. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>3c620d04-8b33-435a-95be-5b939375576</Guid>
          <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Steven Brown</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=90312341a742f0e47e392c80a60d13ecf-Steve</ReferenceId>
        </SearchableMailbox>
      </SearchableMailboxes>
    </GetSearchableMailboxesResponse>
  </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)    
- [ResponseCode](responsecode.md)   
- [SearchableMailboxes](searchablemailboxes.md)    
- [SearchableMailbox](searchablemailbox.md)    
- [Guid](guid-ex15websvcsotherref.md)    
- [PrimarySmtpAddress](primarysmtpaddress.md)    
- [IsExternalMailbox](isexternalmailbox.md)    
- [ExternalEmailAddress](externalemailaddress.md)    
- [DisplayName (chaîne)](displayname-string.md)    
- [IsMembershipGroup](ismembershipgroup.md)    
- [ReferenceId](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a>Réponse d’erreur d’opération GetSearchableMailboxes

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetSearchableMailboxes** . Réponse à une demande d’obtention de toutes les boîtes aux lettres pouvant faire l’objet d’une recherche lorsque l’argument **ExpandGroupMembership** est défini sur **true**. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526"
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [GetSearchableMailboxesResponse](getsearchablemailboxesresponse.md)  
- [MessageText](messagetext.md)   
- [ResponseCode](responsecode.md)   
- [DescriptiveLinkKey](descriptivelinkkey.md) 
- [SearchableMailboxes](searchablemailboxes.md)
    
Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)   
- [Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md)   
- [Opération SearchMailboxes](searchmailboxes-operation.md)   
- [Opération GetHoldOnMailboxes](getholdonmailboxes-operation.md)    
- [Opération GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration-operation.md)   
- [Opération GetNonIndexableItemDetails](getnonindexableitemdetails-operation.md)   
- [Opération GetNonIndexableItemStatistics](getnonindexableitemstatistics-operation.md)
    

