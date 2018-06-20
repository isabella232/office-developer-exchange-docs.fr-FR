---
title: Opération AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Opération de recherche plus d’informations sur la AddImGroup EWS.
ms.openlocfilehash: 91236f9ad2236b3f6bee600b9d57bcf736090ed7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755167"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="41b53-103">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-103">AddImGroup operation</span></span>

<span data-ttu-id="41b53-104">Trouvez des informations sur l’opération EWS **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="41b53-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="41b53-105">L’opération d’Exchange Web Services (EWS) **AddImGroup** ajoute un nouveau groupe de messagerie instantanée à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="41b53-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="41b53-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="41b53-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="41b53-107">Utilisation de l’opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="41b53-108">L’opération **AddImGroup** prend uniquement un argument de nom unique complet.</span><span class="sxs-lookup"><span data-stu-id="41b53-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="41b53-109">Cette opération retourne le nom complet, le type de groupe et l’identificateur de banque Exchange du nouveau groupe.</span><span class="sxs-lookup"><span data-stu-id="41b53-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="41b53-110">L’opération **AddImGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="41b53-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="41b53-111">**Le tableau 1. En-têtes SOAP AddImGroup opération**</span><span class="sxs-lookup"><span data-stu-id="41b53-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="41b53-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="41b53-112">**Header name**</span></span>|<span data-ttu-id="41b53-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="41b53-113">**Element**</span></span>|<span data-ttu-id="41b53-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="41b53-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="41b53-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="41b53-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="41b53-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="41b53-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="41b53-117">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="41b53-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="41b53-118">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="41b53-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="41b53-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="41b53-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="41b53-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="41b53-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="41b53-121">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="41b53-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="41b53-122">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="41b53-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="41b53-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="41b53-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="41b53-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="41b53-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="41b53-125">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="41b53-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="41b53-126">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="41b53-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="41b53-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="41b53-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="41b53-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="41b53-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="41b53-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="41b53-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="41b53-130">Cela s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="41b53-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="41b53-131">Exemple de requête d’opération AddImGroup : créer un nouveau groupe de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="41b53-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="41b53-132">Une requête d’opération **AddImGroup** l’exemple suivant montre comment créer un groupe de messagerie instantanée nommé MyCustomerGroup.</span><span class="sxs-lookup"><span data-stu-id="41b53-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="41b53-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="41b53-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="41b53-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="41b53-135">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="41b53-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="41b53-136">Réponse d’opération AddImGroup réussie</span><span class="sxs-lookup"><span data-stu-id="41b53-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="41b53-137">L’exemple suivant montre une réponse positive à une demande d’opération **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="41b53-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="41b53-138">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="41b53-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="41b53-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="41b53-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="41b53-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="41b53-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="41b53-141">ImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="41b53-142">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="41b53-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="41b53-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="41b53-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="41b53-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="41b53-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="41b53-145">Réponse d’erreur d’opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-145">AddImGroup operation error response</span></span>

<span data-ttu-id="41b53-146">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddImGroup** .</span><span class="sxs-lookup"><span data-stu-id="41b53-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="41b53-147">Il s’agit d’une réponse à une demande qui contient un caractère qui ne peut pas être utilisé dans un nom d’affichage.</span><span class="sxs-lookup"><span data-stu-id="41b53-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="41b53-148">Notez qu’il s’agit d’une erreur SOAP et non un message d’erreur basée sur un schéma.</span><span class="sxs-lookup"><span data-stu-id="41b53-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="41b53-149">Est le nom d’affichage présenté dans la demande ~ ! @# $% ^&amp;, l’erreur se produit sur le &amp; caractère.</span><span class="sxs-lookup"><span data-stu-id="41b53-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="41b53-150">Le &amp; caractères s’est produite sur le caractère de trait et 33rd 11 de la charge utile de demande.</span><span class="sxs-lookup"><span data-stu-id="41b53-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="41b53-151">La réponse a été renvoyée avec un code HTTP 500.</span><span class="sxs-lookup"><span data-stu-id="41b53-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="41b53-152">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="41b53-152">See also</span></span>

- [<span data-ttu-id="41b53-153">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="41b53-153">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="41b53-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="41b53-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="41b53-155">SetImGroup</span></span>](setimgroup.md)
    

