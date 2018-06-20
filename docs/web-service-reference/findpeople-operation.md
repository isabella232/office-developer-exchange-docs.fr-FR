---
title: Opération FindPeople
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: Opération de recherche plus d’informations sur la FindPeople EWS.
ms.openlocfilehash: 97c34d7df590d20513e8f1ad476d62f16815a42b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756416"
---
# <a name="findpeople-operation"></a><span data-ttu-id="32cc8-103">Opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="32cc8-103">FindPeople operation</span></span>

<span data-ttu-id="32cc8-104">Trouvez des informations sur l’opération EWS **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="32cc8-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="32cc8-105">L’opération **FindPeople** renvoie tous les objets personnage d’un dossier de Contacts spécifié ou récupère les contacts qui correspondent à une chaîne de requête spécifiée.</span><span class="sxs-lookup"><span data-stu-id="32cc8-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="32cc8-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="32cc8-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="32cc8-107">Utilisation de l’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="32cc8-107">Using the FindPeople operation</span></span>

<span data-ttu-id="32cc8-108">L’opération **FindPeople** renvoie des informations de contact agrégées.</span><span class="sxs-lookup"><span data-stu-id="32cc8-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="32cc8-109">L’opération **FindPeople** s’appuie sur les fonctionnalités actuelles des [Restriction](restriction.md) et [BaseShape](baseshape.md) des types complexes en ajoutant une restriction de l’agrégation et la capacité à renvoyer des propriétés supplémentaires.</span><span class="sxs-lookup"><span data-stu-id="32cc8-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="32cc8-110">En utilisant une restriction, un client peut spécifier des filtres, tels que « uniquement retourner des résultats qui ont une adresse de messagerie instantanée ».</span><span class="sxs-lookup"><span data-stu-id="32cc8-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="32cc8-111">Le comportement de recherche par défaut cible de boîte aux lettres personnelle de l’utilisateur spécifié et de la liste d’adresses globale (LAG).</span><span class="sxs-lookup"><span data-stu-id="32cc8-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="32cc8-112">Lors de la recherche de la liste d’adresses globale en tant que le dossier de recherche principal, vous devez spécifier une chaîne de requête au lieu d’une restriction, car cette opération ne permet pas de navigation de la liste d’adresses globale.</span><span class="sxs-lookup"><span data-stu-id="32cc8-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="32cc8-113">En-têtes SOAP FindPeople opération</span><span class="sxs-lookup"><span data-stu-id="32cc8-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="32cc8-114">L’opération **FindPeople** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="32cc8-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="32cc8-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="32cc8-115">**Header name**</span></span>|<span data-ttu-id="32cc8-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="32cc8-116">**Element**</span></span>|<span data-ttu-id="32cc8-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="32cc8-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="32cc8-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="32cc8-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="32cc8-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="32cc8-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="32cc8-120">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="32cc8-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="32cc8-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="32cc8-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="32cc8-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="32cc8-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="32cc8-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="32cc8-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="32cc8-124">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="32cc8-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="32cc8-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="32cc8-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="32cc8-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="32cc8-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="32cc8-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="32cc8-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="32cc8-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="32cc8-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="32cc8-129">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="32cc8-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="32cc8-130">Exemple de requête d’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="32cc8-130">FindPeople operation request example</span></span>

<span data-ttu-id="32cc8-131">Une demande d’opération **FindPeople** l’exemple suivant montre comment renvoyer les 100 premières contacts du dossier Contacts.</span><span class="sxs-lookup"><span data-stu-id="32cc8-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="32cc8-132">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="32cc8-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="32cc8-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="32cc8-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="32cc8-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="32cc8-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="32cc8-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="32cc8-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="32cc8-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="32cc8-137">Une demande d’opération **FindPeople** l’exemple suivant montre comment renvoyer les 100 premières contacts à partir de la liste d’adresses globale à l’aide d’une chaîne de requête.</span><span class="sxs-lookup"><span data-stu-id="32cc8-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="32cc8-138">Définition de la **DistinguishedFolderId** « répertoire » recherche la liste d’adresses globale comme principale source de personnages.</span><span class="sxs-lookup"><span data-stu-id="32cc8-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="32cc8-139">Réponse d’opération FindPeople réussie</span><span class="sxs-lookup"><span data-stu-id="32cc8-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="32cc8-140">L’exemple suivant montre une réponse positive à une demande d’opération **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="32cc8-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
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
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="32cc8-141">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="32cc8-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="32cc8-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="32cc8-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="32cc8-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="32cc8-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="32cc8-144">Personnes</span><span class="sxs-lookup"><span data-stu-id="32cc8-144">People</span></span>](people.md)
    
- [<span data-ttu-id="32cc8-145">Personnage</span><span class="sxs-lookup"><span data-stu-id="32cc8-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="32cc8-146">PersonaId</span><span class="sxs-lookup"><span data-stu-id="32cc8-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="32cc8-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="32cc8-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="32cc8-148">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="32cc8-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="32cc8-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="32cc8-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="32cc8-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="32cc8-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="32cc8-151">Classer sous</span><span class="sxs-lookup"><span data-stu-id="32cc8-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="32cc8-152">Prénom</span><span class="sxs-lookup"><span data-stu-id="32cc8-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="32cc8-153">Surname</span><span class="sxs-lookup"><span data-stu-id="32cc8-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="32cc8-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="32cc8-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="32cc8-156">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="32cc8-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="32cc8-158">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="32cc8-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="32cc8-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="32cc8-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="32cc8-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="32cc8-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="32cc8-161">Réponse d’erreur d’opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="32cc8-161">FindPeople operation error response</span></span>

<span data-ttu-id="32cc8-162">Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="32cc8-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="32cc8-163">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="32cc8-163">See also</span></span>

- [<span data-ttu-id="32cc8-164">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="32cc8-164">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="32cc8-165">Opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="32cc8-165">GetPersona operation</span></span>](getpersona-operation.md)
    

