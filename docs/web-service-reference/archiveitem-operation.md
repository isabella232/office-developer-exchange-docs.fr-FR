---
title: Opération ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Opération de recherche plus d’informations sur la ArchiveItem EWS.
ms.openlocfilehash: 954943acefef8da61e92de5f8857ca023ca4fc9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755317"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="75240-103">Opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="75240-103">ArchiveItem operation</span></span>

<span data-ttu-id="75240-104">Trouvez des informations sur l’opération EWS **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="75240-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="75240-105">L’opération **ArchiveItem** déplace un élément dans la boîte aux lettres d’archive boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="75240-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="75240-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="75240-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="75240-107">Utilisation de l’opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="75240-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="75240-108">L’opération **ArchiveItem** prend deux arguments dans la demande qui identifient les éléments à déplacer vers la boîte aux lettres d’archivage et le dossier de destination pour ces éléments.</span><span class="sxs-lookup"><span data-stu-id="75240-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="75240-109">Une boîte aux lettres d’archivage doit être activé pour cette opération travailler.</span><span class="sxs-lookup"><span data-stu-id="75240-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="75240-110">Pour plus d’informations sur la façon d’activer une boîte aux lettres d’archivage, voir [Gérer les Archives locales](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span><span class="sxs-lookup"><span data-stu-id="75240-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="75240-111">En-têtes SOAP ArchiveItem opération</span><span class="sxs-lookup"><span data-stu-id="75240-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="75240-112">L’opération **ArchiveItem** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="75240-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="75240-113">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="75240-113">**Header name**</span></span>|<span data-ttu-id="75240-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="75240-114">**Element**</span></span>|<span data-ttu-id="75240-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="75240-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="75240-116">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="75240-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="75240-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="75240-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="75240-118">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="75240-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="75240-119">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="75240-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="75240-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="75240-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="75240-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="75240-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="75240-122">Identifie la culture, comme défini dans RFC 3066, **des balises pour l’Identification des langues**à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="75240-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="75240-123">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="75240-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="75240-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="75240-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="75240-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="75240-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="75240-126">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="75240-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="75240-127">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="75240-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="75240-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="75240-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="75240-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="75240-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="75240-130">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="75240-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="75240-131">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="75240-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="75240-132">Exemple de requête d’opération ArchiveItem : déplacer un élément vers le dossier boîte de réception d’archivage</span><span class="sxs-lookup"><span data-stu-id="75240-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="75240-133">Une requête d’opération **ArchiveItem** l’exemple suivant montre comment déplacer un élément vers le dossier boîte de réception de l’archive.</span><span class="sxs-lookup"><span data-stu-id="75240-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="75240-134">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="75240-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="75240-135">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="75240-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="75240-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="75240-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="75240-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="75240-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="75240-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="75240-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="75240-139">ItemId</span><span class="sxs-lookup"><span data-stu-id="75240-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="75240-140">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="75240-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="75240-141">Réponse d’opération ArchiveItem réussie</span><span class="sxs-lookup"><span data-stu-id="75240-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="75240-142">L’exemple suivant montre une réponse positive à une demande d’opération **ArchiveItem** pour déplacer un élément vers une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="75240-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="75240-143">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="75240-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="75240-144">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="75240-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="75240-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="75240-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="75240-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="75240-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="75240-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="75240-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="75240-148">Items</span><span class="sxs-lookup"><span data-stu-id="75240-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="75240-149">Réponse d’erreur d’opération ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="75240-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="75240-150">L’exemple suivant montre une réponse d’erreur à une demande d’opération **ArchiveItem** .</span><span class="sxs-lookup"><span data-stu-id="75240-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="75240-151">Il s’agit d’une réponse à une demande d’archiver un élément lorsqu’une boîte aux lettres d’archivage n’est pas activée pour un utilisateur valide.</span><span class="sxs-lookup"><span data-stu-id="75240-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="75240-152">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="75240-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="75240-153">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="75240-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="75240-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="75240-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="75240-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="75240-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="75240-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="75240-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="75240-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="75240-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="75240-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="75240-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="75240-159">Items</span><span class="sxs-lookup"><span data-stu-id="75240-159">Items</span></span>](items.md)
    
<span data-ttu-id="75240-160">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="75240-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="75240-161">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="75240-161">See also</span></span>

- [<span data-ttu-id="75240-162">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="75240-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="75240-163">L'archivage dans EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="75240-163">Archiving in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

