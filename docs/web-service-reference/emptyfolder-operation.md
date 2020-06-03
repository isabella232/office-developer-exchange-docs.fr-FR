---
title: Opération EmptyFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 98161486-e2f2-480f-8d5d-708ba81b208a
description: L’opération EmptyFolder vide les dossiers dans une boîte aux lettres. Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié. Lors de la suppression d’un sous-dossier, le sous-dossier et les messages qu’il contient sont supprimés.
ms.openlocfilehash: 1913db74d33f1e6750cd158df5870f257d0e7839
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530683"
---
# <a name="emptyfolder-operation"></a><span data-ttu-id="f867c-105">Opération EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="f867c-105">EmptyFolder operation</span></span>

<span data-ttu-id="f867c-106">L’opération **EmptyFolder** vide les dossiers dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f867c-106">The **EmptyFolder** operation empties folders in a mailbox.</span></span> <span data-ttu-id="f867c-107">Si vous le souhaitez, cette opération vous permet de supprimer les sous-dossiers du dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="f867c-107">Optionally, this operation enables you to delete the subfolders of the specified folder.</span></span> <span data-ttu-id="f867c-108">Lors de la suppression d’un sous-dossier, le sous-dossier et les messages qu’il contient sont supprimés.</span><span class="sxs-lookup"><span data-stu-id="f867c-108">When a subfolder is deleted, the subfolder and the messages within the subfolder are deleted.</span></span> 
  
## <a name="emptyfolder-request-example"></a><span data-ttu-id="f867c-109">Exemple de requête EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="f867c-109">EmptyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="f867c-110">Description</span><span class="sxs-lookup"><span data-stu-id="f867c-110">Description</span></span>

<span data-ttu-id="f867c-111">L’exemple de requête **EmptyFolder** suivant montre comment créer une demande de vidage d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="f867c-111">This following example of an **EmptyFolder** request shows how to form a request to empty a folder.</span></span> <span data-ttu-id="f867c-112">Cet exemple supprime tous les sous-dossiers du dossier identifié.</span><span class="sxs-lookup"><span data-stu-id="f867c-112">This example deletes all subfolders of the identified folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f867c-113">Les valeurs des attributs **ID** et **ChangeKey** de l’élément [FolderId](folderid.md) ont été raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f867c-113">The values of the **Id** and the **ChangeKey** attributes of the [FolderId](folderid.md) element have been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f867c-114">Code</span><span class="sxs-lookup"><span data-stu-id="f867c-114">Code</span></span>

```XML
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="f867c-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="f867c-115">Comments</span></span>

<span data-ttu-id="f867c-116">Cet exemple effectue une suppression définitive sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="f867c-116">This example performs a hard delete on the folder.</span></span>
  
<span data-ttu-id="f867c-117">Les dossiers peuvent être identifiés par l’élément [DistinguishedFolderId](distinguishedfolderid.md) ou l’élément [FolderId](folderid.md) pour une utilisation dans l’élément [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="f867c-117">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in the [FolderIds](folderids.md) element.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="f867c-118">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="f867c-118">Request elements</span></span>

<span data-ttu-id="f867c-119">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="f867c-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f867c-120">EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="f867c-120">EmptyFolder</span></span>](emptyfolder.md)
    
- [<span data-ttu-id="f867c-121">FolderIds</span><span class="sxs-lookup"><span data-stu-id="f867c-121">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="f867c-122">FolderId</span><span class="sxs-lookup"><span data-stu-id="f867c-122">FolderId</span></span>](folderid.md)
    
## <a name="successful-emptyfolder-response"></a><span data-ttu-id="f867c-123">Réponse EmptyFolder réussie</span><span class="sxs-lookup"><span data-stu-id="f867c-123">Successful EmptyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="f867c-124">Description</span><span class="sxs-lookup"><span data-stu-id="f867c-124">Description</span></span>

<span data-ttu-id="f867c-125">L’exemple suivant montre une réponse réussie à la demande **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="f867c-125">The following example shows a successful response to the **EmptyFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f867c-126">Code</span><span class="sxs-lookup"><span data-stu-id="f867c-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:EmptyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:EmptyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:EmptyFolderResponseMessage>
      </m:ResponseMessages>
    </m:EmptyFolderResponse>
  </s:Body>
</s:Envelope>

```

### <a name="successful-response-elements"></a><span data-ttu-id="f867c-127">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="f867c-127">Successful response elements</span></span>

<span data-ttu-id="f867c-128">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="f867c-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f867c-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f867c-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f867c-130">EmptyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f867c-130">EmptyFolderResponse</span></span>](emptyfolderresponse.md)
    
- [<span data-ttu-id="f867c-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f867c-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f867c-132">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f867c-132">EmptyFolderResponseMessage</span></span>](emptyfolderresponsemessage.md)
    
- [<span data-ttu-id="f867c-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f867c-133">ResponseCode</span></span>](responsecode.md)
    
## <a name="emptyfolder-error-response"></a><span data-ttu-id="f867c-134">Réponse d’erreur EmptyFolder</span><span class="sxs-lookup"><span data-stu-id="f867c-134">EmptyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="f867c-135">Description</span><span class="sxs-lookup"><span data-stu-id="f867c-135">Description</span></span>

<span data-ttu-id="f867c-136">L’exemple suivant montre une réponse d’erreur à une demande **EmptyFolder** .</span><span class="sxs-lookup"><span data-stu-id="f867c-136">The following example shows an error response to an **Emptyfolder** request.</span></span> <span data-ttu-id="f867c-137">L’erreur a été créée car l’opération a essayé de vider un dossier qui n’a pas été trouvé dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="f867c-137">The error was created because the operation tried to empty a folder that was not found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f867c-138">Code</span><span class="sxs-lookup"><span data-stu-id="f867c-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
            MinorVersion="1" 
            MajorBuildNumber="164" 
            MinorBuildNumber="0" 
            Version="Exchange2010_SP1" 
            xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse 
          xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="error-response-elements"></a><span data-ttu-id="f867c-139">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="f867c-139">Error response elements</span></span>

<span data-ttu-id="f867c-140">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="f867c-140">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f867c-141">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f867c-141">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f867c-142">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="f867c-142">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="f867c-143">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f867c-143">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f867c-144">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f867c-144">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="f867c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f867c-145">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f867c-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f867c-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f867c-147">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f867c-147">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="f867c-148">Dossiers</span><span class="sxs-lookup"><span data-stu-id="f867c-148">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="f867c-149">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f867c-149">See also</span></span>

- [<span data-ttu-id="f867c-150">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f867c-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

