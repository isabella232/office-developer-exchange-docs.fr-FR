---
title: Opération SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Opération de recherche plus d’informations sur la SetImGroup EWS.
ms.openlocfilehash: 80980c25888ab3fcae0a761e115c3ac3d578a013
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829421"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="650ca-103">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-103">SetImGroup operation</span></span>

<span data-ttu-id="650ca-104">Trouvez des informations sur l’opération EWS **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="650ca-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="650ca-105">L’opération **SetImGroup** modifie le nom complet d’un groupe (IM) de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="650ca-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="650ca-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="650ca-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="650ca-107">Utilisation de l’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="650ca-108">L’opération **SetImGroup** prend uniquement un argument de nom unique complet.</span><span class="sxs-lookup"><span data-stu-id="650ca-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="650ca-109">En-têtes SOAP SetImGroup opération</span><span class="sxs-lookup"><span data-stu-id="650ca-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="650ca-110">L’opération **SetImGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="650ca-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="650ca-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="650ca-111">**Header name**</span></span>|<span data-ttu-id="650ca-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="650ca-112">**Element**</span></span>|<span data-ttu-id="650ca-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="650ca-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="650ca-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="650ca-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="650ca-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="650ca-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="650ca-116">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="650ca-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="650ca-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="650ca-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="650ca-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="650ca-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="650ca-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="650ca-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="650ca-120">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="650ca-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="650ca-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="650ca-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="650ca-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="650ca-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="650ca-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="650ca-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="650ca-124">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="650ca-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="650ca-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="650ca-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="650ca-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="650ca-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="650ca-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="650ca-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="650ca-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="650ca-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="650ca-129">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="650ca-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="650ca-130">Exemple de requête d’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-130">SetImGroup operation request example</span></span>

<span data-ttu-id="650ca-131">Une demande d’opération **SetImGroup** l’exemple suivant montre comment modifier un nom complet du groupe messagerie instantanée à « MyNewGroupName ».</span><span class="sxs-lookup"><span data-stu-id="650ca-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="650ca-132">L’identificateur de la banque Exchange a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="650ca-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="650ca-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="650ca-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="650ca-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="650ca-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="650ca-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="650ca-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="650ca-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="650ca-137">Réponse d’opération SetImGroup réussie</span><span class="sxs-lookup"><span data-stu-id="650ca-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="650ca-138">L’exemple suivant montre une réponse positive à une demande d’opération **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="650ca-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="650ca-139">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="650ca-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="650ca-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="650ca-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="650ca-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="650ca-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="650ca-142">Réponse d’erreur d’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-142">SetImGroup operation error response</span></span>

<span data-ttu-id="650ca-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="650ca-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="650ca-144">La réponse d’erreur se produit lorsqu’une tentative est effectuée pour modifier le nom complet de groupe pour le nom complet du groupe.</span><span class="sxs-lookup"><span data-stu-id="650ca-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="650ca-145">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="650ca-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="650ca-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="650ca-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="650ca-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="650ca-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="650ca-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="650ca-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="650ca-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="650ca-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="650ca-150">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="650ca-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="650ca-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="650ca-151">See also</span></span>

- [<span data-ttu-id="650ca-152">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="650ca-152">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="650ca-153">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="650ca-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="650ca-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

