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
# <a name="getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="58578-103">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-103">GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="58578-104">Trouvez des informations sur l’opération EWS **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="58578-104">Find information about the **GetDiscoverySearchConfiguration** EWS operation.</span></span> 
  
<span data-ttu-id="58578-105">L’opération **GetDiscoverySearchConfiguration** renvoie les informations de configuration pour les conservations inaltérables, les recherches de découverte enregistrées et les boîtes aux lettres qui sont activées pour la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="58578-105">The **GetDiscoverySearchConfiguration** operation returns configuration information for in-place holds, saved discovery searches, and the mailboxes that are enabled for discovery search.</span></span> 
  
<span data-ttu-id="58578-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58578-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getdiscoverysearchconfiguration-operation"></a><span data-ttu-id="58578-107">Utilisation de l’opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-107">Using the GetDiscoverySearchConfiguration operation</span></span>

<span data-ttu-id="58578-108">L’opération **GetDiscoverySearchConfiguration** fournit des informations de configuration pour la recherche de découverte.</span><span class="sxs-lookup"><span data-stu-id="58578-108">The **GetDiscoverySearchConfiguration** operation provides configuration information for discovery search.</span></span> <span data-ttu-id="58578-109">Les requêtes peuvent contenir un ou plusieurs des arguments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-109">Requests can contain one or more of the following arguments:</span></span> 
  
1. <span data-ttu-id="58578-110">[SearchId](searchid.md) — identifie une recherche de découverte enregistrée.</span><span class="sxs-lookup"><span data-stu-id="58578-110">[SearchId](searchid.md) — Identifies a saved discovery search.</span></span> <span data-ttu-id="58578-111">Si cet argument est envoyé dans la demande, les valeurs des autres arguments sont ignorées.</span><span class="sxs-lookup"><span data-stu-id="58578-111">If this argument is sent in the request, the values of the other arguments are ignored.</span></span> 
    
2. <span data-ttu-id="58578-112">[ExpandGroupMembership](expandgroupmembership.md) — indique si l’appartenance au groupe est développée dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="58578-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether group membership is expanded in the response.</span></span> <span data-ttu-id="58578-113">La valeur **true** indique que l’appartenance au groupe est étendue de sorte que toutes les boîtes aux lettres pouvant faire l’objet d’une recherche soient renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="58578-113">A value of **true** indicates that group membership is expanded so that all searchable mailboxes are returned in the response.</span></span> <span data-ttu-id="58578-114">La valeur **false** indique que seul le groupe est renvoyé dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="58578-114">A value of **false** indicates that only the group is returned in the response.</span></span> 
    
3. <span data-ttu-id="58578-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — indique si toutes les boîtes aux lettres pouvant faire l’objet d’une recherche sont renvoyées en plus de la configuration de conservation inaltérable.</span><span class="sxs-lookup"><span data-stu-id="58578-115">[InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) — Indicates whether all searchable mailboxes are returned in addition to the in-place hold configuration.</span></span> <span data-ttu-id="58578-116">La valeur **true** indique que seules les configurations de conservation inaltérable sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="58578-116">A value of **true** indicates that only the in-place hold configurations are returned.</span></span> <span data-ttu-id="58578-117">La valeur **false** indique que tous les identificateurs de boîte aux lettres pouvant faire l’objet d’une recherche sont renvoyés en plus des identificateurs de conservation inaltérable.</span><span class="sxs-lookup"><span data-stu-id="58578-117">A value of **false** indicates that all searchable mailbox identifiers are returned in addition to the in-place hold identifiers.</span></span> <span data-ttu-id="58578-118">Si cet élément n’est pas présent, le comportement par défaut est l’équivalent de la valeur **false**.</span><span class="sxs-lookup"><span data-stu-id="58578-118">If this element is not present, the default behavior is the equivalent of the value **false**.</span></span> 
    
### <a name="getdiscoverysearchconfiguration-operation-soap-headers"></a><span data-ttu-id="58578-119">En-têtes SOAP d’opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-119">GetDiscoverySearchConfiguration operation SOAP headers</span></span>

