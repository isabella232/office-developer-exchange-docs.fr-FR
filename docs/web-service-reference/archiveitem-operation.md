---
title: Opération ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Trouvez des informations sur l’opération EWS ArchiveItem.
ms.openlocfilehash: d1e18122e67c36babbc8bf01d305309e2b17b568
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463432"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="63fea-103">Opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="63fea-103">ArchiveItem operation</span></span>

<span data-ttu-id="63fea-104">Trouvez des informations sur l’opération EWS **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="63fea-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="63fea-105">L’opération **ArchiveItem** déplace un élément vers la boîte aux lettres d’archivage de l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="63fea-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="63fea-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="63fea-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="63fea-107">Utilisation de l’opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="63fea-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="63fea-108">L’opération **ArchiveItem** prend deux arguments dans la demande qui identifie les éléments à déplacer vers la boîte aux lettres d’archivage et le dossier de destination de ces éléments.</span><span class="sxs-lookup"><span data-stu-id="63fea-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="63fea-109">Une boîte aux lettres d’archivage doit être activée pour que cette opération fonctionne.</span><span class="sxs-lookup"><span data-stu-id="63fea-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="63fea-110">Pour plus d’informations sur l’activation d’une boîte aux lettres d’archivage, consultez la rubrique [Manage in-place Archive](https://technet.microsoft.com/library/jj651146.aspx).</span><span class="sxs-lookup"><span data-stu-id="63fea-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](https://technet.microsoft.com/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="63fea-111">En-têtes SOAP d’opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="63fea-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="63fea-112">L’opération **ArchiveItem** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="63fea-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="63fea-113">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="63fea-113">**Header name**</span></span>|<span data-ttu-id="63fea-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="63fea-114">**Element**</span></span>|<span data-ttu-id="63fea-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="63fea-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="63fea-116">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="63fea-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="63fea-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="63fea-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="63fea-118">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="63fea-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="63fea-119">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="63fea-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="63fea-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="63fea-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="63fea-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="63fea-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="63fea-122">Identifie la culture, telle que définie dans la norme RFC 3066, **pour l’identification des langues**, à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="63fea-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="63fea-123">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="63fea-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="63fea-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="63fea-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="63fea-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="63fea-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="63fea-126">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="63fea-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="63fea-127">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="63fea-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="63fea-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="63fea-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="63fea-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="63fea-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="63fea-130">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="63fea-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="63fea-131">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="63fea-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="63fea-132">Exemple de requête d’opération ArchiveItem : déplacer un élément vers le dossier boîte de réception d’archivage</span><span class="sxs-lookup"><span data-stu-id="63fea-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="63fea-133">L’exemple suivant de demande d’opération **ArchiveItem** indique comment déplacer un élément vers le dossier boîte de réception d’archive.</span><span class="sxs-lookup"><span data-stu-id="63fea-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="63fea-134">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="63fea-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="63fea-135">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="63fea-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="63fea-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="63fea-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="63fea-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="63fea-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="63fea-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="63fea-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="63fea-139">ItemIds</span><span class="sxs-lookup"><span data-stu-id="63fea-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="63fea-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="63fea-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="63fea-141">Réponse de l’opération ArchiveItem réussie</span><span class="sxs-lookup"><span data-stu-id="63fea-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="63fea-142">L’exemple suivant montre une réponse réussie à une demande d’opération **ArchiveItem** pour déplacer un élément vers une boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="63fea-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="63fea-143">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="63fea-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="63fea-144">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="63fea-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="63fea-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="63fea-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="63fea-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="63fea-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="63fea-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="63fea-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="63fea-148">Items</span><span class="sxs-lookup"><span data-stu-id="63fea-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="63fea-149">Réponse d’erreur d’opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="63fea-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="63fea-150">L’exemple suivant montre une réponse d’erreur à une demande d’opération **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="63fea-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="63fea-151">Il s’agit d’une réponse à une demande valide d’archivage d’un élément lorsqu’une boîte aux lettres d’archivage n’est pas activée pour un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="63fea-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
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
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="63fea-152">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="63fea-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="63fea-153">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="63fea-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="63fea-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="63fea-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="63fea-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="63fea-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="63fea-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="63fea-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="63fea-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="63fea-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="63fea-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="63fea-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="63fea-159">Items</span><span class="sxs-lookup"><span data-stu-id="63fea-159">Items</span></span>](items.md)
    
<span data-ttu-id="63fea-160">Pour les autres codes d’erreur qui sont génériques à EWS et spécifiques à cette opération, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="63fea-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="63fea-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="63fea-161">See also</span></span>

- [<span data-ttu-id="63fea-162">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63fea-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="63fea-163">L'archivage dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="63fea-163">Archiving in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

