---
title: Opération AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Opération de recherche plus d’informations sur la AddImContactToGroup EWS.
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755162"
---
# <a name="addimcontacttogroup-operation"></a><span data-ttu-id="a6fe2-103">Opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-103">AddImContactToGroup operation</span></span>

<span data-ttu-id="a6fe2-104">Trouvez des informations sur l’opération EWS **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="a6fe2-104">Find information about the **AddImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="a6fe2-105">L’opération d’Exchange Web Services (EWS) **AddImContactToGroup** ajoute un contact de messagerie instantanée (MI) existant à un groupe.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-105">The **AddImContactToGroup** Exchange Web Services (EWS) operation adds an existing instant messaging (IM) contact to a group.</span></span> 
  
<span data-ttu-id="a6fe2-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimcontacttogroup-operation"></a><span data-ttu-id="a6fe2-107">Utilisation de l’opération AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-107">Using the AddImContactToGroup operation</span></span>

<span data-ttu-id="a6fe2-108">L’opération **AddImContactToGroup** peut accepter uniquement les contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-108">The **AddImContactToGroup** operation can only accept IM contacts.</span></span> <span data-ttu-id="a6fe2-109">Si vous souhaitez ajouter un nouveau contact de messagerie instantanée pour le magasin de contacts unifié, utilisez l’opération [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="a6fe2-109">If you want to add a new IM contact to the Unified Contact Store, use the [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) operation.</span></span> 
  
<span data-ttu-id="a6fe2-110">L’opération **AddImContactToGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-110">The **AddImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="a6fe2-111">**Le tableau 1. En-têtes SOAP AddImContactToGroup opération**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-111">**Table 1. AddImContactToGroup operation SOAP headers**</span></span>

|<span data-ttu-id="a6fe2-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-112">**Header name**</span></span>|<span data-ttu-id="a6fe2-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-113">**Element**</span></span>|<span data-ttu-id="a6fe2-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a6fe2-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="a6fe2-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a6fe2-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a6fe2-117">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="a6fe2-118">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a6fe2-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="a6fe2-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a6fe2-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a6fe2-121">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="a6fe2-122">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a6fe2-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a6fe2-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a6fe2-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a6fe2-125">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a6fe2-126">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a6fe2-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a6fe2-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a6fe2-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a6fe2-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a6fe2-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a6fe2-130">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a><span data-ttu-id="a6fe2-131">Exemple de requête d’opération AddImContactToGroup : ajouter des contacts d’un message instantané existant à un groupe de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="a6fe2-131">AddImContactToGroup operation request example: Add an existing IM contact to an IM group</span></span>

<span data-ttu-id="a6fe2-132">Une requête d’opération **AddImContactToGroup** l’exemple suivant montre comment ajouter un contact de messagerie instantanée existant un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-132">The following example of an **AddImContactToGroup** operation request shows how to add an existing IM contact an IM group.</span></span> 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a6fe2-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a6fe2-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a6fe2-134">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-134">AddImContactToGroup</span></span>](addimcontacttogroup.md)
    
- [<span data-ttu-id="a6fe2-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="a6fe2-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="a6fe2-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="a6fe2-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a><span data-ttu-id="a6fe2-137">Réponse d’opération AddImContactToGroup réussie</span><span class="sxs-lookup"><span data-stu-id="a6fe2-137">Successful AddImContactToGroup operation response</span></span>

<span data-ttu-id="a6fe2-138">L’exemple suivant montre une réponse positive à une demande d’opération **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="a6fe2-138">The following example shows a successful response to an **AddImContactToGroup** operation request.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="a6fe2-139">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a6fe2-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a6fe2-140">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="a6fe2-140">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="a6fe2-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a6fe2-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="a6fe2-142">Opération AddImContactToGroup ErrorInvalidImContactId réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="a6fe2-142">AddImContactToGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="a6fe2-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddImContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="a6fe2-143">The following example shows an error response to an **AddImContactToGroup** operation request.</span></span> <span data-ttu-id="a6fe2-144">La réponse d’erreur se produit lorsqu’une tentative est effectuée pour ajouter un contact qui n’est pas un contact de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a6fe2-144">The following error response occurs when an attempt is made to add a contact that is not an IM contact.</span></span> 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="a6fe2-145">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a6fe2-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a6fe2-146">AddImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="a6fe2-146">AddImContactToGroupResponse</span></span>](addimcontacttogroupresponse.md)
    
- [<span data-ttu-id="a6fe2-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="a6fe2-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a6fe2-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a6fe2-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a6fe2-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a6fe2-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a6fe2-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a6fe2-150">See also</span></span>

- [<span data-ttu-id="a6fe2-151">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-151">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="a6fe2-152">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-152">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="a6fe2-153">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-153">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="a6fe2-154">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="a6fe2-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="a6fe2-155">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="a6fe2-155">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="a6fe2-156">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a6fe2-156">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