<span data-ttu-id="58578-120">L’opération **GetDiscoverySearchConfiguration** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="58578-120">The **GetDiscoverySearchConfiguration** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="58578-121">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="58578-121">**Header name**</span></span>|<span data-ttu-id="58578-122">**Élément**</span><span class="sxs-lookup"><span data-stu-id="58578-122">**Element**</span></span>|<span data-ttu-id="58578-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="58578-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="58578-124">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="58578-124">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="58578-125">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="58578-125">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="58578-126">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="58578-126">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="58578-127">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="58578-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58578-128">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="58578-128">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="58578-129">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="58578-129">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="58578-130">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="58578-130">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="58578-131">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="58578-131">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58578-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="58578-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="58578-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="58578-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="58578-134">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="58578-134">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="58578-135">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="58578-135">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getdiscoverysearchconfiguration-operation-request-example-get-the-discovery-search-configuration-for-a-saved-search"></a><span data-ttu-id="58578-136">Exemple de requête d’opération GetDiscoverySearchConfiguration : obtenir la configuration de recherche de découverte pour une recherche enregistrée</span><span class="sxs-lookup"><span data-stu-id="58578-136">GetDiscoverySearchConfiguration operation request example: Get the discovery search configuration for a saved search</span></span>

<span data-ttu-id="58578-137">L’exemple suivant de demande d’opération **GetDiscoverySearchConfiguration** indique comment demander la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ».</span><span class="sxs-lookup"><span data-stu-id="58578-137">The following example of a **GetDiscoverySearchConfiguration** operation request shows how to request the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> <span data-ttu-id="58578-138">Les arguments des éléments [ExpandGroupMembership](expandgroupmembership.md) et [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) sont ignorés.</span><span class="sxs-lookup"><span data-stu-id="58578-138">The arguments for the [ExpandGroupMembership](expandgroupmembership.md) and [InPlaceHoldConfigurationOnly](inplaceholdconfigurationonly.md) elements are ignored.</span></span> 
  
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

<span data-ttu-id="58578-139">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58578-140">GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-140">GetDiscoverySearchConfiguration</span></span>](getdiscoverysearchconfiguration.md)
    
