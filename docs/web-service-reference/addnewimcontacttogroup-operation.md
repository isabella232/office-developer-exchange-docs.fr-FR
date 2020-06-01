---
title: Opération AddNewImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: Trouvez des informations sur l’opération EWS AddNewImContactToGroup.
ms.openlocfilehash: e91cc067b4161b366e6713a9adc16873e63b1562
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465028"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="1880b-103">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="1880b-104">Trouvez des informations sur l’opération EWS **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="1880b-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="1880b-105">L’opération **AddNewImContactToGroup** ajoute un nouveau contact à un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="1880b-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="1880b-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1880b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="1880b-107">Utilisation de l’opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="1880b-108">L’opération **AddNewImContactToGroup** prend les trois arguments suivants pour ajouter un nouveau contact à un groupe de messagerie instantanée :</span><span class="sxs-lookup"><span data-stu-id="1880b-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="1880b-109">**IMAddress** , propriété : identifie l’adresse de messagerie instantanée du contact.</span><span class="sxs-lookup"><span data-stu-id="1880b-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="1880b-110">Cette propriété est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="1880b-110">This property is required.</span></span> 
    
- <span data-ttu-id="1880b-111">**DisplayName** , propriété-identifie le nom d’affichage du contact.</span><span class="sxs-lookup"><span data-stu-id="1880b-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="1880b-112">**GroupID** , propriété : identifie le groupe auquel le contact est ajouté.</span><span class="sxs-lookup"><span data-stu-id="1880b-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="1880b-113">Cette opération renvoie le personnage du contact qui a été ajouté au groupe.</span><span class="sxs-lookup"><span data-stu-id="1880b-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="1880b-114">En-têtes SOAP d’opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="1880b-115">L’opération **AddNewImContactToGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="1880b-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1880b-116">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="1880b-116">**Header name**</span></span>|<span data-ttu-id="1880b-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1880b-117">**Element**</span></span>|<span data-ttu-id="1880b-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="1880b-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1880b-119">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="1880b-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1880b-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1880b-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1880b-121">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="1880b-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1880b-122">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="1880b-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1880b-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1880b-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1880b-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1880b-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1880b-125">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="1880b-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1880b-126">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="1880b-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1880b-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1880b-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1880b-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1880b-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1880b-129">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="1880b-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1880b-130">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="1880b-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1880b-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1880b-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1880b-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1880b-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1880b-133">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="1880b-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1880b-134">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="1880b-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="1880b-135">Exemple de requête d’opération AddNewImContactToGroup : ajouter un nouveau contact de messagerie instantanée à un groupe</span><span class="sxs-lookup"><span data-stu-id="1880b-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="1880b-136">L’exemple suivant de demande d’opération **AddNewImContactToGroup** indique comment ajouter un nouveau contact à un groupe de messagerie instantanée existant.</span><span class="sxs-lookup"><span data-stu-id="1880b-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="1880b-137">La valeur de la propriété **GroupID** de cet exemple a été renvoyée à partir des résultats de l' [opération AddImGroup](addimgroup-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1880b-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="1880b-138">La propriété **ExchangeStoreId** contient la valeur de la propriété **GroupID** .</span><span class="sxs-lookup"><span data-stu-id="1880b-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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
> <span data-ttu-id="1880b-139">La valeur **GroupID** a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1880b-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="1880b-140">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1880b-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1880b-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="1880b-142">IMAddress (String)</span><span class="sxs-lookup"><span data-stu-id="1880b-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="1880b-143">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1880b-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1880b-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="1880b-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="1880b-145">Réponse de l’opération AddNewImContactToGroup réussie</span><span class="sxs-lookup"><span data-stu-id="1880b-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="1880b-146">L’exemple suivant montre une réponse réussie à une demande d’opération **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="1880b-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="1880b-147">La réponse contient le personnage du contact nouvellement créé.</span><span class="sxs-lookup"><span data-stu-id="1880b-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="1880b-148">Le contact est ajouté au dossier contacts rapides dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="1880b-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1880b-149">Les identificateurs ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="1880b-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
        <ImAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="1880b-150">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1880b-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1880b-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1880b-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="1880b-152">Persona</span><span class="sxs-lookup"><span data-stu-id="1880b-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="1880b-153">PersonaId</span><span class="sxs-lookup"><span data-stu-id="1880b-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="1880b-154">PersonaType</span><span class="sxs-lookup"><span data-stu-id="1880b-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="1880b-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="1880b-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="1880b-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1880b-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1880b-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="1880b-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="1880b-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="1880b-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="1880b-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="1880b-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="1880b-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1880b-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="1880b-161">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1880b-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="1880b-162">Address (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1880b-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="1880b-163">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="1880b-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="1880b-164">IMAddress (String)</span><span class="sxs-lookup"><span data-stu-id="1880b-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="1880b-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="1880b-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="1880b-166">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="1880b-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="1880b-167">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="1880b-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="1880b-168">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="1880b-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="1880b-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="1880b-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="1880b-170">IsWritable</span><span class="sxs-lookup"><span data-stu-id="1880b-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="1880b-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="1880b-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="1880b-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="1880b-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="1880b-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="1880b-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="1880b-174">DisplayName</span><span class="sxs-lookup"><span data-stu-id="1880b-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="1880b-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1880b-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="1880b-176">Valeur (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="1880b-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="1880b-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="1880b-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="1880b-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="1880b-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="1880b-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="1880b-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="1880b-180">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="1880b-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="1880b-181">Réponse d’erreur d’opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="1880b-182">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddNewImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="1880b-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="1880b-183">Il s’agit d’une réponse à une demande d’ajout d’un contact à un groupe qui ne se trouve pas dans la boîte aux lettres du demandeur.</span><span class="sxs-lookup"><span data-stu-id="1880b-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1880b-184">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="1880b-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1880b-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1880b-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="1880b-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="1880b-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1880b-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1880b-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1880b-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1880b-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="1880b-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1880b-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="1880b-190">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="1880b-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1880b-191">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1880b-191">See also</span></span>



[<span data-ttu-id="1880b-192">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="1880b-193">Opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="1880b-194">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="1880b-195">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="1880b-196">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="1880b-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="1880b-197">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1880b-197">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

