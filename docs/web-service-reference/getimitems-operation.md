---
title: Opération GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: Opération de recherche plus d’informations sur la GetImItems EWS.
ms.openlocfilehash: 4335cc22b22dc5f102f2221f7fdb22a506ba026f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756643"
---
# <a name="getimitems-operation"></a><span data-ttu-id="325e5-103">Opération GetImItems</span><span class="sxs-lookup"><span data-stu-id="325e5-103">GetImItems operation</span></span>

<span data-ttu-id="325e5-104">Trouvez des informations sur l’opération EWS **GetImItems** .</span><span class="sxs-lookup"><span data-stu-id="325e5-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="325e5-105">L’opération **GetImItems** récupère des informations sur les groupes de la messagerie instantanée et les personnages du contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="325e5-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="325e5-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="325e5-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="325e5-107">Utilisation de l’opération GetImItems</span><span class="sxs-lookup"><span data-stu-id="325e5-107">Using the GetImItems operation</span></span>

<span data-ttu-id="325e5-108">L’opération **GetImItems** accepte le groupe et contact identificateurs d’élément et renvoie un ensemble d’informations sur les groupes et les contacts.</span><span class="sxs-lookup"><span data-stu-id="325e5-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="325e5-109">Les jeux de propriétés retournés dans la réponse sont identifiées par les propriétés étendues, plusieurs identificateurs de contact, les identificateurs de groupe et étendues des définitions de propriétés en tant qu’arguments.</span><span class="sxs-lookup"><span data-stu-id="325e5-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="325e5-110">En-têtes SOAP GetImItems opération</span><span class="sxs-lookup"><span data-stu-id="325e5-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="325e5-111">L’opération **GetImItems** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="325e5-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="325e5-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="325e5-112">**Header name**</span></span>|<span data-ttu-id="325e5-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="325e5-113">**Element**</span></span>|<span data-ttu-id="325e5-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="325e5-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="325e5-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="325e5-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="325e5-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="325e5-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="325e5-117">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="325e5-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="325e5-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="325e5-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="325e5-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="325e5-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="325e5-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="325e5-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="325e5-121">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="325e5-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="325e5-122">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="325e5-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="325e5-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="325e5-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="325e5-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="325e5-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="325e5-125">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="325e5-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="325e5-126">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="325e5-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="325e5-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="325e5-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="325e5-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="325e5-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="325e5-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="325e5-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="325e5-130">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="325e5-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="325e5-131">Exemple de requête d’opération GetImItems : obtenir des informations détaillées sur les contacts de messagerie instantanée et les groupes</span><span class="sxs-lookup"><span data-stu-id="325e5-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="325e5-132">Une demande d’opération **GetImItems** l’exemple suivant montre comment demander des informations détaillées sur les contacts de messagerie instantanée et les groupes.</span><span class="sxs-lookup"><span data-stu-id="325e5-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="325e5-133">Une opération **GetImItems** peut demander un ou plusieurs contacts ou détails du groupe.</span><span class="sxs-lookup"><span data-stu-id="325e5-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="325e5-134">Vous pouvez également utiliser les propriétés étendues pour obtenir les propriétés personnalisées sur des groupes et des contacts.</span><span class="sxs-lookup"><span data-stu-id="325e5-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="325e5-135">Si une propriété étendue demandée n’existe pas sur un élément, la réponse ignore la propriété demandée et retourner la réponse pour le jeu de propriétés par défaut.</span><span class="sxs-lookup"><span data-stu-id="325e5-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="325e5-136">Cet exemple montre comment obtenir le nom complet à l’aide des propriétés étendues.</span><span class="sxs-lookup"><span data-stu-id="325e5-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="325e5-137">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="325e5-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="325e5-138">Notez que modifier les clés sont ignorées par le service pour cette opération.</span><span class="sxs-lookup"><span data-stu-id="325e5-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="325e5-139">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="325e5-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="325e5-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="325e5-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="325e5-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="325e5-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="325e5-142">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="325e5-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="325e5-143">GroupID</span><span class="sxs-lookup"><span data-stu-id="325e5-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="325e5-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="325e5-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="325e5-145">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="325e5-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="325e5-146">Réponse d’opération GetImItems réussie</span><span class="sxs-lookup"><span data-stu-id="325e5-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="325e5-147">L’exemple suivant montre une réponse positive à une demande de **GetImItems** pour obtenir un contact de messagerie instantanée et de groupe.</span><span class="sxs-lookup"><span data-stu-id="325e5-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="325e5-148">Le nom complet est demandé dans une propriété étendue.</span><span class="sxs-lookup"><span data-stu-id="325e5-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="325e5-149">Contacts de messagerie instantanée sont renvoyées sous la forme d’un personnage.</span><span class="sxs-lookup"><span data-stu-id="325e5-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="325e5-150">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="325e5-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="325e5-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="325e5-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="325e5-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="325e5-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="325e5-153">ImItemList</span><span class="sxs-lookup"><span data-stu-id="325e5-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="325e5-154">Groupes (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="325e5-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="325e5-155">ImGroup</span><span class="sxs-lookup"><span data-stu-id="325e5-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="325e5-156">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="325e5-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="325e5-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="325e5-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="325e5-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="325e5-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="325e5-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="325e5-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="325e5-160">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="325e5-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="325e5-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="325e5-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="325e5-162">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="325e5-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="325e5-163">Personnages</span><span class="sxs-lookup"><span data-stu-id="325e5-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="325e5-164">PersonaId</span><span class="sxs-lookup"><span data-stu-id="325e5-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="325e5-165">PersonaType</span><span class="sxs-lookup"><span data-stu-id="325e5-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="325e5-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="325e5-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="325e5-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="325e5-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="325e5-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="325e5-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="325e5-169">Classer sous</span><span class="sxs-lookup"><span data-stu-id="325e5-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="325e5-170">[FileAsId](fileasid.md) FileAsId</span><span class="sxs-lookup"><span data-stu-id="325e5-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="325e5-171">ImAddress (chaîne)</span><span class="sxs-lookup"><span data-stu-id="325e5-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="325e5-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="325e5-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="325e5-173">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="325e5-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="325e5-174">Attribution (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="325e5-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="325e5-175">ID (chaîne)</span><span class="sxs-lookup"><span data-stu-id="325e5-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="325e5-176">ID source</span><span class="sxs-lookup"><span data-stu-id="325e5-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="325e5-177">IsWritable</span><span class="sxs-lookup"><span data-stu-id="325e5-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="325e5-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="325e5-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="325e5-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="325e5-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="325e5-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="325e5-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="325e5-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="325e5-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="325e5-182">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="325e5-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="325e5-183">Valeur (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="325e5-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="325e5-184">Réponse d’erreur d’opération GetImItems</span><span class="sxs-lookup"><span data-stu-id="325e5-184">GetImItems operation error response</span></span>

<span data-ttu-id="325e5-185">L’opération **GetImItems** ne valide pas les identificateurs et ne retourne pas la réponse attendue d’erreur **ErrorInvalidImContactId** ou **ErrorInvalidImGroupId** si un contact non valide ou un identificateur de groupe est fourni pour le service.</span><span class="sxs-lookup"><span data-stu-id="325e5-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="325e5-186">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="325e5-186">See also</span></span>

- [<span data-ttu-id="325e5-187">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="325e5-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="325e5-188">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="325e5-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

