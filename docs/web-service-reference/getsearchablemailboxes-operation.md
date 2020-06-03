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
# <a name="getsearchablemailboxes-operation"></a><span data-ttu-id="1aa61-103">Opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-103">GetSearchableMailboxes operation</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1aa61-104">À partir du 1er avril 2020, l’opération GetSearchableMailboxes ne sera plus disponible dans Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="1aa61-104">Starting on April 1, 2020, the GetSearchableMailboxes operation will no longer be available in Exchange Online.</span></span> <span data-ttu-id="1aa61-105">Cette opération ne sera pas affectée dans les versions locales d’Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="1aa61-105">This operation won't be affected in on-premises versions of Exchange Server.</span></span> <span data-ttu-id="1aa61-106">Pour plus d’informations, reportez-vous à la section [retraite des outils eDiscovery hérités dans Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span><span class="sxs-lookup"><span data-stu-id="1aa61-106">For more information, see [Retirement of legacy eDiscovery tools in Exchange Online](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#getsearchablemailboxes-setholdonmailboxes-and-getholdonmailboxes-operations-in-the-ews-api).</span></span>

<span data-ttu-id="1aa61-107">Trouvez des informations sur l’opération EWS **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="1aa61-107">Find information about the **GetSearchableMailboxes** EWS operation.</span></span> 
  
<span data-ttu-id="1aa61-108">L’opération **GetSearchableMailboxes** obtient un ensemble d’étendues de boîtes aux lettres pouvant faire l’objet d’une recherche pour les recherches de découverte.</span><span class="sxs-lookup"><span data-stu-id="1aa61-108">The **GetSearchableMailboxes** operation gets a scoped set of searchable mailboxes for discovery searches.</span></span> <span data-ttu-id="1aa61-109">L’étendue des boîtes aux lettres pouvant faire l’objet d’une recherche renvoyée dans la réponse est déterminée par le filtre de recherche et par le fait que l’appartenance au groupe de distribution est développée ou non.</span><span class="sxs-lookup"><span data-stu-id="1aa61-109">The scope of searchable mailboxes returned in the response is determined by the search filter and whether distribution group membership is expanded.</span></span> 

> [!NOTE] 
> <span data-ttu-id="1aa61-110">Cette opération est destinée à être utilisée avec le filtre de recherche et pour récupérer uniquement les quelques premières milliers ; elle n’est pas destinée à une extraction exhaustive.</span><span class="sxs-lookup"><span data-stu-id="1aa61-110">This operation is intended to be used with the search filter and to retrieve only the first few thousands; it's not intended for exhaustive retrieval.</span></span>
  
<span data-ttu-id="1aa61-111">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1aa61-111">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getsearchablemailboxes-operation"></a><span data-ttu-id="1aa61-112">Utilisation de l’opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-112">Using the GetSearchableMailboxes operation</span></span>

<span data-ttu-id="1aa61-113">L’opération **GetSearchableMailboxes** obtient des informations sur les boîtes aux lettres pouvant faire l’objet d’une recherche.</span><span class="sxs-lookup"><span data-stu-id="1aa61-113">The **GetSearchableMailboxes** operation gets information about searchable mailboxes.</span></span> <span data-ttu-id="1aa61-114">Les arguments suivants peuvent être transmis dans la demande :</span><span class="sxs-lookup"><span data-stu-id="1aa61-114">The following arguments can be passed in the request:</span></span> 
  
- <span data-ttu-id="1aa61-115">[Unsearchfilter](searchfilter.md) -accepte un seul alias de courrier électronique en tant qu’argument.</span><span class="sxs-lookup"><span data-stu-id="1aa61-115">[SearchFilter](searchfilter.md) - Accepts a single email alias as an argument.</span></span> 
    
- <span data-ttu-id="1aa61-116">[ExpandGroupMembership](expandgroupmembership.md) -indique si l’appartenance au groupe de distribution est développée dans les résultats renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="1aa61-116">[ExpandGroupMembership](expandgroupmembership.md) - Indicates whether the distribution group membership is expanded in the results returned in the response.</span></span> 
    
