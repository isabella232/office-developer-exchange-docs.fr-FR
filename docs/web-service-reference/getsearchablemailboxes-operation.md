---
title: Opération GetSearchableMailboxes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 47f8ff57-4835-4d2d-9136-44afb31a4cbe
description: Opération de recherche plus d’informations sur la GetSearchableMailboxes EWS.
ms.openlocfilehash: 5e14288280b23e2555eea4fce0f77743d7d210ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756736"
---
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="277d5-103">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-103">GetSearchableMailboxes operation</span></span>

<span data-ttu-id="277d5-104">Trouvez des informations sur l’opération EWS **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="277d5-104">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="277d5-105">L’opération **GetSearchableMailboxes** Obtient un jeu d’étendue de recherche boîtes aux lettres pour les recherches de découverte.</span><span class="sxs-lookup"><span data-stu-id="277d5-105">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="277d5-106">L’étendue de recherche boîtes aux lettres retourné dans la réponse est déterminée par le filtre de recherche et si l’appartenance au groupe de distribution est développée.</span><span class="sxs-lookup"><span data-stu-id="277d5-106">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 
  
<span data-ttu-id="277d5-107">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="277d5-107">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="277d5-108">Utilisation de l’opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-108">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="277d5-109">L’opération **GetSearchableMailboxes** Obtient des informations sur les boîtes aux lettres de recherche.</span><span class="sxs-lookup"><span data-stu-id="277d5-109">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="277d5-110">Les arguments suivants peuvent être passés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="277d5-110">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="277d5-111">[SearchFilter](searchfilter.md) — accepte un alias de messagerie unique en tant qu’argument.</span><span class="sxs-lookup"><span data-stu-id="277d5-111">[SearchFilter](searchfilter.md) —Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="277d5-112">[ExpandGroupMembership](expandgroupmembership.md) — indique si l’appartenance au groupe de distribution est développée dans les résultats renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="277d5-112">[ExpandGroupMembership](expandgroupmembership.md) — Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="277d5-113">Si l’alias de messagerie définies dans le filtre de recherche est un groupe de distribution et les appartenances aux groupes de distribution n’est pas développé, la réponse contient les informations de boîte aux lettres pour le groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="277d5-113">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="277d5-114">Si l’alias de messagerie définies dans le filtre de recherche est un groupe de distribution et les appartenances aux groupes de distribution est développée, la réponse contient les informations de boîte aux lettres pour chaque boîte aux lettres qui est un membre du groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="277d5-114">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="277d5-115">Si le filtre de recherche contient des alias d’un utilisateur unique, la réponse contient les informations de boîte aux lettres de l’utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="277d5-115">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="277d5-116">La réponse contient toutes les boîtes aux lettres recherche si l’élément [GetSearchableMailboxes](getsearchablemailboxes.md) est vide.</span><span class="sxs-lookup"><span data-stu-id="277d5-116">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="277d5-117">Il s’agit de la même comme ayant un élément [SearchFilter](searchfilter.md) vide et l’élément [ExpandGroupMembership](expandgroupmembership.md) la valeur **false**.</span><span class="sxs-lookup"><span data-stu-id="277d5-117">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="277d5-118">En-têtes SOAP GetSearchableMailboxes opération</span><span class="sxs-lookup"><span data-stu-id="277d5-118">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="277d5-119">L’opération **GetSearchableMailboxes** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="277d5-119">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="277d5-120">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="277d5-120">**Header name**</span></span>|<span data-ttu-id="277d5-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="277d5-121">**Element**</span></span>|<span data-ttu-id="277d5-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="277d5-122">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="277d5-123">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="277d5-123">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="277d5-124">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="277d5-124">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="277d5-125">Identifie les rôles de serveur qui sont nécessaires pour l’appelant effectuer la demande.</span><span class="sxs-lookup"><span data-stu-id="277d5-125">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="277d5-126">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="277d5-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="277d5-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="277d5-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="277d5-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="277d5-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="277d5-129">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="277d5-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="277d5-130">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="277d5-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="277d5-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="277d5-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="277d5-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="277d5-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="277d5-133">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="277d5-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="277d5-134">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="277d5-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="277d5-135">Exemple de requête d’opération GetSearchableMailboxes : demander des informations sur un groupe de distribution</span><span class="sxs-lookup"><span data-stu-id="277d5-135">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="277d5-136">Une demande d’opération **GetSearchableMailboxes** l’exemple suivant montre comment obtenir les informations de boîte aux lettres pour le groupe de distribution lolgroup.</span><span class="sxs-lookup"><span data-stu-id="277d5-136">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="277d5-137">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="277d5-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="277d5-138">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-138">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)
    
- [<span data-ttu-id="277d5-139">SearchFilter</span><span class="sxs-lookup"><span data-stu-id="277d5-139">SearchFilter</span></span>](searchfilter.md)
    
