---
title: Opération DeleteFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolder
api_type:
- schema
ms.assetid: b0f92682-4895-4bcf-a4a1-e4c2e8403979
description: L’opération DeleteFolder supprime les dossiers d’une boîte aux lettres.
ms.openlocfilehash: e9bb9199027c2af2cbbb664ef7ad4fa70b7ef718
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455743"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="59e97-103">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="59e97-103">DeleteFolder operation</span></span>

<span data-ttu-id="59e97-104">L’opération **DeleteFolder** supprime les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="59e97-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="59e97-105">Exemple de requête DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="59e97-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="59e97-106">Description</span><span class="sxs-lookup"><span data-stu-id="59e97-106">Description</span></span>

<span data-ttu-id="59e97-107">L’exemple de requête **DeleteFolder** suivant montre comment créer une demande de suppression d’un dossier.</span><span class="sxs-lookup"><span data-stu-id="59e97-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="59e97-108">Code</span><span class="sxs-lookup"><span data-stu-id="59e97-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="59e97-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="59e97-109">Comments</span></span>

<span data-ttu-id="59e97-110">Cet exemple effectue une suppression définitive sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="59e97-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="59e97-111">L’ID de dossier a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="59e97-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="59e97-112">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="59e97-112">Request elements</span></span>

<span data-ttu-id="59e97-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="59e97-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="59e97-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="59e97-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="59e97-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="59e97-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="59e97-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="59e97-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="59e97-117">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="59e97-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="59e97-118">Pour trouver d’autres options pour le message de demande de l’opération **DeleteFolder** , explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="59e97-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="59e97-119">Commencez par l’élément [DeleteFolder](deletefolder.md) .</span><span class="sxs-lookup"><span data-stu-id="59e97-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="59e97-120">Réponse DeleteFolder réussie</span><span class="sxs-lookup"><span data-stu-id="59e97-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="59e97-121">Description</span><span class="sxs-lookup"><span data-stu-id="59e97-121">Description</span></span>

<span data-ttu-id="59e97-122">L’exemple suivant montre une réponse réussie à la demande **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="59e97-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="59e97-123">Code</span><span class="sxs-lookup"><span data-stu-id="59e97-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="59e97-124">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="59e97-124">Response elements</span></span>

<span data-ttu-id="59e97-125">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="59e97-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="59e97-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="59e97-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="59e97-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="59e97-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="59e97-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="59e97-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="59e97-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="59e97-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="59e97-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="59e97-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="59e97-131">Pour trouver d’autres options pour le message de réponse de l’opération **DeleteFolder** , explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="59e97-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="59e97-132">Commencez par l’élément [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="59e97-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="59e97-133">Réponse d’erreur DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="59e97-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="59e97-134">Description</span><span class="sxs-lookup"><span data-stu-id="59e97-134">Description</span></span>

<span data-ttu-id="59e97-135">L’exemple suivant montre une réponse d’erreur à une requête **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="59e97-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="59e97-136">L’erreur a été causée par une demande de suppression d’un dossier qui n’était pas présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="59e97-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="59e97-137">Code</span><span class="sxs-lookup"><span data-stu-id="59e97-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="59e97-138">Commentaires</span><span class="sxs-lookup"><span data-stu-id="59e97-138">Comments</span></span>

<span data-ttu-id="59e97-139">L’opération **DeleteFolder** ne peut pas être utilisée sur des dossiers uniques.</span><span class="sxs-lookup"><span data-stu-id="59e97-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="59e97-140">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="59e97-140">Error response elements</span></span>

<span data-ttu-id="59e97-141">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="59e97-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="59e97-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="59e97-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="59e97-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="59e97-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="59e97-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="59e97-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="59e97-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="59e97-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="59e97-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="59e97-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="59e97-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="59e97-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="59e97-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="59e97-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="59e97-149">Pour rechercher d’autres options pour le message d’erreur de réponse de l’opération **DeleteFolder** , explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="59e97-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="59e97-150">Commencez par l’élément [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="59e97-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="59e97-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59e97-151">See also</span></span>

- [<span data-ttu-id="59e97-152">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59e97-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="59e97-153">Suppression de dossiers</span><span class="sxs-lookup"><span data-stu-id="59e97-153">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

