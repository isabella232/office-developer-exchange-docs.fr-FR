---
title: Opération EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: L’opération EmptyFolder vide des dossiers dans une boîte aux lettres. Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié. Lorsqu’un sous-dossier est supprimé, le sous-dossier et les messages dans le sous-dossier sont supprimés.
ms.openlocfilehash: 0192744516c5a6d24b95915452bfcffecc2d92b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756152"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="648fc-105">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="648fc-105">EmptyFolder operation</span></span>

<span data-ttu-id="648fc-106">L’opération **EmptyFolder** vide des dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="648fc-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="648fc-107">Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="648fc-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="648fc-108">Lorsqu’un sous-dossier est supprimé, le sous-dossier et les messages dans le sous-dossier sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="648fc-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="648fc-109">Exemple de requête EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="648fc-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="648fc-110">Description</span><span class="sxs-lookup"><span data-stu-id="648fc-110">Description</span></span>

<span data-ttu-id="648fc-111">L’exemple suivant d’une demande **EmptyFolder** montre comment former une demande pour vider un dossier.</span><span class="sxs-lookup"><span data-stu-id="648fc-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="648fc-112">Cet exemple supprime tous les sous-dossiers du dossier identifié.</span><span class="sxs-lookup"><span data-stu-id="648fc-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="648fc-113">Les valeurs de l' **Id** et les attributs **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="648fc-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="648fc-114">Code</span><span class="sxs-lookup"><span data-stu-id="648fc-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
    </soap:Header>
    <soap:Body>
      <m:EmptyFolder DeleteType="HardDelete" DeleteSubFolders="true">
        <m:FolderIds>
          <t:FolderId Id="AQMkADhhOGU0"  ChangeKey="AQAAABYAAABsMB" />
        </m:FolderIds>
      </m:EmptyFolder>
    </soap:Body>
</soap:Envelope>

```

### <a name="comments"></a><span data-ttu-id="648fc-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="648fc-115">Comments</span></span>

<span data-ttu-id="648fc-116">Cet exemple effectue une suppression définitive sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="648fc-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="648fc-117">Dossiers peuvent être identifiés par l’élément [DistinguishedFolderId](distinguishedfolderid.md) ou de l’élément [FolderId](folderid.md) pour une utilisation dans l’élément [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="648fc-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="648fc-118">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="648fc-118">Request elements</span></span>

<span data-ttu-id="648fc-119">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="648fc-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="648fc-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="648fc-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="648fc-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="648fc-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="648fc-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="648fc-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="648fc-123">Réponse EmptyFolder réussie</span><span class="sxs-lookup"><span data-stu-id="648fc-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="648fc-124">Description</span><span class="sxs-lookup"><span data-stu-id="648fc-124">Description</span></span>

<span data-ttu-id="648fc-125">L’exemple suivant montre une réponse positive à la demande **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="648fc-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="648fc-126">Code</span><span class="sxs-lookup"><span data-stu-id="648fc-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="648fc-127">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="648fc-127">Successful response elements</span></span>

<span data-ttu-id="648fc-128">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="648fc-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="648fc-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="648fc-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="648fc-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="648fc-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="648fc-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="648fc-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="648fc-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="648fc-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="648fc-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="648fc-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="648fc-134">Réponse d’erreur EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="648fc-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="648fc-135">Description</span><span class="sxs-lookup"><span data-stu-id="648fc-135">Description</span></span>

<span data-ttu-id="648fc-136">L’exemple suivant montre une réponse d’erreur à une demande **Emptyfolder** .</span><span class="sxs-lookup"><span data-stu-id="648fc-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="648fc-137">L’erreur a été créé, car l’opération a tenté de vider un dossier est introuvable dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="648fc-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="648fc-138">Code</span><span class="sxs-lookup"><span data-stu-id="648fc-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="648fc-139">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="648fc-139">Error response elements</span></span>

<span data-ttu-id="648fc-140">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="648fc-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="648fc-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="648fc-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="648fc-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="648fc-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="648fc-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="648fc-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="648fc-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="648fc-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="648fc-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="648fc-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="648fc-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="648fc-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="648fc-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="648fc-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="648fc-148">Dossiers</span><span class="sxs-lookup"><span data-stu-id="648fc-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="648fc-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="648fc-149">See also</span></span>

- [<span data-ttu-id="648fc-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="648fc-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