<span data-ttu-id="1aa61-117">Si le jeu d’alias de messagerie du filtre de recherche est un groupe de distribution et que l’appartenance au groupe de distribution n’est pas développée, la réponse contiendra les informations de boîte aux lettres du groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="1aa61-117">If the email alias set in the search filter is a distribution group and the distribution group membership is not expanded, the response will contain the mailbox information for the distribution group.</span></span> <span data-ttu-id="1aa61-118">Si le jeu d’alias de messagerie du filtre de recherche est un groupe de distribution et que l’appartenance au groupe de distribution est étendue, la réponse contient les informations de boîte aux lettres de chaque boîte aux lettres membre du groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="1aa61-118">If the email alias set in the search filter is a distribution group and the distribution group membership is expanded, the response will contain the mailbox information for each mailbox that is a member of the distribution group.</span></span> <span data-ttu-id="1aa61-119">Si le filtre de recherche contient l’alias d’un seul utilisateur, la réponse contiendra les informations de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1aa61-119">If the search filter contains a single user's alias, the response will contain the mailbox information for the single user.</span></span> <span data-ttu-id="1aa61-120">La réponse contiendra toutes les boîtes aux lettres pouvant faire l’objet d’une recherche si l’élément [GetSearchableMailboxes](getsearchablemailboxes.md) est vide.</span><span class="sxs-lookup"><span data-stu-id="1aa61-120">The response will contain all searchable mailboxes if the [GetSearchableMailboxes](getsearchablemailboxes.md) element is empty.</span></span> <span data-ttu-id="1aa61-121">Cela revient à avoir un élément [unsearchfilter](searchfilter.md) vide et l’élément [ExpandGroupMembership](expandgroupmembership.md) définis sur **false**.</span><span class="sxs-lookup"><span data-stu-id="1aa61-121">This is the same as having an empty [SearchFilter](searchfilter.md) element and the [ExpandGroupMembership](expandgroupmembership.md) element set to **false**.</span></span>
  
### <a name="getsearchablemailboxes-operation-soap-headers"></a><span data-ttu-id="1aa61-122">En-têtes SOAP d’opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-122">GetSearchableMailboxes operation SOAP headers</span></span>

<span data-ttu-id="1aa61-123">L’opération **GetSearchableMailboxes** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="1aa61-123">The **GetSearchableMailboxes** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1aa61-124">Nom de l’en-tête</span><span class="sxs-lookup"><span data-stu-id="1aa61-124">Header name</span></span>|<span data-ttu-id="1aa61-125">Élément</span><span class="sxs-lookup"><span data-stu-id="1aa61-125">Element</span></span>|<span data-ttu-id="1aa61-126">Description</span><span class="sxs-lookup"><span data-stu-id="1aa61-126">Description</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1aa61-127">**ManagementRole**</span><span class="sxs-lookup"><span data-stu-id="1aa61-127">**ManagementRole**</span></span> <br/> |[<span data-ttu-id="1aa61-128">ManagementRole</span><span class="sxs-lookup"><span data-stu-id="1aa61-128">ManagementRole</span></span>](managementrole.md) <br/> |<span data-ttu-id="1aa61-129">Identifie les rôles serveur nécessaires pour que l’appelant effectue la demande.</span><span class="sxs-lookup"><span data-stu-id="1aa61-129">Identifies the server roles that are necessary in order for the caller to make the request.</span></span> <span data-ttu-id="1aa61-130">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="1aa61-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1aa61-131">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1aa61-131">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1aa61-132">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1aa61-132">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1aa61-133">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="1aa61-133">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1aa61-134">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="1aa61-134">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1aa61-135">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1aa61-135">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1aa61-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1aa61-136">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1aa61-137">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="1aa61-137">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1aa61-138">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="1aa61-138">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getsearchablemailboxes-operation-request-example-request-information-about-a-distribution-group"></a><span data-ttu-id="1aa61-139">Exemple de requête d’opération GetSearchableMailboxes : demander des informations sur un groupe de distribution</span><span class="sxs-lookup"><span data-stu-id="1aa61-139">GetSearchableMailboxes operation request example: Request information about a distribution group</span></span>

