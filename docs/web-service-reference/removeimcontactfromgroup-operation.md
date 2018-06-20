---
title: Opération RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Opération de recherche plus d’informations sur la RemoveImContactFromGroup EWS.
ms.openlocfilehash: 8c9af251014dbddabb439ed5bf5dc35580da6a90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829099"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="5b9f9-103">Opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="5b9f9-104">Trouvez des informations sur l’opération EWS **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="5b9f9-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="5b9f9-105">L’opération **RemoveImContactFromGroup** supprime un contact de messagerie instantanée à partir d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="5b9f9-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="5b9f9-107">Utilisation de l’opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="5b9f9-108">L’opération **RemoveImContactFromGroup** prend deux arguments : un identificateur de l’élément de contact et le groupe (IM) à partir de laquelle le contact est supprimé de pic correspondant.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="5b9f9-109">En-têtes SOAP RemoveImContactFromGroup opération</span><span class="sxs-lookup"><span data-stu-id="5b9f9-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="5b9f9-110">L’opération **RemoveImContactFromGroup** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5b9f9-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-111">**Header name**</span></span>|<span data-ttu-id="5b9f9-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-112">**Element**</span></span>|<span data-ttu-id="5b9f9-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5b9f9-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="5b9f9-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="5b9f9-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="5b9f9-116">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="5b9f9-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b9f9-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="5b9f9-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="5b9f9-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="5b9f9-120">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="5b9f9-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b9f9-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5b9f9-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="5b9f9-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5b9f9-124">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5b9f9-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5b9f9-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="5b9f9-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5b9f9-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5b9f9-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5b9f9-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5b9f9-129">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="5b9f9-130">Exemple de requête d’opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="5b9f9-131">Une demande d’opération **RemoveImContactFromGroup** l’exemple suivant montre comment supprimer un contact de messagerie instantanée d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5b9f9-132">Les identificateurs de groupe et contacts ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5b9f9-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5b9f9-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b9f9-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="5b9f9-135">ContactId</span><span class="sxs-lookup"><span data-stu-id="5b9f9-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="5b9f9-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="5b9f9-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="5b9f9-137">Réponse d’opération RemoveImContactFromGroup réussie</span><span class="sxs-lookup"><span data-stu-id="5b9f9-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="5b9f9-138">L’exemple suivant montre une réponse positive à une demande d’opération **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="5b9f9-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5b9f9-139">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5b9f9-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b9f9-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="5b9f9-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="5b9f9-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5b9f9-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="5b9f9-142">Opération RemoveImContactFromGroup ErrorInvalidImContactId réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="5b9f9-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="5b9f9-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="5b9f9-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="5b9f9-144">La réponse d’erreur se produit lorsqu’une tentative est effectuée pour supprimer un élément de contact qui n’existe pas dans le groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="5b9f9-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="5b9f9-145">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="5b9f9-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5b9f9-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="5b9f9-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="5b9f9-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="5b9f9-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5b9f9-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5b9f9-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5b9f9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5b9f9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="5b9f9-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5b9f9-150">See also</span></span>

- [<span data-ttu-id="5b9f9-151">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5b9f9-151">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="5b9f9-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="5b9f9-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="5b9f9-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="5b9f9-154">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="5b9f9-155">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="5b9f9-156">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="5b9f9-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="5b9f9-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="5b9f9-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="5b9f9-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="5b9f9-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="5b9f9-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="5b9f9-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="5b9f9-160">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="5b9f9-161">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="5b9f9-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="5b9f9-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="5b9f9-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

