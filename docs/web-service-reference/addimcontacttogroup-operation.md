---
title: Opération AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Trouvez des informations sur l’opération EWS AddImContactToGroup.
ms.openlocfilehash: a69ee0b355e78e1249383cab612a75bcda8d9e8a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458410"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="cfae2-103">Opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="cfae2-104">Trouvez des informations sur l’opération EWS **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="cfae2-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="cfae2-105">L’opération **AddImContactToGroup** les services Web Exchange (EWS) ajoute un contact de messagerie instantanée à un groupe.</span><span class="sxs-lookup"><span data-stu-id="cfae2-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="cfae2-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="cfae2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="cfae2-107">Utilisation de l’opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="cfae2-108">L’opération **AddImContactToGroup** peut accepter uniquement les contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="cfae2-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="cfae2-109">Si vous souhaitez ajouter un nouveau contact de messagerie instantanée au magasin de contacts unifié, utilisez l’opération [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="cfae2-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="cfae2-110">L’opération **AddImContactToGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="cfae2-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="cfae2-111">**Tableau 1. En-têtes SOAP d’opération AddImContactToGroup**</span><span class="sxs-lookup"><span data-stu-id="cfae2-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="cfae2-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="cfae2-112">**Header name**</span></span>|<span data-ttu-id="cfae2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cfae2-113">**Element**</span></span>|<span data-ttu-id="cfae2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="cfae2-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cfae2-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="cfae2-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cfae2-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cfae2-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cfae2-117">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="cfae2-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cfae2-118">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cfae2-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cfae2-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="cfae2-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cfae2-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="cfae2-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cfae2-121">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="cfae2-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cfae2-122">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cfae2-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cfae2-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cfae2-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cfae2-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cfae2-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cfae2-125">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="cfae2-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cfae2-126">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="cfae2-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cfae2-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cfae2-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cfae2-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cfae2-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cfae2-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="cfae2-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cfae2-130">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="cfae2-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="cfae2-131">Exemple de requête d’opération AddImContactToGroup : ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="cfae2-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="cfae2-132">L’exemple suivant de demande d’opération **AddImContactToGroup** indique comment ajouter un contact de messagerie instantanée existant à un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="cfae2-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cfae2-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cfae2-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cfae2-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="cfae2-135">Mettez</span><span class="sxs-lookup"><span data-stu-id="cfae2-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="cfae2-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="cfae2-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="cfae2-137">Réponse de l’opération AddImContactToGroup réussie</span><span class="sxs-lookup"><span data-stu-id="cfae2-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="cfae2-138">L’exemple suivant montre une réponse réussie à une demande d’opération **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="cfae2-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cfae2-139">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cfae2-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cfae2-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="cfae2-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="cfae2-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cfae2-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="cfae2-142">AddImContactToGroup Operation ErrorInvalidImContactId Error Response</span><span class="sxs-lookup"><span data-stu-id="cfae2-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="cfae2-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="cfae2-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="cfae2-144">La réponse d’erreur suivante se produit lors d’une tentative d’ajout d’un contact qui n’est pas un contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="cfae2-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="cfae2-145">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="cfae2-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cfae2-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="cfae2-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="cfae2-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="cfae2-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cfae2-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cfae2-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cfae2-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cfae2-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="cfae2-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cfae2-150">See also</span></span>

- [<span data-ttu-id="cfae2-151">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="cfae2-152">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="cfae2-153">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="cfae2-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="cfae2-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="cfae2-155">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="cfae2-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="cfae2-156">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="cfae2-156">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