<span data-ttu-id="1aa61-140">L’exemple suivant de demande d’opération **GetSearchableMailboxes** indique comment obtenir les informations de boîte aux lettres pour le groupe de distribution lolgroup.</span><span class="sxs-lookup"><span data-stu-id="1aa61-140">The following example of a **GetSearchableMailboxes** operation request shows how to get the mailbox information for the lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="1aa61-141">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1aa61-141">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1aa61-142">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-142">GetSearchableMailboxes</span></span>](getsearchablemailboxes.md)   
- [<span data-ttu-id="1aa61-143">Unsearchfilter</span><span class="sxs-lookup"><span data-stu-id="1aa61-143">SearchFilter</span></span>](searchfilter.md)    
- [<span data-ttu-id="1aa61-144">ExpandGroupMembership</span><span class="sxs-lookup"><span data-stu-id="1aa61-144">ExpandGroupMembership</span></span>](expandgroupmembership.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-a-distribution-group"></a><span data-ttu-id="1aa61-145">Réponse de l’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution</span><span class="sxs-lookup"><span data-stu-id="1aa61-145">Successful GetSearchableMailboxes operation response: Get information about a distribution group</span></span>

<span data-ttu-id="1aa61-146">L’exemple suivant montre une réponse réussie à une demande d’opération **GetSearchableMailboxes** afin d’obtenir les informations de découverte pour le groupe de distribution lolgroup.</span><span class="sxs-lookup"><span data-stu-id="1aa61-146">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information for the lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="1aa61-147">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1aa61-147">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1aa61-148">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="1aa61-148">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)   
- [<span data-ttu-id="1aa61-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1aa61-149">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="1aa61-150">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-150">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="1aa61-151">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="1aa61-151">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="1aa61-152">Guid</span><span class="sxs-lookup"><span data-stu-id="1aa61-152">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="1aa61-153">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1aa61-153">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="1aa61-154">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="1aa61-154">IsExternalMailbox</span></span>](isexternalmailbox.md)   
- [<span data-ttu-id="1aa61-155">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1aa61-155">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="1aa61-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1aa61-156">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="1aa61-157">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="1aa61-157">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="1aa61-158">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="1aa61-158">ReferenceId</span></span>](referenceid.md)
    
## <a name="successful-getsearchablemailboxes-operation-response-get-information-about-an-expanded-distribution-group"></a><span data-ttu-id="1aa61-159">Réponse de l’opération GetSearchableMailboxes réussie : obtenir des informations sur un groupe de distribution étendu</span><span class="sxs-lookup"><span data-stu-id="1aa61-159">Successful GetSearchableMailboxes operation response: Get information about an expanded distribution group</span></span>

<span data-ttu-id="1aa61-160">L’exemple suivant montre une réponse réussie à une demande d’opération **GetSearchableMailboxes** pour obtenir les informations de découverte sur les membres du groupe de distribution lolgroup étendu.</span><span class="sxs-lookup"><span data-stu-id="1aa61-160">The following example shows a successful response to a **GetSearchableMailboxes** operation request to get the discovery information about members of the expanded lolgroup distribution group.</span></span> 
  
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

<span data-ttu-id="1aa61-161">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1aa61-161">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1aa61-162">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="1aa61-162">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)    
- [<span data-ttu-id="1aa61-163">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1aa61-163">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="1aa61-164">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-164">SearchableMailboxes</span></span>](searchablemailboxes.md)    
- [<span data-ttu-id="1aa61-165">SearchableMailbox</span><span class="sxs-lookup"><span data-stu-id="1aa61-165">SearchableMailbox</span></span>](searchablemailbox.md)    
- [<span data-ttu-id="1aa61-166">Guid</span><span class="sxs-lookup"><span data-stu-id="1aa61-166">Guid</span></span>](guid-ex15websvcsotherref.md)    
- [<span data-ttu-id="1aa61-167">PrimarySmtpAddress</span><span class="sxs-lookup"><span data-stu-id="1aa61-167">PrimarySmtpAddress</span></span>](primarysmtpaddress.md)    
- [<span data-ttu-id="1aa61-168">IsExternalMailbox</span><span class="sxs-lookup"><span data-stu-id="1aa61-168">IsExternalMailbox</span></span>](isexternalmailbox.md)    
- [<span data-ttu-id="1aa61-169">ExternalEmailAddress</span><span class="sxs-lookup"><span data-stu-id="1aa61-169">ExternalEmailAddress</span></span>](externalemailaddress.md)    
- [<span data-ttu-id="1aa61-170">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1aa61-170">DisplayName (string)</span></span>](displayname-string.md)    
- [<span data-ttu-id="1aa61-171">IsMembershipGroup</span><span class="sxs-lookup"><span data-stu-id="1aa61-171">IsMembershipGroup</span></span>](ismembershipgroup.md)    
- [<span data-ttu-id="1aa61-172">ReferenceId</span><span class="sxs-lookup"><span data-stu-id="1aa61-172">ReferenceId</span></span>](referenceid.md)
    
## <a name="getsearchablemailboxes-operation-error-response"></a><span data-ttu-id="1aa61-173">Réponse d’erreur d’opération GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-173">GetSearchableMailboxes operation error response</span></span>

<span data-ttu-id="1aa61-174">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetSearchableMailboxes** .</span><span class="sxs-lookup"><span data-stu-id="1aa61-174">The following example shows an error response to a **GetSearchableMailboxes** operation request.</span></span> <span data-ttu-id="1aa61-175">Réponse à une demande d’obtention de toutes les boîtes aux lettres pouvant faire l’objet d’une recherche lorsque l’argument **ExpandGroupMembership** est défini sur **true**.</span><span class="sxs-lookup"><span data-stu-id="1aa61-175">This is a response to a request to get all searchable mailboxes when the **ExpandGroupMembership** argument is set to **true**.</span></span> 
  
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

<span data-ttu-id="1aa61-176">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1aa61-176">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1aa61-177">GetSearchableMailboxesResponse</span><span class="sxs-lookup"><span data-stu-id="1aa61-177">GetSearchableMailboxesResponse</span></span>](getsearchablemailboxesresponse.md)  
- [<span data-ttu-id="1aa61-178">MessageText</span><span class="sxs-lookup"><span data-stu-id="1aa61-178">MessageText</span></span>](messagetext.md)   
- [<span data-ttu-id="1aa61-179">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1aa61-179">ResponseCode</span></span>](responsecode.md)   
- [<span data-ttu-id="1aa61-180">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1aa61-180">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) 
- [<span data-ttu-id="1aa61-181">SearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-181">SearchableMailboxes</span></span>](searchablemailboxes.md)
    
<span data-ttu-id="1aa61-182">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="1aa61-182">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1aa61-183">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1aa61-183">See also</span></span>

- [<span data-ttu-id="1aa61-184">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1aa61-184">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="1aa61-185">Opération SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-185">SetHoldOnMailboxes operation</span></span>](setholdonmailboxes-operation.md)   
- [<span data-ttu-id="1aa61-186">Opération SearchMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-186">SearchMailboxes operation</span></span>](searchmailboxes-operation.md)   
- [<span data-ttu-id="1aa61-187">Opération GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="1aa61-187">GetHoldOnMailboxes operation</span></span>](getholdonmailboxes-operation.md)    
- [<span data-ttu-id="1aa61-188">Opération GetDiscoverySearchConfiguration</span><span class="sxs-lookup"><span data-stu-id="1aa61-188">GetDiscoverySearchConfiguration operation</span></span>](getdiscoverysearchconfiguration-operation.md)   
- [<span data-ttu-id="1aa61-189">Opération GetNonIndexableItemDetails</span><span class="sxs-lookup"><span data-stu-id="1aa61-189">GetNonIndexableItemDetails operation</span></span>](getnonindexableitemdetails-operation.md)   
- [<span data-ttu-id="1aa61-190">Opération GetNonIndexableItemStatistics</span><span class="sxs-lookup"><span data-stu-id="1aa61-190">GetNonIndexableItemStatistics operation</span></span>](getnonindexableitemstatistics-operation.md)
    

