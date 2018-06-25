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
ms.openlocfilehash: 0fd7c9d4b04a706dcdb83f41087eaa4f3d45f129
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755859"
---
# <a name="deletefolder-operation"></a><span data-ttu-id="e0fb7-103">Opération DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e0fb7-103">DeleteFolder operation</span></span>

<span data-ttu-id="e0fb7-104">L’opération **DeleteFolder** supprime les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-104">The **DeleteFolder** operation deletes folders from a mailbox.</span></span> 
  
## <a name="deletefolder-request-example"></a><span data-ttu-id="e0fb7-105">Exemple de requête DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e0fb7-105">DeleteFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="e0fb7-106">Description</span><span class="sxs-lookup"><span data-stu-id="e0fb7-106">Description</span></span>

<span data-ttu-id="e0fb7-107">L’exemple suivant d’une demande **DeleteFolder** indique comment former une demande pour supprimer un dossier.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-107">This following example of a **DeleteFolder** request shows how to form a request to delete a folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e0fb7-108">Code</span><span class="sxs-lookup"><span data-stu-id="e0fb7-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                  DeleteType="HardDelete" >
      <FolderIds>
        <t:FolderId Id="AS4AUnVz=" />
      </FolderIds>
    </DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="e0fb7-109">Commentaires</span><span class="sxs-lookup"><span data-stu-id="e0fb7-109">Comments</span></span>

<span data-ttu-id="e0fb7-110">Cet exemple effectue une suppression définitive sur le dossier.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-110">This example performs a hard delete on the folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e0fb7-111">L’ID du dossier a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-111">The folder ID has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="e0fb7-112">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="e0fb7-112">Request elements</span></span>

<span data-ttu-id="e0fb7-113">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="e0fb7-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="e0fb7-114">DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e0fb7-114">DeleteFolder</span></span>](deletefolder.md)
    
- [<span data-ttu-id="e0fb7-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e0fb7-115">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="e0fb7-116">FolderId</span><span class="sxs-lookup"><span data-stu-id="e0fb7-116">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="e0fb7-117">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-117">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="e0fb7-118">Pour trouver d’autres options pour le message de demande de l’opération **DeleteFolder** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-118">To find other options for the request message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e0fb7-119">Commencer à l’élément [DeleteFolder](deletefolder.md) .</span><span class="sxs-lookup"><span data-stu-id="e0fb7-119">Start at the [DeleteFolder](deletefolder.md) element.</span></span> 
  
## <a name="successful-deletefolder-response"></a><span data-ttu-id="e0fb7-120">Réponse DeleteFolder réussie</span><span class="sxs-lookup"><span data-stu-id="e0fb7-120">Successful DeleteFolder response</span></span>

### <a name="description"></a><span data-ttu-id="e0fb7-121">Description</span><span class="sxs-lookup"><span data-stu-id="e0fb7-121">Description</span></span>

<span data-ttu-id="e0fb7-122">L’exemple suivant montre une réponse positive à la demande **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="e0fb7-122">The following example shows a successful response to the **DeleteFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e0fb7-123">Code</span><span class="sxs-lookup"><span data-stu-id="e0fb7-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteFolderResponseMessage>
      </m:ResponseMessages>
    </DeleteFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="e0fb7-124">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="e0fb7-124">Response elements</span></span>

<span data-ttu-id="e0fb7-125">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="e0fb7-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="e0fb7-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e0fb7-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e0fb7-127">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="e0fb7-127">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="e0fb7-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0fb7-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0fb7-129">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0fb7-129">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="e0fb7-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0fb7-130">ResponseCode</span></span>](responsecode.md)
    
<span data-ttu-id="e0fb7-131">Pour trouver d’autres options pour le message de réponse de l’opération **DeleteFolder** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-131">To find other options for the response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e0fb7-132">Démarrez au niveau de l’élément [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e0fb7-132">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="deletefolder-error-response"></a><span data-ttu-id="e0fb7-133">Réponse d’erreur DeleteFolder</span><span class="sxs-lookup"><span data-stu-id="e0fb7-133">DeleteFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="e0fb7-134">Description</span><span class="sxs-lookup"><span data-stu-id="e0fb7-134">Description</span></span>

<span data-ttu-id="e0fb7-135">L’exemple suivant montre une réponse d’erreur à une demande **DeleteFolder** .</span><span class="sxs-lookup"><span data-stu-id="e0fb7-135">The following example shows an error response to a **DeleteFolder** request.</span></span> <span data-ttu-id="e0fb7-136">L’erreur a été provoquée par une demande pour supprimer un dossier qui n’était pas présent dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-136">The error was caused by a request to delete a folder that was not present in the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="e0fb7-137">Code</span><span class="sxs-lookup"><span data-stu-id="e0fb7-137">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <DeleteFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="e0fb7-138">Commentaires</span><span class="sxs-lookup"><span data-stu-id="e0fb7-138">Comments</span></span>

<span data-ttu-id="e0fb7-139">L’opération **DeleteFolder** ne peut pas être utilisée dans les dossiers uniques.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-139">The **DeleteFolder** operation cannot be used on distinguished folders.</span></span> 
  
### <a name="error-response-elements"></a><span data-ttu-id="e0fb7-140">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="e0fb7-140">Error response elements</span></span>

<span data-ttu-id="e0fb7-141">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="e0fb7-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="e0fb7-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e0fb7-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="e0fb7-143">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="e0fb7-143">DeleteFolderResponse</span></span>](deletefolderresponse.md)
    
- [<span data-ttu-id="e0fb7-144">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0fb7-144">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0fb7-145">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0fb7-145">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
    
- [<span data-ttu-id="e0fb7-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="e0fb7-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e0fb7-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0fb7-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e0fb7-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e0fb7-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="e0fb7-149">Pour trouver d’autres options pour le message de réponse de l’opération **DeleteFolder** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="e0fb7-149">To find other options for the error response message of the **DeleteFolder** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="e0fb7-150">Démarrez au niveau de l’élément [DeleteFolderResponse](deletefolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="e0fb7-150">Start at the [DeleteFolderResponse](deletefolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e0fb7-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e0fb7-151">See also</span></span>

- [<span data-ttu-id="e0fb7-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e0fb7-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="e0fb7-153">Suppression des dossiers</span><span class="sxs-lookup"><span data-stu-id="e0fb7-153">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

