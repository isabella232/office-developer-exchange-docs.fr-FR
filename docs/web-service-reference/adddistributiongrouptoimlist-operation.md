---
title: Opération AddDistributionGroupToImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Opération de recherche plus d’informations sur la AddDistributionGroupToImList EWS.
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755161"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="a790b-103">Opération AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="a790b-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="a790b-104">Trouvez des informations sur l’opération EWS **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="a790b-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="a790b-105">L’opération d’Exchange Web Services (EWS) **AddDistributionGroupToImList** ajoute un groupe de distribution à la liste (IM) dans le magasin de contacts unifié de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a790b-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="a790b-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a790b-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="a790b-107">Utilisation de l’opération AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="a790b-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="a790b-108">L’opération **AddDistributionGroupToImList** prend un argument unique qui identifie un groupe de distribution à ajouter à la liste de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a790b-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="a790b-109">Cette opération ne crée pas d’un groupe de distribution ; le groupe de distribution doit déjà être créé.</span><span class="sxs-lookup"><span data-stu-id="a790b-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="a790b-110">Cette opération peut utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="a790b-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="a790b-111">**Le tableau 1. En-têtes SOAP AddDistributionGroupToImList opération**</span><span class="sxs-lookup"><span data-stu-id="a790b-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="a790b-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="a790b-112">**Header name**</span></span>|<span data-ttu-id="a790b-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a790b-113">**Element**</span></span>|<span data-ttu-id="a790b-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a790b-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a790b-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="a790b-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="a790b-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a790b-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a790b-117">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="a790b-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="a790b-118">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="a790b-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a790b-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="a790b-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="a790b-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a790b-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a790b-121">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a790b-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="a790b-122">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="a790b-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a790b-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a790b-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a790b-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a790b-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a790b-125">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="a790b-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a790b-126">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="a790b-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a790b-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a790b-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a790b-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a790b-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a790b-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="a790b-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a790b-130">Cela s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="a790b-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="a790b-131">Exemple de requête d’opération AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="a790b-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="a790b-132">Une requête d’opération **AddDistributionGroupToImList** l’exemple suivant montre comment ajouter un groupe de distribution à la liste de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="a790b-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
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
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="a790b-133">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a790b-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a790b-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="a790b-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="a790b-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="a790b-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="a790b-136">Réponse d’opération AddDistributionGroupToImList réussie</span><span class="sxs-lookup"><span data-stu-id="a790b-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="a790b-137">L’exemple suivant montre une réponse positive à une demande d’opération **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="a790b-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="a790b-138">La réponse correcte contient le nom complet du groupe distribution, la classe de la banque Exchange pour le groupe de distribution et l’identificateur EWS du nouveau groupe de distribution.</span><span class="sxs-lookup"><span data-stu-id="a790b-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="a790b-139">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a790b-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a790b-140">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="a790b-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="a790b-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a790b-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a790b-142">ImGroup</span><span class="sxs-lookup"><span data-stu-id="a790b-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="a790b-143">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="a790b-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a790b-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="a790b-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="a790b-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="a790b-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="a790b-146">Opération AddDistributionGroupToImList ErrorInvalidImDistributionGroupSmtpAddress réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="a790b-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="a790b-147">L’exemple suivant montre une réponse d’erreur à une demande d’opération **AddDistributionGroupToImList** .</span><span class="sxs-lookup"><span data-stu-id="a790b-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="a790b-148">La réponse d’erreur se produit lorsqu’une tentative est effectuée pour ajouter un groupe de distribution qui n’existe pas dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="a790b-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
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
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="a790b-149">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="a790b-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a790b-150">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="a790b-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="a790b-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="a790b-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a790b-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a790b-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a790b-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a790b-153">See also</span></span>

- [<span data-ttu-id="a790b-154">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a790b-154">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="a790b-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="a790b-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="a790b-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="a790b-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

