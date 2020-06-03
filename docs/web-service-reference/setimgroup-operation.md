---
title: Opération SetImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: Trouvez des informations sur l’opération EWS SetImGroup.
ms.openlocfilehash: 37b290559fff0b2de57669741547ba4b1b56c28c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44438074"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="6422b-103">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-103">SetImGroup operation</span></span>

<span data-ttu-id="6422b-104">Trouvez des informations sur l’opération EWS **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="6422b-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="6422b-105">L’opération **SetImGroup** modifie le nom d’affichage d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="6422b-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="6422b-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6422b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="6422b-107">Utilisation de l’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="6422b-108">L’opération **SetImGroup** ne prend qu’un seul argument Nom complet.</span><span class="sxs-lookup"><span data-stu-id="6422b-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="6422b-109">En-têtes SOAP d’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="6422b-110">L’opération **SetImGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="6422b-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="6422b-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="6422b-111">**Header name**</span></span>|<span data-ttu-id="6422b-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6422b-112">**Element**</span></span>|<span data-ttu-id="6422b-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="6422b-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6422b-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="6422b-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="6422b-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="6422b-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6422b-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="6422b-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="6422b-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="6422b-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6422b-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="6422b-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="6422b-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="6422b-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="6422b-120">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="6422b-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="6422b-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="6422b-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6422b-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="6422b-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="6422b-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6422b-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6422b-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="6422b-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="6422b-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="6422b-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6422b-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="6422b-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="6422b-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6422b-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6422b-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="6422b-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6422b-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="6422b-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="6422b-130">Exemple de requête d’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-130">SetImGroup operation request example</span></span>

<span data-ttu-id="6422b-131">L’exemple suivant de demande d’opération **SetImGroup** indique comment modifier un nom complet de groupe de messagerie instantanée en « MyNewGroupName ».</span><span class="sxs-lookup"><span data-stu-id="6422b-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6422b-132">L’identificateur de la banque Exchange a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6422b-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6422b-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6422b-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6422b-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="6422b-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="6422b-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="6422b-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="6422b-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="6422b-137">Réponse de l’opération SetImGroup réussie</span><span class="sxs-lookup"><span data-stu-id="6422b-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="6422b-138">L’exemple suivant montre une réponse réussie à une demande d’opération **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="6422b-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="6422b-139">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6422b-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6422b-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="6422b-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="6422b-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6422b-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="6422b-142">Réponse d’erreur d’opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-142">SetImGroup operation error response</span></span>

<span data-ttu-id="6422b-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **SetImGroup** .</span><span class="sxs-lookup"><span data-stu-id="6422b-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="6422b-144">La réponse d’erreur suivante se produit lors d’une tentative de modification du nom d’affichage du groupe en nom complet du groupe existant.</span><span class="sxs-lookup"><span data-stu-id="6422b-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6422b-145">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="6422b-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6422b-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="6422b-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="6422b-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="6422b-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6422b-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6422b-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6422b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6422b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="6422b-150">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="6422b-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6422b-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6422b-151">See also</span></span>

- [<span data-ttu-id="6422b-152">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6422b-152">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="6422b-153">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="6422b-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="6422b-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

