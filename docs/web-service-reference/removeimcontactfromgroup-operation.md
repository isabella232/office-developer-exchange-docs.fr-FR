---
title: Opération RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a190bbec-c71b-4e6a-880b-55854c724d8c
description: Trouvez des informations sur l’opération EWS RemoveImContactFromGroup.
ms.openlocfilehash: 4750ef57794c3da540ac36baa8ef6ef093939ea1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466968"
---
# <a name="removeimcontactfromgroup-operation"></a><span data-ttu-id="3e3ce-103">Opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-103">RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="3e3ce-104">Trouvez des informations sur l’opération EWS **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="3e3ce-104">Find information about the **RemoveImContactFromGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3e3ce-105">L’opération **RemoveImContactFromGroup** supprime un seul contact de messagerie instantanée d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-105">The **RemoveImContactFromGroup** operation removes a single IM contact from an IM group.</span></span> 
  
<span data-ttu-id="3e3ce-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimcontactfromgroup-operation"></a><span data-ttu-id="3e3ce-107">Utilisation de l’opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-107">Using the RemoveImContactFromGroup operation</span></span>

<span data-ttu-id="3e3ce-108">L’opération **RemoveImContactFromGroup** prend deux arguments : un identificateur d’élément de contact et le groupe de messagerie instantanée (im) correspondant à partir duquel le contact est supprimé.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-108">The **RemoveImContactFromGroup** operation takes two arguments: a contact item identifier, and the corresponding instant messaging (IM) group from which the contact is removed.</span></span> 
  
### <a name="removeimcontactfromgroup-operation-soap-headers"></a><span data-ttu-id="3e3ce-109">En-têtes SOAP d’opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-109">RemoveImContactFromGroup operation SOAP headers</span></span>

<span data-ttu-id="3e3ce-110">L’opération **RemoveImContactFromGroup** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-110">The **RemoveImContactFromGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3e3ce-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-111">**Header name**</span></span>|<span data-ttu-id="3e3ce-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-112">**Element**</span></span>|<span data-ttu-id="3e3ce-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3e3ce-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3e3ce-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3e3ce-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3e3ce-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3e3ce-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3e3ce-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3e3ce-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3e3ce-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3e3ce-120">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3e3ce-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3e3ce-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3e3ce-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3e3ce-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3e3ce-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3e3ce-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3e3ce-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3e3ce-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3e3ce-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3e3ce-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3e3ce-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3e3ce-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimcontactfromgroup-operation-request-example"></a><span data-ttu-id="3e3ce-130">Exemple de requête d’opération RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-130">RemoveImContactFromGroup operation request example</span></span>

<span data-ttu-id="3e3ce-131">L’exemple suivant de demande d’opération **RemoveImContactFromGroup** montre comment supprimer un contact de messagerie instantanée d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-131">The following example of a **RemoveImContactFromGroup** operation request shows how to remove an IM contact from an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="3e3ce-132">Les identificateurs de contact et de groupe ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-132">The group and contact identifiers have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImContactFromGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTcAAAAvcAAA="
                      ChangeKey="EQAAABYAAABtF8oI7iVOQ"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkbWAAAAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImContactFromGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3e3ce-133">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3e3ce-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3e3ce-134">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-134">RemoveImContactFromGroup</span></span>](removeimcontactfromgroup.md)
    
- [<span data-ttu-id="3e3ce-135">Mettez</span><span class="sxs-lookup"><span data-stu-id="3e3ce-135">ContactId</span></span>](contactid.md)
    
- [<span data-ttu-id="3e3ce-136">GroupId</span><span class="sxs-lookup"><span data-stu-id="3e3ce-136">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimcontactfromgroup-operation-response"></a><span data-ttu-id="3e3ce-137">Réponse de l’opération RemoveImContactFromGroup réussie</span><span class="sxs-lookup"><span data-stu-id="3e3ce-137">Successful RemoveImContactFromGroup operation response</span></span>

<span data-ttu-id="3e3ce-138">L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="3e3ce-138">The following example shows a successful response to a **RemoveImContactFromGroup** operation request.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Success" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3e3ce-139">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3e3ce-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3e3ce-140">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3e3ce-140">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="3e3ce-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3e3ce-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimcontactfromgroup-operation-errorinvalidimcontactid-error-response"></a><span data-ttu-id="3e3ce-142">RemoveImContactFromGroup Operation ErrorInvalidImContactId Error Response</span><span class="sxs-lookup"><span data-stu-id="3e3ce-142">RemoveImContactFromGroup operation ErrorInvalidImContactId error response</span></span>

<span data-ttu-id="3e3ce-143">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveImContactFromGroup** .</span><span class="sxs-lookup"><span data-stu-id="3e3ce-143">The following example shows an error response to a **RemoveImContactFromGroup** operation request.</span></span> <span data-ttu-id="3e3ce-144">La réponse d’erreur suivante se produit lorsqu’une tentative de suppression d’un élément de contact qui n’existe pas dans le groupe de messagerie instantanée est effectuée.</span><span class="sxs-lookup"><span data-stu-id="3e3ce-144">The following error response occurs when an attempt is made to remove a contact item that does not exist in the IM group.</span></span> 
  
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
      <RemoveImContactFromGroupResponse ResponseClass="Error" 
                                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImContactFromGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3e3ce-145">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="3e3ce-145">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3e3ce-146">RemoveImContactFromGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3e3ce-146">RemoveImContactFromGroupResponse</span></span>](removeimcontactfromgroupresponse.md)
    
- [<span data-ttu-id="3e3ce-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="3e3ce-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3e3ce-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3e3ce-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3e3ce-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3e3ce-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3e3ce-150">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3e3ce-150">See also</span></span>

- [<span data-ttu-id="3e3ce-151">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="3e3ce-151">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3e3ce-152">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="3e3ce-152">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="3e3ce-153">AddImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-153">AddImContactToGroup</span></span>](addimcontacttogroup-operation.md)
    
- [<span data-ttu-id="3e3ce-154">Opération AddImGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-154">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="3e3ce-155">Opération AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-155">AddNewImContactToGroup operation</span></span>](addnewimcontacttogroup-operation.md)
    
- [<span data-ttu-id="3e3ce-156">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="3e3ce-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="3e3ce-157">GetImItems</span><span class="sxs-lookup"><span data-stu-id="3e3ce-157">GetImItems</span></span>](getimitems-operation.md)
    
- [<span data-ttu-id="3e3ce-158">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="3e3ce-158">RemoveContactFromImList</span></span>](removecontactfromimlist-operation.md)
    
- [<span data-ttu-id="3e3ce-159">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="3e3ce-159">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist-operation.md)
    
- [<span data-ttu-id="3e3ce-160">Opération RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-160">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="3e3ce-161">Opération SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3e3ce-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    
- [<span data-ttu-id="3e3ce-162">SetImListMigrationCompleted</span><span class="sxs-lookup"><span data-stu-id="3e3ce-162">SetImListMigrationCompleted</span></span>](setimlistmigrationcompleted-operation.md)
    

