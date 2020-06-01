---
title: Opération GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Trouvez des informations sur l’opération EWS GetDiscoverySearchConfiguration.
ms.openlocfilehash: 4db435988a9954b921e7851986b6f92ffedbad94
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461022"
---
# <a name="getdiscoverysearchconfiguration-operation"></a>Opération GetDiscoverySearchConfiguration

Trouvez des informations sur l’opération EWS **GetDiscoverySearchConfiguration** . 
  
L’opération **GetDiscoverySearchConfiguration** renvoie les informations de configuration pour les conservations inaltérables, les recherches de découverte enregistrées et les boîtes aux lettres qui sont activées pour la recherche de découverte. 
  
Cette opération est une nouveauté d’Exchange Server 2013.
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a>Utilisation de l’opération GetDiscoverySearchConfiguration

L’opération **GetDiscoverySearchConfiguration** fournit des informations de configuration pour la recherche de découverte. Les requêtes peuvent contenir un ou plusieurs des arguments suivants : 
  
1. [SearchId](searchid.md) — identifie une recherche de découverte enregistrée. Si cet argument est envoyé dans la demande, les valeurs des autres arguments sont ignorées. 
    
2. [ExpandGroupMembership](expandgroupmembership.md) — indique si l’appartenance au groupe est développée dans la réponse. La valeur **true** indique que l’appartenance au groupe est étendue de sorte que toutes les boîtes aux lettres pouvant faire l’objet d’une recherche soient renvoyées dans la réponse. La valeur **false** indique que seul le groupe est renvoyé dans la réponse. 
    
