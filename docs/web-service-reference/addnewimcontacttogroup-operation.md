---
title: Opération AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Opération de recherche plus d’informations sur la AddNewImContactToGroup EWS.
ms.openlocfilehash: f75b89dbb6e948431d56acb9baa93fe4d4a1d939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755177"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="5d342-103">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="5d342-104">Trouvez des informations sur l’opération EWS **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="5d342-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="5d342-105">L’opération **AddNewImContactToGroup** ajoute un nouveau contact à un groupe (IM) de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5d342-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="5d342-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5d342-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="5d342-107">Utilisation de l’opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="5d342-108">L’opération **AddNewImContactToGroup** prend les trois arguments à ajouter un nouveau contact à un groupe de messagerie instantanée suivants :</span><span class="sxs-lookup"><span data-stu-id="5d342-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="5d342-109">**IMAddress,** propriété - identifie l’adresse de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5d342-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="5d342-110">Cette propriété est requise.</span><span class="sxs-lookup"><span data-stu-id="5d342-110">This property is required.</span></span> 
    
- <span data-ttu-id="5d342-111">Propriété **DisplayName** - identifie le nom du contact complet.</span><span class="sxs-lookup"><span data-stu-id="5d342-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="5d342-112">Propriété **GroupId** - identifie le groupe que le contact est ajouté à.</span><span class="sxs-lookup"><span data-stu-id="5d342-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="5d342-113">Cette opération retourne le personnage du contact qui a été ajouté au groupe.</span><span class="sxs-lookup"><span data-stu-id="5d342-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="5d342-114">En-têtes SOAP AddNewImContactToGroup opération</span><span class="sxs-lookup"><span data-stu-id="5d342-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="5d342-115">L’opération **AddNewImContactToGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5d342-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5d342-116">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="5d342-116">**Header name**</span></span>|<span data-ttu-id="5d342-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5d342-117">**Element**</span></span>|<span data-ttu-id="5d342-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="5d342-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5d342-119">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="5d342-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5d342-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5d342-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5d342-121">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="5d342-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5d342-122">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5d342-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5d342-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5d342-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5d342-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5d342-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5d342-125">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5d342-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5d342-126">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5d342-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5d342-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5d342-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5d342-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5d342-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5d342-129">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="5d342-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5d342-130">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5d342-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5d342-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5d342-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5d342-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5d342-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5d342-133">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="5d342-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5d342-134">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="5d342-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="5d342-135">Exemple de requête d’opération AddNewImContactToGroup : ajouter un nouveau contact de messagerie instantanée à un groupe</span><span class="sxs-lookup"><span data-stu-id="5d342-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="5d342-136">Une requête d’opération **AddNewImContactToGroup** l’exemple suivant montre comment ajouter un nouveau contact à un groupe existant de la messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5d342-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="5d342-137">La valeur de la propriété **GroupId** pour que cet exemple a été retournée à partir des résultats de l' [opération AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5d342-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="5d342-138">La propriété **ExchangeStoreId** contient la valeur de la propriété **GroupId** .</span><span class="sxs-lookup"><span data-stu-id="5d342-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="5d342-139">La valeur **GroupId** a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5d342-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="5d342-140">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5d342-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d342-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="5d342-142">ImAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="5d342-143">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5d342-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="5d342-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="5d342-145">Réponse d’opération AddNewImContactToGroup réussie</span><span class="sxs-lookup"><span data-stu-id="5d342-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="5d342-146">L’exemple suivant montre une réponse positive à une demande d’opération **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="5d342-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="5d342-147">La réponse contient le personnage du contact nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="5d342-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="5d342-148">Le contact est ajouté au dossier Contacts rapides dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d342-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5d342-149">Les identificateurs ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5d342-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
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
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="http://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="5d342-150">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5d342-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d342-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="5d342-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="5d342-152">Personnage</span><span class="sxs-lookup"><span data-stu-id="5d342-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="5d342-153">PersonaId</span><span class="sxs-lookup"><span data-stu-id="5d342-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="5d342-154">PersonaType</span><span class="sxs-lookup"><span data-stu-id="5d342-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="5d342-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="5d342-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="5d342-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5d342-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="5d342-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="5d342-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="5d342-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="5d342-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="5d342-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="5d342-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5d342-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="5d342-161">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5d342-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="5d342-162">Adresse (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="5d342-163">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5d342-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="5d342-164">ImAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="5d342-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="5d342-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="5d342-166">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="5d342-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="5d342-167">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="5d342-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="5d342-168">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5d342-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="5d342-169">ID source</span><span class="sxs-lookup"><span data-stu-id="5d342-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="5d342-170">IsWritable</span><span class="sxs-lookup"><span data-stu-id="5d342-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="5d342-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="5d342-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="5d342-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="5d342-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="5d342-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="5d342-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="5d342-174">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="5d342-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="5d342-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="5d342-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="5d342-176">Valeur (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="5d342-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="5d342-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="5d342-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="5d342-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="5d342-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="5d342-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="5d342-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="5d342-180">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="5d342-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="5d342-181">Réponse d’erreur d’opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="5d342-182">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="5d342-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="5d342-183">Il s’agit d’une réponse à une demande pour ajouter un contact à un groupe qui ne figure pas dans la boîte aux lettres du demandeur.</span><span class="sxs-lookup"><span data-stu-id="5d342-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5d342-184">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5d342-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5d342-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="5d342-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="5d342-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="5d342-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5d342-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5d342-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5d342-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5d342-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5d342-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5d342-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="5d342-190">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5d342-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5d342-191">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5d342-191">See also</span></span>



[<span data-ttu-id="5d342-192">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="5d342-193">Opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="5d342-194">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="5d342-195">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="5d342-196">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="5d342-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="5d342-197">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5d342-197">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