- [<span data-ttu-id="277d5-140">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="277d5-140">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="277d5-141">Réponse d’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution</span><span class="sxs-lookup"><span data-stu-id="277d5-141">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="277d5-142">L’exemple suivant montre une réponse positive à une demande d’opération **GetSearchableMailboxes** pour obtenir les informations de découverte pour le groupe de distribution lolgroup.</span><span class="sxs-lookup"><span data-stu-id="277d5-142">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Success" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <SearchableMailboxes>
            <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="277d5-143">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="277d5-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="277d5-144">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="277d5-144">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="277d5-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="277d5-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="277d5-146">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-146">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="277d5-147">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="277d5-147">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="277d5-148">GUID</span><span class="sxs-lookup"><span data-stu-id="277d5-148">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="277d5-149">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="277d5-149">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="277d5-150">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="277d5-150">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="277d5-151">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="277d5-151">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="277d5-152">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="277d5-152">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="277d5-153">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="277d5-153">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="277d5-154">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="277d5-154">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="277d5-155">Réponse d’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution développé</span><span class="sxs-lookup"><span data-stu-id="277d5-155">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="277d5-156">L’exemple suivant montre une réponse positive à une demande d’opération **GetSearchableMailboxes** pour obtenir les informations de découverte sur les membres du groupe de distribution lolgroup étendue.</span><span class="sxs-lookup"><span data-stu-id="277d5-156">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="526" MinorBuildNumber="0" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetSearchableMailboxesResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <SearchableMailboxes>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>e2d42cdf-a227-1ec3-486b-6fa0ebaadb9f5</Guid>
          <PrimarySmtpAddress>JSmith@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Julia Smith</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=0a1fc86f883846152405d60956dd02e7-Julia</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Guid>45d0fff1-6541-459a-a343-52453b30e12ca</Guid>
          <PrimarySmtpAddress>LMoore@contoso.com</PrimarySmtpAddress>
          <IsExternalMailbox>false</IsExternalMailbox>
          <ExternalEmailAddress/>
          <DisplayName>Laura Moore</DisplayName>
          <IsMembershipGroup>false</IsMembershipGroup>
          <ReferenceId>/o=First Organization/ou=Exchange Administrative Group (FYDLT)/cn=Recipients/cn=2910d8f8316f4378bbf9338d8f9d714b-Laura</ReferenceId>
        </SearchableMailbox>
        <SearchableMailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="277d5-157">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="277d5-157">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="277d5-158">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="277d5-158">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="277d5-159">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="277d5-159">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="277d5-160">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-160">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
- [<span data-ttu-id="277d5-161">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="277d5-161">SearchableMailbox</span></span>](searchablemailbox.md)
    
- [<span data-ttu-id="277d5-162">GUID</span><span class="sxs-lookup"><span data-stu-id="277d5-162">Guid</span></span>](guid-ex15websvcsotherref.md)
    
- [<span data-ttu-id="277d5-163">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="277d5-163">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)
    
- [<span data-ttu-id="277d5-164">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="277d5-164">IsExternalMailbox</span></span>](isexternalmailbox.md)
    
- [<span data-ttu-id="277d5-165">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="277d5-165">ExternalEmailAddress</span></span>](externalemailaddress.md)
    
- [<span data-ttu-id="277d5-166">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="277d5-166">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="277d5-167">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="277d5-167">IsMembershipGroup</span></span>](ismembershipgroup.md)
    
- [<span data-ttu-id="277d5-168">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="277d5-168">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="277d5-169">Réponse d’erreur d’opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-169">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="277d5-170">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="277d5-170">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="277d5-171">Il s’agit d’une réponse à une demande pour obtenir toutes les boîtes aux lettres recherche lorsque l’argument **ExpandGroupMembership** est défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="277d5-171">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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
      <GetSearchableMailboxesResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot use wildcard or empty query when auto group expansion is enabled.</MessageText>
         <ResponseCode>ErrorInvalidArgument</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <SearchableMailboxes/>
      </GetSearchableMailboxesResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="277d5-172">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="277d5-172">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="277d5-173">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="277d5-173">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)
    
- [<span data-ttu-id="277d5-174">MessageText</span><span class="sxs-lookup"><span data-stu-id="277d5-174">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="277d5-175">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="277d5-175">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="277d5-176">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="277d5-176">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="277d5-177">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-177">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="277d5-178">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="277d5-178">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="277d5-179">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="277d5-179">See also</span></span>

- [<span data-ttu-id="277d5-180">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="277d5-180">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="277d5-181">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-181">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)
    
- [<span data-ttu-id="277d5-182">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-182">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)
    
- [<span data-ttu-id="277d5-183">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="277d5-183">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)
    
- [<span data-ttu-id="277d5-184">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="277d5-184">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)
    
- [<span data-ttu-id="277d5-185">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="277d5-185">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)
    
- [<span data-ttu-id="277d5-186">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="277d5-186">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

