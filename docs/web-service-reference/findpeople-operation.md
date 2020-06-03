---
title: Opération FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Trouvez des informations sur l’opération EWS FindPeople.
ms.openlocfilehash: ab5edc3f140e34123ce1f009c401ddd61a0e2598
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462907"
---
# <a name="findpeople-operation"></a><span data-ttu-id="5022b-103">Opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-103">FindPeople operation</span></span>

<span data-ttu-id="5022b-104">Trouvez des informations sur l’opération EWS **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="5022b-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="5022b-105">L’opération **FindPeople** renvoie tous les objets Persona d’un dossier de contacts spécifié ou récupère les contacts qui correspondent à une chaîne de requête spécifiée.</span><span class="sxs-lookup"><span data-stu-id="5022b-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="5022b-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5022b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="5022b-107">Utilisation de l’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-107">Using the FindPeople operation</span></span>

<span data-ttu-id="5022b-108">L’opération **FindPeople** renvoie des informations de contact regroupées.</span><span class="sxs-lookup"><span data-stu-id="5022b-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="5022b-109">L’opération **FindPeople** s’appuie sur la fonctionnalité existante des types complexes de [restriction](restriction.md) et de [BaseShape](baseshape.md) en ajoutant une restriction d’agrégation et la possibilité de renvoyer des propriétés supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="5022b-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="5022b-110">À l’aide d’une restriction, un client peut spécifier des filtres, tels que « renvoyer uniquement les résultats ayant une adresse de messagerie instantanée ».</span><span class="sxs-lookup"><span data-stu-id="5022b-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="5022b-111">Le comportement de recherche par défaut cible à la fois la boîte aux lettres personnelle de l’utilisateur spécifié et la liste d’adresses globale (LAG).</span><span class="sxs-lookup"><span data-stu-id="5022b-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="5022b-112">Lors de la recherche dans la liste d’adresses globale en tant que dossier de recherche principal, vous devez spécifier une chaîne de requête au lieu d’une restriction, car cette opération ne permet pas de parcourir la liste d’adresses globale.</span><span class="sxs-lookup"><span data-stu-id="5022b-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="5022b-113">En-têtes SOAP d’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="5022b-114">L’opération **FindPeople** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5022b-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5022b-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="5022b-115">**Header name**</span></span>|<span data-ttu-id="5022b-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5022b-116">**Element**</span></span>|<span data-ttu-id="5022b-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="5022b-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5022b-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="5022b-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5022b-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5022b-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5022b-120">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="5022b-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5022b-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="5022b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5022b-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5022b-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5022b-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5022b-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5022b-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="5022b-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5022b-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="5022b-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5022b-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5022b-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5022b-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5022b-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5022b-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="5022b-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5022b-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="5022b-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="5022b-130">Exemple de requête d’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-130">FindPeople operation request example</span></span>

<span data-ttu-id="5022b-131">L’exemple suivant de demande d’opération **FindPeople** indique comment renvoyer les premiers contacts 100 à partir du dossier contacts.</span><span class="sxs-lookup"><span data-stu-id="5022b-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="5022b-132">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5022b-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5022b-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="5022b-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="5022b-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="5022b-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="5022b-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="5022b-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="5022b-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="5022b-137">L’exemple suivant de demande d’opération **FindPeople** indique comment renvoyer les premiers contacts 100 de la liste d’adresses globale à l’aide d’une chaîne de requête.</span><span class="sxs-lookup"><span data-stu-id="5022b-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="5022b-138">La définition de **DistinguishedFolderId** sur « Directory » effectuera une recherche dans la liste d’adresses globale comme source principale de personnages.</span><span class="sxs-lookup"><span data-stu-id="5022b-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="5022b-139">Réponse de l’opération FindPeople réussie</span><span class="sxs-lookup"><span data-stu-id="5022b-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="5022b-140">L’exemple suivant montre une réponse réussie à une demande d’opération **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="5022b-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
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
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="5022b-141">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5022b-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5022b-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="5022b-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="5022b-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5022b-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5022b-144">Contacts</span><span class="sxs-lookup"><span data-stu-id="5022b-144">People</span></span>](people.md)
    
- [<span data-ttu-id="5022b-145">Persona</span><span class="sxs-lookup"><span data-stu-id="5022b-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="5022b-146">PersonaId</span><span class="sxs-lookup"><span data-stu-id="5022b-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="5022b-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="5022b-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="5022b-148">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="5022b-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="5022b-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="5022b-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="5022b-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="5022b-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="5022b-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="5022b-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="5022b-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="5022b-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="5022b-153">Surname</span><span class="sxs-lookup"><span data-stu-id="5022b-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="5022b-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="5022b-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="5022b-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5022b-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="5022b-156">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5022b-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="5022b-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5022b-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="5022b-158">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5022b-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="5022b-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="5022b-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="5022b-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="5022b-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="5022b-161">Réponse d’erreur d’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="5022b-161">FindPeople operation error response</span></span>

<span data-ttu-id="5022b-162">Pour les codes d’erreur qui sont génériques à EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5022b-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5022b-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5022b-163">See also</span></span>

- [<span data-ttu-id="5022b-164">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5022b-164">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="5022b-165">Opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="5022b-165">GetPersona operation</span></span>](getpersona-operation.md)
    

