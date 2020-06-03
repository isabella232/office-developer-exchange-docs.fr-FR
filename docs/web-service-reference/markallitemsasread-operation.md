---
title: Opération MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Trouvez des informations sur l’opération EWS MarkAllItemsAsRead.
ms.openlocfilehash: aeeacea1cd5eed723f93027dd1ef75b34605fdfd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530529"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="73c80-103">Opération MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="73c80-104">Trouvez des informations sur l’opération EWS **MarkAllItemsAsRead** .</span><span class="sxs-lookup"><span data-stu-id="73c80-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="73c80-105">L’opération **MarkAllItemsAsRead** définit la propriété [IsRead](isread.md) sur tous les éléments, dans un ou plusieurs dossiers, pour indiquer que tous les éléments sont lus ou non lus.</span><span class="sxs-lookup"><span data-stu-id="73c80-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="73c80-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="73c80-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="73c80-107">Utilisation de l’opération MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="73c80-108">L’opération **MarkAllItemsAsRead** peut définir la propriété [IsRead](isread.md) sur tous les éléments dans les dossiers identifiés par l’identificateur de dossier des services Web Exchange (EWS) ou par le nom de dossier Exchange par défaut.</span><span class="sxs-lookup"><span data-stu-id="73c80-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="73c80-109">L’opération **MarkAllItemsAsRead** peut également supprimer l’envoi de confirmations de lecture pour les éléments marqués comme lus.</span><span class="sxs-lookup"><span data-stu-id="73c80-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="73c80-110">En-têtes SOAP d’opération MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="73c80-111">L’opération **MarkAllItemsAsRead** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="73c80-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="73c80-112">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="73c80-112">**Header name**</span></span>|<span data-ttu-id="73c80-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="73c80-113">**Element**</span></span>|<span data-ttu-id="73c80-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="73c80-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="73c80-115">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="73c80-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="73c80-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="73c80-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="73c80-117">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="73c80-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="73c80-118">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="73c80-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73c80-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="73c80-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="73c80-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="73c80-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="73c80-121">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="73c80-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="73c80-122">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="73c80-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73c80-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="73c80-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="73c80-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="73c80-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="73c80-125">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="73c80-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="73c80-126">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="73c80-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="73c80-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="73c80-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="73c80-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="73c80-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="73c80-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="73c80-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="73c80-130">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="73c80-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="73c80-131">Exemple de requête d’opération MarkAllItemsAsRead : marquer tous les éléments d’un dossier comme lus</span><span class="sxs-lookup"><span data-stu-id="73c80-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="73c80-132">L’exemple suivant de demande d’opération **MarkAllItemsAsRead** indique comment définir la propriété [IsRead](isread.md) , qui est également appelée indicateur de lecture, à **true** pour tous les éléments d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="73c80-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="73c80-133">Cet exemple montre également que les confirmations de lecture ne sont pas envoyées en réponse à des demandes de confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="73c80-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="73c80-134">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="73c80-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="73c80-135">Les clés de modification ne sont pas requises pour cette opération.</span><span class="sxs-lookup"><span data-stu-id="73c80-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="73c80-136">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="73c80-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73c80-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="73c80-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="73c80-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="73c80-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="73c80-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="73c80-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="73c80-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="73c80-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="73c80-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="73c80-142">Réponse de l’opération MarkAllItemsAsRead réussie</span><span class="sxs-lookup"><span data-stu-id="73c80-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="73c80-143">L’exemple suivant montre une réponse réussie à une demande d’opération **MarkAllItemsAsRead** pour marquer tous les éléments d’un dossier comme étant lus.</span><span class="sxs-lookup"><span data-stu-id="73c80-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="73c80-144">Le corps SOAP de réponse contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="73c80-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73c80-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="73c80-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="73c80-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="73c80-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="73c80-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73c80-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="73c80-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="73c80-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="73c80-149">Exemple de requête d’opération MarkAllItemsAsRead : marquer tous les éléments d’un dossier comme non lus</span><span class="sxs-lookup"><span data-stu-id="73c80-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="73c80-150">L’exemple suivant de demande d’opération **MarkAllItemsAsRead** indique comment définir la propriété [IsRead](isread.md) sur **false** sur tous les éléments d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="73c80-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="73c80-151">Cet exemple montre également que les confirmations de lecture ne sont pas envoyées en réponse à des demandes de confirmation de lecture.</span><span class="sxs-lookup"><span data-stu-id="73c80-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="73c80-152">Une réponse réussie à une demande de marquage de tous les éléments comme lus est identique à la réponse à une demande de marquage de tous les éléments comme non lus.</span><span class="sxs-lookup"><span data-stu-id="73c80-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="73c80-153">Le corps SOAP de la demande contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="73c80-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73c80-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="73c80-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="73c80-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="73c80-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="73c80-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="73c80-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="73c80-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="73c80-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="73c80-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="73c80-159">Réponse d’erreur d’opération MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="73c80-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="73c80-160">L’exemple suivant montre une réponse d’erreur à une demande d’opération **MarkAllItemsAsRead** pour marquer tous les éléments d’un dossier comme lus ou non lus lorsque le dossier n’existe pas dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="73c80-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="73c80-161">Le corps SOAP de la réponse d’erreur contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="73c80-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="73c80-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="73c80-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="73c80-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="73c80-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="73c80-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="73c80-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="73c80-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="73c80-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="73c80-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="73c80-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="73c80-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="73c80-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="73c80-168">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="73c80-168">See also</span></span>

- [<span data-ttu-id="73c80-169">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="73c80-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="73c80-170">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="73c80-170">FindFolder operation</span></span>](findfolder-operation.md)
    

