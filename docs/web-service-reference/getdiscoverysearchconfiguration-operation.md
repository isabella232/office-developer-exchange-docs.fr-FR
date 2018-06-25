---
title: Opération GetDiscoverySearchConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8a54a6dc-110c-4972-a8bc-5ddb43c4b857
description: Opération de recherche plus d’informations sur la GetDiscoverySearchConfiguration EWS.
ms.openlocfilehash: a50463e575bf5a4ffdafc357d91563b0ca0486f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756573"
---
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="d4bcd-103">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="d4bcd-104">Trouvez des informations sur l’opération EWS **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4bcd-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="d4bcd-105">L’opération **GetDiscoverySearchConfiguration** renvoie contient des informations de configuration sur place, enregistré les recherches de découverte et les boîtes aux lettres qui sont activées pour la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="d4bcd-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="d4bcd-107">Utilisation de l’opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="d4bcd-108">L’opération **GetDiscoverySearchConfiguration** fournit des informations de configuration pour la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="d4bcd-109">Demandes peuvent contenir une ou plusieurs des arguments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="d4bcd-110">[La valeur SearchId](searchid.md) — identifie une recherche de découverte enregistrés.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="d4bcd-111">Si cet argument est envoyé dans la demande, les valeurs des autres arguments sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="d4bcd-112">[ExpandGroupMembership](expandgroupmembership.md) — indique si l’appartenance au groupe est développée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="d4bcd-113">La valeur **true** indique que l’appartenance au groupe est étendue afin que toutes les boîtes aux lettres de recherche sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="d4bcd-114">La valeur **false** indique que seul le groupe est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="d4bcd-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — indique si toutes les boîtes aux lettres de recherche sont renvoyés en plus de la configuration dans une archive permanente.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="d4bcd-116">La valeur **true** indique qu’uniquement les configurations de suspension en place sont retournées.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="d4bcd-117">La valeur **false** indique que tous les identificateurs de recherche de boîte aux lettres sont retournés outre les identificateurs de suspension en place.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="d4bcd-118">Si cet élément n’est pas présent, le comportement par défaut est l’équivalent de la valeur **false**.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="d4bcd-119">En-têtes SOAP GetDiscoverySearchConfiguration opération</span><span class="sxs-lookup"><span data-stu-id="d4bcd-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="d4bcd-120">L’opération **GetDiscoverySearchConfiguration** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d4bcd-121">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-121">**Header name**</span></span>|<span data-ttu-id="d4bcd-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-122">**Element**</span></span>|<span data-ttu-id="d4bcd-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d4bcd-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="d4bcd-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="d4bcd-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="d4bcd-126">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="d4bcd-127">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d4bcd-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d4bcd-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d4bcd-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d4bcd-130">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d4bcd-131">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d4bcd-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d4bcd-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d4bcd-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d4bcd-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d4bcd-134">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d4bcd-135">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="d4bcd-136">Exemple de requête d’opération GetDiscoverySearchConfiguration : obtenir la configuration de recherche de découverte d’une recherche enregistrée</span><span class="sxs-lookup"><span data-stu-id="d4bcd-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="d4bcd-137">Une demande d’opération **GetDiscoverySearchConfiguration** l’exemple suivant montre comment demander la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ».</span><span class="sxs-lookup"><span data-stu-id="d4bcd-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="d4bcd-138">Les arguments des éléments [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) [ExpandGroupMembership](expandgroupmembership.md) sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="d4bcd-139">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4bcd-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="d4bcd-141">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="d4bcd-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="d4bcd-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="d4bcd-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="d4bcd-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="d4bcd-144">Réponse d’opération GetDiscoverySearchConfiguration réussie : demander pour une seule recherche enregistrée</span><span class="sxs-lookup"><span data-stu-id="d4bcd-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="d4bcd-145">L’exemple suivant montre une réponse positive à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ».</span><span class="sxs-lookup"><span data-stu-id="d4bcd-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetDiscoverySearchConfigurationResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <DiscoverySearchConfigurations>
        <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d4bcd-146">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4bcd-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="d4bcd-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="d4bcd-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4bcd-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d4bcd-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="d4bcd-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="d4bcd-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="d4bcd-151">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="d4bcd-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="d4bcd-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="d4bcd-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="d4bcd-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="d4bcd-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="d4bcd-155">GUID</span><span class="sxs-lookup"><span data-stu-id="d4bcd-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d4bcd-156">PrimarySmtpAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d4bcd-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="d4bcd-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="d4bcd-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="d4bcd-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d4bcd-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="d4bcd-159">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d4bcd-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="d4bcd-160">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="d4bcd-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="d4bcd-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="d4bcd-162">Réponse d’opération GetDiscoverySearchConfiguration réussie : demande d’archives permanentes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="d4bcd-163">L’exemple suivant montre une réponse positive à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir uniquement des archives permanentes.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <SearchId>MyDiscSearchFor-sbrown</SearchId>
               <SearchQuery>test item</SearchQuery>
               <InPlaceHoldIdentity>3f37d90f53144558a80814ef0272749a9</InPlaceHoldIdentity>
               <ManagedByOrganization/>
            </DiscoverySearchConfiguration>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d4bcd-164">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4bcd-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="d4bcd-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="d4bcd-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4bcd-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d4bcd-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="d4bcd-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="d4bcd-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="d4bcd-169">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="d4bcd-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="d4bcd-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="d4bcd-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="d4bcd-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="d4bcd-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="d4bcd-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="d4bcd-173">Réponse d’opération GetDiscoverySearchConfiguration réussie : demander pour tous les enregistrement découverte des configurations de recherche</span><span class="sxs-lookup"><span data-stu-id="d4bcd-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="d4bcd-174">L’exemple suivant montre une réponse positive à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir toutes les recherches de découverte enregistrés.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Success" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <DiscoverySearchConfigurations>
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <DiscoverySearchConfiguration xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d4bcd-175">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4bcd-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="d4bcd-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="d4bcd-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4bcd-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d4bcd-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="d4bcd-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="d4bcd-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="d4bcd-180">Valeur SearchId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="d4bcd-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="d4bcd-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="d4bcd-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="d4bcd-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="d4bcd-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="d4bcd-184">GUID</span><span class="sxs-lookup"><span data-stu-id="d4bcd-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d4bcd-185">PrimarySmtpAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d4bcd-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="d4bcd-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="d4bcd-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="d4bcd-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d4bcd-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="d4bcd-188">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d4bcd-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="d4bcd-189">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="d4bcd-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="d4bcd-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="d4bcd-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="d4bcd-191">Réponse d’erreur d’opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="d4bcd-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="d4bcd-192">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="d4bcd-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="d4bcd-193">Il s’agit d’une réponse à une demande pour obtenir une recherche enregistrée est introuvable sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="d4bcd-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
```XML
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
      <GetDiscoverySearchConfigurationResponse ResponseClass="Error" 
                                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Search configuration corresponding to the search id was not found.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <DiscoverySearchConfigurations/>
      </GetDiscoverySearchConfigurationResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="d4bcd-194">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d4bcd-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d4bcd-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="d4bcd-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="d4bcd-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="d4bcd-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d4bcd-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d4bcd-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d4bcd-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d4bcd-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="d4bcd-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="d4bcd-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="d4bcd-200">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d4bcd-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d4bcd-201">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d4bcd-201">See also</span></span>

- [<span data-ttu-id="d4bcd-202">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d4bcd-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d4bcd-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="d4bcd-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="d4bcd-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="d4bcd-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d4bcd-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="d4bcd-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="d4bcd-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="d4bcd-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="d4bcd-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

