---
title: Opération RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Trouvez des informations sur l’opération EWS RemoveDistributionGroupFromImList.
ms.openlocfilehash: 66220f0cab99f404e17136bbb7836ca13d569b53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459601"
---
# <a name="removedistributiongroupfromimlist-operation"></a><span data-ttu-id="93e41-103">Opération RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="93e41-103">RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="93e41-104">Trouvez des informations sur l’opération EWS **RemoveDistributionGroupFromImList** .</span><span class="sxs-lookup"><span data-stu-id="93e41-104">Find information about the **RemoveDistributionGroupFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="93e41-105">L’opération **RemoveDistributionGroupFromImList** supprime un groupe de distribution de la liste de messagerie instantanée (im) Lync lorsque Lync utilise Exchange pour le magasin de contacts.</span><span class="sxs-lookup"><span data-stu-id="93e41-105">The **RemoveDistributionGroupFromImList** operation removes a distribution group from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="93e41-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="93e41-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a><span data-ttu-id="93e41-107">Utilisation de l’opération RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="93e41-107">Using the RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="93e41-108">L’opération **RemoveDistributionGroupFromImList** accepte un seul argument qui identifie un groupe de distribution à supprimer de la liste de messagerie instantanée Lync stockée sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="93e41-108">The **RemoveDistributionGroupFromImList** operation accepts a single argument that identifies a distribution group to remove from the Lync IM list stored on an Exchange server.</span></span> 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a><span data-ttu-id="93e41-109">En-têtes SOAP d’opération RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="93e41-109">RemoveDistributionGroupFromImList operation SOAP headers</span></span>

<span data-ttu-id="93e41-110">L’opération **RemoveDistributionGroupFromImList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="93e41-110">The **RemoveDistributionGroupFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="93e41-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="93e41-111">**Header name**</span></span>|<span data-ttu-id="93e41-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="93e41-112">**Element**</span></span>|<span data-ttu-id="93e41-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="93e41-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="93e41-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="93e41-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="93e41-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="93e41-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="93e41-116">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="93e41-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="93e41-117">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="93e41-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="93e41-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="93e41-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="93e41-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="93e41-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="93e41-120">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="93e41-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="93e41-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="93e41-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="93e41-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="93e41-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="93e41-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="93e41-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="93e41-124">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="93e41-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="93e41-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="93e41-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="93e41-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="93e41-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="93e41-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="93e41-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="93e41-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="93e41-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="93e41-129">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="93e41-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a><span data-ttu-id="93e41-130">Exemple de requête d’opération RemoveDistributionGroupFromImList : supprimer un groupe de distribution d’une liste de messagerie instantanée</span><span class="sxs-lookup"><span data-stu-id="93e41-130">RemoveDistributionGroupFromImList operation request example: Remove a distribution group from an IM list</span></span>

<span data-ttu-id="93e41-131">L’exemple suivant de demande d’opération **RemoveDistributionGroupFromImList** montre comment supprimer un groupe de distribution d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="93e41-131">The following example of a **RemoveDistributionGroupFromImList** operation request shows how to remove a distribution group from an IM group.</span></span> <span data-ttu-id="93e41-132">L’opération **RemoveDistributionGroupFromImList** accepte l’identificateur unique de groupe pour identifier le groupe de distribution à supprimer de la liste de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="93e41-132">The **RemoveDistributionGroupFromImList** operation accepts the unique group identifier to identify the distribution group to remove from the IM list.</span></span> <span data-ttu-id="93e41-133">L’élément [ExchangeStoreId](exchangestoreid.md) renvoyé dans la réponse pour l' [opération GetImItemList](getimitemlist-operation.md) et l' [opération AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) identifie les groupes de distribution qui peuvent être supprimés de la liste de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="93e41-133">The [ExchangeStoreId](exchangestoreid.md) element that is returned in the response for the [GetImItemList operation](getimitemlist-operation.md) and the [AddDistributionGroupToImList operation](adddistributiongrouptoimlist-operation.md) identifies distribution groups that can be removed from the IM list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="93e41-134">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="93e41-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="93e41-135">Les éléments suivants sont utilisés dans le corps SOAP de la demande :</span><span class="sxs-lookup"><span data-stu-id="93e41-135">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="93e41-136">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="93e41-136">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist.md)
    
- [<span data-ttu-id="93e41-137">GroupId</span><span class="sxs-lookup"><span data-stu-id="93e41-137">GroupId</span></span>](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a><span data-ttu-id="93e41-138">Réponse de l’opération RemoveDistributionGroupFromImList réussie</span><span class="sxs-lookup"><span data-stu-id="93e41-138">Successful RemoveDistributionGroupFromImList operation response</span></span>

<span data-ttu-id="93e41-139">L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveDistributionGroupFromImList** à une suppression d’un groupe de distribution d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="93e41-139">The following example shows a successful response to a **RemoveDistributionGroupFromImList** operation request to a remove a distribution group from an IM group.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="93e41-140">Les éléments suivants sont utilisés dans le corps SOAP de réponse :</span><span class="sxs-lookup"><span data-stu-id="93e41-140">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="93e41-141">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="93e41-141">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="93e41-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="93e41-142">ResponseCode</span></span>](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a><span data-ttu-id="93e41-143">Exemple de réponse d’erreur d’opération RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="93e41-143">RemoveDistributionGroupFromImList operation error response example</span></span>

<span data-ttu-id="93e41-144">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveDistributionGroupFromImList** .</span><span class="sxs-lookup"><span data-stu-id="93e41-144">The following example shows an error response to a **RemoveDistributionGroupFromImList** operation request.</span></span> <span data-ttu-id="93e41-145">Réponse à une demande de suppression d’un groupe de distribution qui a déjà été supprimé de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="93e41-145">This is a response to a request to remove a distribution group that has already been removed from the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="93e41-146">Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :</span><span class="sxs-lookup"><span data-stu-id="93e41-146">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="93e41-147">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="93e41-147">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="93e41-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="93e41-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="93e41-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="93e41-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="93e41-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="93e41-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="93e41-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="93e41-151">See also</span></span>

- [<span data-ttu-id="93e41-152">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="93e41-152">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="93e41-153">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="93e41-153">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="93e41-154">Opération AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="93e41-154">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="93e41-155">Personnes et contacts dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="93e41-155">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

