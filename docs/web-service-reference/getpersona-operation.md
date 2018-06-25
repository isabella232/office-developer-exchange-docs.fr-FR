---
title: Opération GetPersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Opération de recherche plus d’informations sur la GetPersona EWS.
ms.openlocfilehash: c6ac357eaa34e9bae2fe0a79a4a2d02449100e78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756712"
---
# <a name="getpersona-operation"></a><span data-ttu-id="65e6e-103">Opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="65e6e-103">GetPersona operation</span></span>

<span data-ttu-id="65e6e-104">Trouvez des informations sur l’opération EWS **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="65e6e-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="65e6e-105">L’opération **GetPersona** renvoie un ensemble de propriétés qui sont associés à un personnage.</span><span class="sxs-lookup"><span data-stu-id="65e6e-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="65e6e-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="65e6e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="65e6e-107">Utilisation de l’opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="65e6e-107">Using the GetPersona operation</span></span>

<span data-ttu-id="65e6e-108">L’opération **GetPersona** donne accès aux informations de contact agrégées sous la forme d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="65e6e-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="65e6e-109">L’élément [PersonaId](personaid.md) dans la demande identifie le personnage à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="65e6e-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="65e6e-110">La réponse peut contenir un jeu de propriétés personnage par défaut ou un jeu de propriétés personnalisées.</span><span class="sxs-lookup"><span data-stu-id="65e6e-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="65e6e-111">Nous vous recommandons de spécifier une propriété personnalisée définie de sorte que les propriétés inutiles ne sont pas traitées et envoyées à partir du serveur au client.</span><span class="sxs-lookup"><span data-stu-id="65e6e-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="65e6e-112">En-têtes SOAP GetPersona opération</span><span class="sxs-lookup"><span data-stu-id="65e6e-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="65e6e-113">L’opération **GetPersona** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="65e6e-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="65e6e-114">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="65e6e-114">**Header name**</span></span>|<span data-ttu-id="65e6e-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="65e6e-115">**Element**</span></span>|<span data-ttu-id="65e6e-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="65e6e-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="65e6e-117">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="65e6e-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="65e6e-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="65e6e-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="65e6e-119">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="65e6e-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="65e6e-120">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="65e6e-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="65e6e-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="65e6e-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="65e6e-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="65e6e-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="65e6e-123">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="65e6e-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="65e6e-124">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="65e6e-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="65e6e-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="65e6e-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="65e6e-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="65e6e-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="65e6e-127">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="65e6e-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="65e6e-128">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="65e6e-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="65e6e-129">Exemple de requête d’opération GetPersona : renvoyer un ensemble par défaut des propriétés d’un personnage</span><span class="sxs-lookup"><span data-stu-id="65e6e-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="65e6e-130">Une demande d’opération **GetPersona** l’exemple suivant montre comment renvoyer un ensemble par défaut des propriétés qui sont associés à un personnage.</span><span class="sxs-lookup"><span data-stu-id="65e6e-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="65e6e-131">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="65e6e-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="65e6e-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="65e6e-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="65e6e-133">PersonaId</span><span class="sxs-lookup"><span data-stu-id="65e6e-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="65e6e-134">Réponse d’opération GetPersona réussie</span><span class="sxs-lookup"><span data-stu-id="65e6e-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="65e6e-135">L’exemple suivant montre une réponse positive à une demande d’opération **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="65e6e-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="65e6e-136">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="65e6e-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="65e6e-137">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="65e6e-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="65e6e-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65e6e-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="65e6e-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="65e6e-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="65e6e-140">Personnage</span><span class="sxs-lookup"><span data-stu-id="65e6e-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="65e6e-141">PersonaId</span><span class="sxs-lookup"><span data-stu-id="65e6e-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="65e6e-142">PersonaType</span><span class="sxs-lookup"><span data-stu-id="65e6e-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="65e6e-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="65e6e-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="65e6e-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="65e6e-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="65e6e-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="65e6e-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="65e6e-146">Classer sous</span><span class="sxs-lookup"><span data-stu-id="65e6e-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="65e6e-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="65e6e-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="65e6e-148">Prénom</span><span class="sxs-lookup"><span data-stu-id="65e6e-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="65e6e-149">Surname</span><span class="sxs-lookup"><span data-stu-id="65e6e-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="65e6e-150">CompanyName</span><span class="sxs-lookup"><span data-stu-id="65e6e-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="65e6e-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="65e6e-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="65e6e-152">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="65e6e-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="65e6e-153">Attribution (chaîne)</span><span class="sxs-lookup"><span data-stu-id="65e6e-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="65e6e-154">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="65e6e-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="65e6e-155">[ID source](sourceid.md) ID source</span><span class="sxs-lookup"><span data-stu-id="65e6e-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="65e6e-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="65e6e-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="65e6e-157">IsWritable</span><span class="sxs-lookup"><span data-stu-id="65e6e-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="65e6e-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="65e6e-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="65e6e-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="65e6e-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="65e6e-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="65e6e-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="65e6e-161">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="65e6e-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="65e6e-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="65e6e-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="65e6e-163">Valeur (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="65e6e-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="65e6e-164">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="65e6e-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="65e6e-165">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="65e6e-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="65e6e-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="65e6e-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="65e6e-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="65e6e-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="65e6e-168">GivenNames</span><span class="sxs-lookup"><span data-stu-id="65e6e-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="65e6e-169">Prénoms</span><span class="sxs-lookup"><span data-stu-id="65e6e-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="65e6e-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="65e6e-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="65e6e-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="65e6e-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="65e6e-172">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="65e6e-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="65e6e-173">Number</span><span class="sxs-lookup"><span data-stu-id="65e6e-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="65e6e-174">Type (chaîne)</span><span class="sxs-lookup"><span data-stu-id="65e6e-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="65e6e-175">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="65e6e-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="65e6e-176">Réponse d’erreur d’opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="65e6e-176">GetPersona operation error response</span></span>

<span data-ttu-id="65e6e-177">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="65e6e-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="65e6e-178">Il s’agit d’une réponse à une demande qui contient un identificateur personnage incorrectement spécifié.</span><span class="sxs-lookup"><span data-stu-id="65e6e-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
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
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="65e6e-179">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="65e6e-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="65e6e-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="65e6e-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="65e6e-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="65e6e-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="65e6e-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="65e6e-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="65e6e-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="65e6e-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="65e6e-184">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="65e6e-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="65e6e-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65e6e-185">See also</span></span>

- [<span data-ttu-id="65e6e-186">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65e6e-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="65e6e-187">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65e6e-187">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="65e6e-188">Opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="65e6e-188">FindPeople operation</span></span>](findpeople-operation.md)
    