3. [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — indique si toutes les boîtes aux lettres pouvant faire l’objet d’une recherche sont renvoyées en plus de la configuration de conservation inaltérable. La valeur **true** indique que seules les configurations de conservation inaltérable sont renvoyées. La valeur **false** indique que tous les identificateurs de boîte aux lettres pouvant faire l’objet d’une recherche sont renvoyés en plus des identificateurs de conservation inaltérable. Si cet élément n’est pas présent, le comportement par défaut est l’équivalent de la valeur **false**. 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a>En-têtes SOAP d’opération GetDiscoverySearchConfiguration

L’opération **GetDiscoverySearchConfiguration** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant. 
  
|**Nom de l'en-tête**|**Élément**|**Description**|
|:-----|:-----|:-----|
|**ManagementRole** <br/> |[ManagementRole](managementrole.md) <br/> |Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande. Cet en-tête s’applique à une demande.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Identifie la version de schéma de la demande d’opération. Cet en-tête s’applique à une demande.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Identifie la version du serveur qui a répondu à la demande. Cet en-tête s’applique à une réponse.  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a>Exemple de requête d’opération GetDiscoverySearchConfiguration : obtenir la configuration de recherche de découverte pour une recherche enregistrée

L’exemple suivant de demande d’opération **GetDiscoverySearchConfiguration** indique comment demander la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ». Les arguments des éléments [ExpandGroupMembership](expandgroupmembership.md) et [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) sont ignorés. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetDiscoverySearchConfiguration>
         <m:SearchId>MyDiscSearchFor-sbrown</m:SearchId>
         <m:ExpandGroupMembership>true</m:ExpandGroupMembership>
         <m:InPlaceHoldConfigurationOnly>false</m:InPlaceHoldConfigurationOnly>
      </m:GetDiscoverySearchConfiguration>
   </soap:Body>
</soap:Envelope>

```

Le corps SOAP de la demande contient les éléments suivants :
  
- [GetDiscoverySearchConfiguration](getdiscoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [ExpandGroupMembership](expandgroupmembership.md)
    
- [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a>Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande d’une recherche enregistrée unique

L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ». 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <SearchId>MyDiscSearchFor-sbrown</SearchId>
          <SearchQuery>test item</SearchQuery>
          <SearchableMailboxes>
            <SearchableMailbox>
              <Guid>3c620d04-8b22-432e-92be-5b9321599576</Guid>
              <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
              <IsExternalMailbox>false</IsExternalMailbox>
              <ExternalEmailAddress/>
              <DisplayName>Steven Brown</DisplayName>
              <IsMembershipGroup>false</IsMembershipGroup>
              <ReferenceId>/o=First/ou=Exchange(FYDILT)/cn=Recipients/cn=313ecf-Steve</ReferenceId>
            </SearchableMailbox>
          </SearchableMailboxes>
        </DiscoverySearchConfiguration>
      </DiscoverySearchConfigurations>
    </GetDiscoverySearchConfigurationResponse>
  </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (String)](primarysmtpaddress-string.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a>Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande de conservations inaltérables

L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** afin d’obtenir uniquement les conservations inaltérables. 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <InPlaceHoldIdentity>6ea486f0f3f140efb044682a2e782abdf</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [InPlaceHoldIdentity](inplaceholdidentity.md)
    
- [ManagedByOrganization](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a>Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande pour toutes les configurations de recherche enregistrées

L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir toutes les recherches de découverte enregistrées. 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>3c620d04-8b33-435e-95be-5b9351599576</Guid>
                     <PrimarySmtpAddress>SBrown@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Steven Brown</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=35381a742f0e47e395c8601a60d13ecz-Steve</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearch</SearchId>
               <SearchQuery>test</SearchQuery>
               <SearchableMailboxes>
                  <SearchableMailbox>
                     <Guid>e788c4b0-54a2-458c-83b2-22d5bb02b23f</Guid>
                     <PrimarySmtpAddress>Administrator@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Administrator</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=ebez7871332d4595abe1c62962911a58-Admin</ReferenceId>
                  </SearchableMailbox>
                  <SearchableMailbox>
                     <Guid>6f6cff39-8967-4a60-b43f-328413c25199</Guid>
                     <PrimarySmtpAddress>ADavis@contoso.com</PrimarySmtpAddress>
                     <IsExternalMailbox>false</IsExternalMailbox>
                     <ExternalEmailAddress/>
                     <DisplayName>Anthony Davis</DisplayName>
                     <IsMembershipGroup>false</IsMembershipGroup>
                     <ReferenceId>/o=First/ou=Exchange (FYLT)/cn=Recipients/cn=f10c9f70519844beb04101d8f40c572z-Antho</ReferenceId>
                  </SearchableMailbox>
               </SearchableMailboxes>
            </DiscoverySearchConfiguration>
         </DiscoverySearchConfigurations>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>
```

Le corps SOAP de réponse contient les éléments suivants :
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
- [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
    
- [SearchId](searchid.md)
    
- [SearchQuery](searchquery.md)
    
- [SearchableMailboxes](searchablemailboxes.md)
    
- [SearchableMailbox](searchablemailbox.md)
    
- [Guid](guid-ex15websvcsotherref.md)
    
- [PrimarySmtpAddress (String)](primarysmtpaddress-string.md)
    
- [IsExternalMailbox](isexternalmailbox.md)
    
- [ExternalEmailAddress](externalemailaddress.md)
    
- [DisplayName (chaîne)](displayname-string.md)
    
- [IsMembershipGroup](ismembershipgroup.md)
    
- [ReferenceId](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a>Réponse d’erreur d’opération GetDiscoverySearchConfiguration

L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetDiscoverySearchConfiguration** . Réponse à une demande d’obtention d’une recherche enregistrée qui est introuvable sur le serveur. 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

Le corps SOAP de la réponse d’erreur contient les éléments suivants :
  
- [GetDiscoverySearchConfigurationResponse](getdiscoverysearchconfigurationresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [DiscoverySearchConfigurations](discoverysearchconfigurations.md)
    
Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>Voir aussi

- [Opérations EWS dans Exchange](ews-operations-in-exchange.md)
    
- [GetSearchableMailboxes](getsearchablemailboxes.md)
    
- [SearchMailboxes](searchmailboxes.md)
    
- [GetHoldOnMailboxes](getholdonmailboxes.md)
    
- [SetHoldOnMailboxes](setholdonmailboxes.md)
    
- [GetNonIndexableItemDetails](getnonindexableitemdetails.md)
    
- [GetNonIndexableItemStatistics](getnonindexableitemstatistics.md)
    

