---
title: Opération RemoveImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: Trouvez des informations sur l’opération EWS RemoveImGroup.
ms.openlocfilehash: b5e38404cbb1907a1118ab3ae8e56abb5a8d5e41
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456740"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="7e6d0-103">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-103">RemoveImGroup operation</span></span>

<span data-ttu-id="7e6d0-104">Trouvez des informations sur l’opération EWS **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7e6d0-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="7e6d0-105">L’opération **RemoveImGroup** supprime un seul groupe de messagerie instantanée d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="7e6d0-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="7e6d0-107">Utilisation de l’opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="7e6d0-108">L’opération **RemoveImGroup** ne prend qu’un seul argument d’identificateur de groupe.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="7e6d0-109">En-têtes SOAP d’opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="7e6d0-110">L’opération **RemoveImGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7e6d0-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-111">**Header name**</span></span>|<span data-ttu-id="7e6d0-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-112">**Element**</span></span>|<span data-ttu-id="7e6d0-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7e6d0-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="7e6d0-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7e6d0-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7e6d0-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7e6d0-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7e6d0-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="7e6d0-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7e6d0-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="7e6d0-120">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="7e6d0-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7e6d0-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7e6d0-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7e6d0-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7e6d0-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7e6d0-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7e6d0-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7e6d0-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7e6d0-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7e6d0-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7e6d0-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7e6d0-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="7e6d0-130">Exemple de requête d’opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="7e6d0-131">L’exemple suivant de demande d’opération **RemoveImGroup** montre comment supprimer un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7e6d0-132">L’ID de groupe a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-132">The group ID has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7e6d0-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="7e6d0-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7e6d0-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="7e6d0-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="7e6d0-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="7e6d0-136">Réponse de l’opération RemoveImGroup réussie</span><span class="sxs-lookup"><span data-stu-id="7e6d0-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="7e6d0-137">L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7e6d0-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7e6d0-138">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="7e6d0-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7e6d0-139">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="7e6d0-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="7e6d0-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e6d0-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="7e6d0-141">RemoveImGroup Operation ErrorInvalidImGroupId Error Response</span><span class="sxs-lookup"><span data-stu-id="7e6d0-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="7e6d0-142">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7e6d0-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="7e6d0-143">La réponse d’erreur suivante se produit lors d’une tentative de suppression d’un groupe qui n’existe pas dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7e6d0-144">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="7e6d0-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7e6d0-145">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="7e6d0-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="7e6d0-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e6d0-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7e6d0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e6d0-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7e6d0-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e6d0-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7e6d0-149">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="7e6d0-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="7e6d0-150">RemoveImGroup Operation ErrorInvalidIdMalformed Error Response</span><span class="sxs-lookup"><span data-stu-id="7e6d0-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="7e6d0-151">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImGroup** .</span><span class="sxs-lookup"><span data-stu-id="7e6d0-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="7e6d0-152">La réponse d’erreur suivante se produit lors d’une tentative de suppression d’un groupe avec un identificateur de groupe avec un format incorrect.</span><span class="sxs-lookup"><span data-stu-id="7e6d0-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7e6d0-153">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="7e6d0-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7e6d0-154">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="7e6d0-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="7e6d0-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e6d0-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7e6d0-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e6d0-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7e6d0-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e6d0-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7e6d0-158">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e6d0-158">See also</span></span>

- [<span data-ttu-id="7e6d0-159">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7e6d0-159">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="7e6d0-160">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="7e6d0-161">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="7e6d0-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