- [<span data-ttu-id="58578-141">SearchId</span><span class="sxs-lookup"><span data-stu-id="58578-141">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="58578-142">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="58578-142">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
- [<span data-ttu-id="58578-143">InPlaceHoldConfigurationOnly</span><span class="sxs-lookup"><span data-stu-id="58578-143">InPlaceHoldConfigurationOnly</span></span>](inplaceholdconfigurationonly.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-a-single-saved-search"></a><span data-ttu-id="58578-144">Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande d’une recherche enregistrée unique</span><span class="sxs-lookup"><span data-stu-id="58578-144">Successful GetDiscoverySearchConfiguration operation response: Request for a single saved search</span></span>

<span data-ttu-id="58578-145">L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir la configuration d’une recherche enregistrée appelée « MyDiscSearchFor-sbrown ».</span><span class="sxs-lookup"><span data-stu-id="58578-145">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get the configuration of a saved search called "MyDiscSearchFor-sbrown".</span></span> 
  
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

<span data-ttu-id="58578-146">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58578-147">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="58578-147">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="58578-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58578-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58578-149">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="58578-149">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="58578-150">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-150">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="58578-151">SearchId</span><span class="sxs-lookup"><span data-stu-id="58578-151">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="58578-152">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="58578-152">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="58578-153">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-153">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="58578-154">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="58578-154">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="58578-155">Guid</span><span class="sxs-lookup"><span data-stu-id="58578-155">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="58578-156">PrimarySmtpAddress (String)</span><span class="sxs-lookup"><span data-stu-id="58578-156">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="58578-157">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="58578-157">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="58578-158">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="58578-158">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="58578-159">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58578-159">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58578-160">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="58578-160">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="58578-161">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="58578-161">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-in-place-holds"></a><span data-ttu-id="58578-162">Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande de conservations inaltérables</span><span class="sxs-lookup"><span data-stu-id="58578-162">Successful GetDiscoverySearchConfiguration operation response: Request for in-place holds</span></span>

<span data-ttu-id="58578-163">L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** afin d’obtenir uniquement les conservations inaltérables.</span><span class="sxs-lookup"><span data-stu-id="58578-163">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to only get in-place holds.</span></span> 
  
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

<span data-ttu-id="58578-164">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-164">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58578-165">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="58578-165">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="58578-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58578-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58578-167">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="58578-167">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="58578-168">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-168">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="58578-169">SearchId</span><span class="sxs-lookup"><span data-stu-id="58578-169">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="58578-170">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="58578-170">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="58578-171">InPlaceHoldIdentity</span><span class="sxs-lookup"><span data-stu-id="58578-171">InPlaceHoldIdentity</span></span>](inplaceholdidentity.md)
    
- [<span data-ttu-id="58578-172">ManagedByOrganization</span><span class="sxs-lookup"><span data-stu-id="58578-172">ManagedByOrganization</span></span>](managedbyorganization.md)
    
## <a name="successful-getdiscoverysearchconfiguration-operation-response-request-for-all-saved-discovery-search-configurations"></a><span data-ttu-id="58578-173">Réponse de l’opération GetDiscoverySearchConfiguration réussie : demande pour toutes les configurations de recherche enregistrées</span><span class="sxs-lookup"><span data-stu-id="58578-173">Successful GetDiscoverySearchConfiguration operation response: Request for all saved discovery search configurations</span></span>

<span data-ttu-id="58578-174">L’exemple suivant montre une réponse réussie à une demande d’opération **GetDiscoverySearchConfiguration** pour obtenir toutes les recherches de découverte enregistrées.</span><span class="sxs-lookup"><span data-stu-id="58578-174">The following example shows a successful response to a **GetDiscoverySearchConfiguration** operation request to get all saved discovery searches.</span></span> 
  
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

<span data-ttu-id="58578-175">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-175">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58578-176">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="58578-176">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="58578-177">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58578-177">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58578-178">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="58578-178">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
- [<span data-ttu-id="58578-179">DiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-179">DiscoverySearchConfiguration</span></span>](discoverysearchconfiguration.md)
    
- [<span data-ttu-id="58578-180">SearchId</span><span class="sxs-lookup"><span data-stu-id="58578-180">SearchId</span></span>](searchid.md)
    
- [<span data-ttu-id="58578-181">SearchQuery</span><span class="sxs-lookup"><span data-stu-id="58578-181">SearchQuery</span></span>](searchquery.md)
    
- [<span data-ttu-id="58578-182">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-182">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="58578-183">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="58578-183">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="58578-184">Guid</span><span class="sxs-lookup"><span data-stu-id="58578-184">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="58578-185">PrimarySmtpAddress (String)</span><span class="sxs-lookup"><span data-stu-id="58578-185">PrimarySmtpAddress (string)</span></span>](primarysmtpaddress-string.md)
    
- [<span data-ttu-id="58578-186">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="58578-186">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="58578-187">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="58578-187">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="58578-188">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58578-188">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58578-189">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="58578-189">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="58578-190">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="58578-190">ReferenceId</span></span>](referenceid.md)
    
## <a name="getdiscoverysearchconfiguration-operation-error-response"></a><span data-ttu-id="58578-191">Réponse d’erreur d’opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="58578-191">GetDiscoverySearchConfiguration operation error response</span></span>

<span data-ttu-id="58578-192">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="58578-192">The following example shows an error response to a **GetDiscoverySearchConfiguration** operation request.</span></span> <span data-ttu-id="58578-193">Réponse à une demande d’obtention d’une recherche enregistrée qui est introuvable sur le serveur.</span><span class="sxs-lookup"><span data-stu-id="58578-193">This is a response to a request to get a saved search that is not found on the server.</span></span> 
  
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

<span data-ttu-id="58578-194">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58578-194">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58578-195">GetDiscoverySearchConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="58578-195">GetDiscoverySearchConfigurationResponse</span></span>](getdiscoverysearchconfigurationresponse.md)
    
- [<span data-ttu-id="58578-196">MessageText</span><span class="sxs-lookup"><span data-stu-id="58578-196">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="58578-197">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58578-197">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58578-198">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="58578-198">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="58578-199">DiscoverySearchConfigurations</span><span class="sxs-lookup"><span data-stu-id="58578-199">DiscoverySearchConfigurations</span></span>](discoverysearchconfigurations.md)
    
<span data-ttu-id="58578-200">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="58578-200">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="58578-201">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="58578-201">See also</span></span>

- [<span data-ttu-id="58578-202">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="58578-202">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="58578-203">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-203">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="58578-204">SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-204">SearchMailboxes</span></span>](searchmailboxes.md)
    
- [<span data-ttu-id="58578-205">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-205">GetHoldOnMailboxes</span></span>](getholdonmailboxes.md)
    
- [<span data-ttu-id="58578-206">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="58578-206">SetHoldOnMailboxes</span></span>](setholdonmailboxes.md)
    
- [<span data-ttu-id="58578-207">GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="58578-207">GetNonIndexableItemDetails</span></span>](getnonindexableitemdetails.md)
    
- [<span data-ttu-id="58578-208">GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="58578-208">GetNonIndexableItemStatistics</span></span>](getnonindexableitemstatistics.md)
    

