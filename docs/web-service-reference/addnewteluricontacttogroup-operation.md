---
title: Opération AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: Trouvez des informations sur l’utilisation de l’opération EWS AddNewTelUriContactToGroup.
ms.openlocfilehash: 34450171776b4215d9c0a39700a309e2e2d755dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755178"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="58a0c-103">Opération AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="58a0c-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="58a0c-104">Trouvez des informations sur l’utilisation de l’opération EWS **AddNewTelUriContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="58a0c-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="58a0c-105">L’opération **AddNewTelUriContactToGroup** ajoute un nouveau contact à un groupe basé sur le numéro de téléphone d’un contact.</span><span class="sxs-lookup"><span data-stu-id="58a0c-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="58a0c-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="58a0c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="58a0c-107">Utilisation de l’opération AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="58a0c-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="58a0c-108">Une requête d’opération **AddNewTelUriContactToGroup** envoie les URI de téléphone d’un contact, URI SIP, numéro de téléphone et le groupe pour ajouter le contact.</span><span class="sxs-lookup"><span data-stu-id="58a0c-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="58a0c-109">Une réponse d’opération **AddNewTelUriContactToGroup** crée un personnage pour le nouveau contact.</span><span class="sxs-lookup"><span data-stu-id="58a0c-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="58a0c-110">Cette opération permet aux clients d’ajouter un nouveau contact même si le contact n’a pas de nom.</span><span class="sxs-lookup"><span data-stu-id="58a0c-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="58a0c-111">En-têtes SOAP AddNewTelUriContactToGroup opération</span><span class="sxs-lookup"><span data-stu-id="58a0c-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="58a0c-112">L’opération **AddNewTelUriContactToGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="58a0c-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="58a0c-113">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="58a0c-113">**Header name**</span></span>|<span data-ttu-id="58a0c-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="58a0c-114">**Element**</span></span>|<span data-ttu-id="58a0c-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="58a0c-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="58a0c-116">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="58a0c-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="58a0c-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="58a0c-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="58a0c-118">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="58a0c-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="58a0c-119">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="58a0c-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58a0c-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="58a0c-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="58a0c-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="58a0c-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="58a0c-122">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="58a0c-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="58a0c-123">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="58a0c-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58a0c-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="58a0c-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="58a0c-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="58a0c-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="58a0c-126">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="58a0c-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="58a0c-127">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="58a0c-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="58a0c-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="58a0c-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="58a0c-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="58a0c-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="58a0c-130">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="58a0c-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="58a0c-131">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="58a0c-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="58a0c-132">Exemple de requête d’opération AddNewTelUriContactToGroup : ajouter un nouveau contact à un groupe</span><span class="sxs-lookup"><span data-stu-id="58a0c-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="58a0c-133">Une requête d’opération **AddNewTelUriContactToGroup** l’exemple suivant montre comment créer un nouveau contact et ajouter le nouveau contact à un groupe (IM) de messagerie instantané à l’aide du contact TEL et URI SIP.</span><span class="sxs-lookup"><span data-stu-id="58a0c-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="58a0c-134">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="58a0c-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="58a0c-135">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58a0c-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58a0c-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="58a0c-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="58a0c-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="58a0c-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="58a0c-138">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="58a0c-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="58a0c-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="58a0c-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="58a0c-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="58a0c-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="58a0c-141">Réponse d’opération AddNewTelUriContactToGroup réussie</span><span class="sxs-lookup"><span data-stu-id="58a0c-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="58a0c-142">L’exemple suivant montre une réponse positive à une demande d’opération **AddNewTelUriContactToGroup** pour créer un contact.</span><span class="sxs-lookup"><span data-stu-id="58a0c-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="58a0c-143">La réponse contient l’identificateur personnage associée pour le contact, le nom complet du personnage, dans ce cas basé sur le numéro de téléphone du contact, et l’identificateur d’élément du contact, qui s’affiche dans le cadre de l’attribution d’identificateur de source.</span><span class="sxs-lookup"><span data-stu-id="58a0c-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="58a0c-144">La réponse SOAP body contient la suite des éléments :</span><span class="sxs-lookup"><span data-stu-id="58a0c-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="58a0c-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="58a0c-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="58a0c-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58a0c-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58a0c-147">Personnage</span><span class="sxs-lookup"><span data-stu-id="58a0c-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="58a0c-148">PersonaId</span><span class="sxs-lookup"><span data-stu-id="58a0c-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="58a0c-149">PersonaType</span><span class="sxs-lookup"><span data-stu-id="58a0c-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="58a0c-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="58a0c-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="58a0c-151">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58a0c-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="58a0c-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="58a0c-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="58a0c-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="58a0c-154">Classer sous</span><span class="sxs-lookup"><span data-stu-id="58a0c-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="58a0c-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="58a0c-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="58a0c-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="58a0c-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="58a0c-157">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="58a0c-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="58a0c-158">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="58a0c-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="58a0c-159">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="58a0c-160">ID source</span><span class="sxs-lookup"><span data-stu-id="58a0c-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="58a0c-161">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="58a0c-162">IsWritable</span><span class="sxs-lookup"><span data-stu-id="58a0c-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="58a0c-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="58a0c-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="58a0c-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="58a0c-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="58a0c-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="58a0c-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="58a0c-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="58a0c-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="58a0c-167">Valeur</span><span class="sxs-lookup"><span data-stu-id="58a0c-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="58a0c-168">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="58a0c-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="58a0c-169">Attribution (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="58a0c-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="58a0c-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="58a0c-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="58a0c-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="58a0c-172">Valeur</span><span class="sxs-lookup"><span data-stu-id="58a0c-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="58a0c-173">Number</span><span class="sxs-lookup"><span data-stu-id="58a0c-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="58a0c-174">Type (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="58a0c-175">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="58a0c-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="58a0c-176">Attribution (chaîne)</span><span class="sxs-lookup"><span data-stu-id="58a0c-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="58a0c-177">Exemple de réponse d’erreur opération AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="58a0c-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="58a0c-178">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddNewTelUriContactToGroup** lorsque l’identificateur de groupe contient une valeur correcte qui n’identifie pas un groupe dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="58a0c-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="58a0c-179">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="58a0c-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="58a0c-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="58a0c-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="58a0c-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="58a0c-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="58a0c-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="58a0c-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="58a0c-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="58a0c-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="58a0c-184">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="58a0c-184">See also</span></span>

- [<span data-ttu-id="58a0c-185">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="58a0c-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="58a0c-186">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="58a0c-186">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

