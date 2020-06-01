---
title: Opération GetPersona
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: Trouvez des informations sur l’opération EWS GetPersona.
ms.openlocfilehash: 2b335c694a85f87c96432ea6d7c1c674613d2f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460945"
---
# <a name="getpersona-operation"></a><span data-ttu-id="d7d7d-103">Opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-103">GetPersona operation</span></span>

<span data-ttu-id="d7d7d-104">Trouvez des informations sur l’opération EWS **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d7d7d-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="d7d7d-105">L’opération **GetPersona** renvoie un jeu de propriétés qui sont associées à un personnage.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="d7d7d-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="d7d7d-107">Utilisation de l’opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-107">Using the GetPersona operation</span></span>

<span data-ttu-id="d7d7d-108">L’opération **GetPersona** fournit l’accès aux informations de contact agrégées sous la forme d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="d7d7d-109">L’élément [PersonaId](personaid.md) dans la demande identifie le personnage à renvoyer dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="d7d7d-110">La réponse peut contenir un ensemble par défaut de propriétés de personnages ou un jeu de propriétés personnalisées.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="d7d7d-111">Nous vous recommandons de spécifier un jeu de propriétés personnalisées afin que les propriétés inutilisées ne soient pas traitées et envoyées du serveur au client.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="d7d7d-112">En-têtes SOAP d’opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="d7d7d-113">L’opération **GetPersona** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d7d7d-114">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-114">**Header name**</span></span>|<span data-ttu-id="d7d7d-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-115">**Element**</span></span>|<span data-ttu-id="d7d7d-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d7d7d-117">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d7d7d-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d7d7d-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d7d7d-119">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d7d7d-120">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7d7d-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d7d7d-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d7d7d-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d7d7d-123">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d7d7d-124">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7d7d-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d7d7d-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d7d7d-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7d7d-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d7d7d-127">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d7d7d-128">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="d7d7d-129">Exemple de requête d’opération GetPersona : renvoyer un ensemble de propriétés par défaut pour un personnage</span><span class="sxs-lookup"><span data-stu-id="d7d7d-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="d7d7d-130">L’exemple suivant de demande d’opération **GetPersona** indique comment renvoyer un ensemble de propriétés par défaut associées à un personnage.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="d7d7d-131">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d7d7d-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d7d7d-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="d7d7d-133">PersonaId</span><span class="sxs-lookup"><span data-stu-id="d7d7d-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="d7d7d-134">Réponse de l’opération GetPersona réussie</span><span class="sxs-lookup"><span data-stu-id="d7d7d-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="d7d7d-135">L’exemple suivant montre une réponse réussie à une demande d’opération **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d7d7d-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d7d7d-136">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d7d7d-137">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d7d7d-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="d7d7d-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7d7d-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="d7d7d-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7d7d-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7d7d-140">Persona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="d7d7d-141">PersonaId</span><span class="sxs-lookup"><span data-stu-id="d7d7d-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="d7d7d-142">PersonaType</span><span class="sxs-lookup"><span data-stu-id="d7d7d-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="d7d7d-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="d7d7d-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="d7d7d-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="d7d7d-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="d7d7d-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="d7d7d-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="d7d7d-146">FileAs</span><span class="sxs-lookup"><span data-stu-id="d7d7d-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="d7d7d-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="d7d7d-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="d7d7d-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="d7d7d-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="d7d7d-149">Surname</span><span class="sxs-lookup"><span data-stu-id="d7d7d-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="d7d7d-150">CompanyName</span><span class="sxs-lookup"><span data-stu-id="d7d7d-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="d7d7d-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="d7d7d-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="d7d7d-152">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="d7d7d-153">Attribution (String)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="d7d7d-154">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="d7d7d-155">[SourceId](sourceid.md) ID</span><span class="sxs-lookup"><span data-stu-id="d7d7d-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="d7d7d-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="d7d7d-157">IsWritable</span><span class="sxs-lookup"><span data-stu-id="d7d7d-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="d7d7d-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="d7d7d-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="d7d7d-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="d7d7d-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="d7d7d-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="d7d7d-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="d7d7d-161">DisplayName</span><span class="sxs-lookup"><span data-stu-id="d7d7d-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="d7d7d-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d7d7d-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="d7d7d-163">Valeur (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="d7d7d-164">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="d7d7d-165">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="d7d7d-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="d7d7d-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="d7d7d-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="d7d7d-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="d7d7d-168">GivenNames</span><span class="sxs-lookup"><span data-stu-id="d7d7d-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="d7d7d-169">Nom</span><span class="sxs-lookup"><span data-stu-id="d7d7d-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="d7d7d-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="d7d7d-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="d7d7d-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="d7d7d-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="d7d7d-172">Valeur (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="d7d7d-173">Number</span><span class="sxs-lookup"><span data-stu-id="d7d7d-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="d7d7d-174">Type (chaîne)</span><span class="sxs-lookup"><span data-stu-id="d7d7d-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="d7d7d-175">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="d7d7d-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="d7d7d-176">Réponse d’erreur d’opération GetPersona</span><span class="sxs-lookup"><span data-stu-id="d7d7d-176">GetPersona operation error response</span></span>

<span data-ttu-id="d7d7d-177">L’exemple suivant montre une réponse d’erreur à une demande d’opération **GetPersona** .</span><span class="sxs-lookup"><span data-stu-id="d7d7d-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="d7d7d-178">Il s’agit d’une réponse à une demande contenant un identificateur de personnage incorrectement spécifié.</span><span class="sxs-lookup"><span data-stu-id="d7d7d-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
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
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d7d7d-179">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="d7d7d-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d7d7d-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d7d7d-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="d7d7d-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7d7d-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d7d7d-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7d7d-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7d7d-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7d7d-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="d7d7d-184">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d7d7d-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d7d7d-185">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d7d7d-185">See also</span></span>

- [<span data-ttu-id="d7d7d-186">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d7d7d-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d7d7d-187">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d7d7d-187">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="d7d7d-188">Opération FindPeople</span><span class="sxs-lookup"><span data-stu-id="d7d7d-188">FindPeople operation</span></span>](findpeople-operation.md)
    

