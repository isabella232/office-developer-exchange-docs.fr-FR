---
title: CopyFolder, opération
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolder
api_type:
- schema
ms.assetid: c7ea0d68-9793-4144-b378-d99536776db9
description: L’opération CopyFolder copie les dossiers d’une boîte aux lettres.
ms.openlocfilehash: 1f9a7a3f3ede2d3cf8f9d41677d8ce0487266f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468893"
---
# <a name="copyfolder-operation"></a><span data-ttu-id="093e8-103">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="093e8-103">CopyFolder operation</span></span>

<span data-ttu-id="093e8-104">L’opération CopyFolder copie les dossiers d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="093e8-104">The CopyFolder operation copies folders in a mailbox.</span></span>
  
## <a name="using-the-copyfolder-operation"></a><span data-ttu-id="093e8-105">Utilisation de l’opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="093e8-105">Using the CopyFolder operation</span></span>

<span data-ttu-id="093e8-106">L’opération CopyFolder est semblable à l' [opération MoveFolder](movefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="093e8-106">The CopyFolder operation is similar to the [MoveFolder operation](movefolder-operation.md).</span></span> <span data-ttu-id="093e8-107">Il copie les dossiers identifiés et renvoie l' **ID** et **ChangeKey** des dossiers copiés.</span><span class="sxs-lookup"><span data-stu-id="093e8-107">It copies identified folders and returns the **Id** and **ChangeKey** of the copied folders.</span></span> 
  
## <a name="copyfolder-request-example"></a><span data-ttu-id="093e8-108">Exemple de requête CopyFolder</span><span class="sxs-lookup"><span data-stu-id="093e8-108">CopyFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="093e8-109">Description</span><span class="sxs-lookup"><span data-stu-id="093e8-109">Description</span></span>

<span data-ttu-id="093e8-110">L’exemple de requête CopyFolder suivant montre comment copier des dossiers dans le dossier boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="093e8-110">The following example of a CopyFolder request shows how to copy folders into the Inbox folder.</span></span>
  
> [!NOTE]
> <span data-ttu-id="093e8-111">La valeur de l’attribut **ID** de l’élément [FolderId](folderid.md) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="093e8-111">The value of the **Id** attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="093e8-112">Code</span><span class="sxs-lookup"><span data-stu-id="093e8-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AS4A=" ChangeKey="fsVU4=="/>
        <t:FolderId Id="AS4AU=" ChangeKey="fsVU4o=="/>
      </FolderIds>
    </CopyFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="093e8-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="093e8-113">Comments</span></span>

<span data-ttu-id="093e8-114">Les dossiers peuvent être identifiés par l’élément [DistinguishedFolderId](distinguishedfolderid.md) ou l’élément [FolderId](folderid.md) pour une utilisation dans les éléments [ToFolderId](tofolderid.md) ou [FolderIds](folderids.md) .</span><span class="sxs-lookup"><span data-stu-id="093e8-114">Folders can be identified by either the [DistinguishedFolderId](distinguishedfolderid.md) element or the [FolderId](folderid.md) element for use in either the [ToFolderId](tofolderid.md) or the [FolderIds](folderids.md) elements.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="093e8-115">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="093e8-115">Request elements</span></span>

<span data-ttu-id="093e8-116">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="093e8-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="093e8-117">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="093e8-117">CopyFolder</span></span>](copyfolder.md)
    
- [<span data-ttu-id="093e8-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="093e8-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="093e8-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="093e8-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="093e8-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="093e8-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="093e8-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="093e8-121">FolderId</span></span>](folderid.md)
    
> [!NOTE]
> <span data-ttu-id="093e8-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="093e8-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="093e8-123">Pour rechercher d’autres options pour le message de demande de l’opération CopyFolder, explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="093e8-123">To find other options for the request message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="093e8-124">Commencez par l’élément [CopyFolder](copyfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="093e8-124">Start at the [CopyFolder](copyfolder.md) element.</span></span> 
  
## <a name="successful-copyfolder-response"></a><span data-ttu-id="093e8-125">Réponse CopyFolder réussie</span><span class="sxs-lookup"><span data-stu-id="093e8-125">Successful CopyFolder response</span></span>

### <a name="description"></a><span data-ttu-id="093e8-126">Description</span><span class="sxs-lookup"><span data-stu-id="093e8-126">Description</span></span>

<span data-ttu-id="093e8-127">L’exemple suivant montre une réponse réussie à la demande CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="093e8-127">The following example shows a successful response to the CopyFolder request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="093e8-128">L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="093e8-128">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="093e8-129">Code</span><span class="sxs-lookup"><span data-stu-id="093e8-129">Code</span></span>

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
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn=" ChangeKey="fsVU4o==" />
            </t:Folder>
          </m:Folders>
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="093e8-130">Commentaire</span><span class="sxs-lookup"><span data-stu-id="093e8-130">Comment</span></span>

<span data-ttu-id="093e8-131">L’élément [FolderId](folderid.md) renvoyé dans la réponse représente le dossier qui a été copié dans le nouvel emplacement de dossier.</span><span class="sxs-lookup"><span data-stu-id="093e8-131">The [FolderId](folderid.md) element that is returned in the response represents the folder that was copied in the new folder location.</span></span> 
  
### <a name="response-elements"></a><span data-ttu-id="093e8-132">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="093e8-132">Response elements</span></span>

<span data-ttu-id="093e8-133">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="093e8-133">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="093e8-134">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="093e8-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="093e8-135">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="093e8-135">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="093e8-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="093e8-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="093e8-137">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="093e8-137">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="093e8-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="093e8-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="093e8-139">Dossiers</span><span class="sxs-lookup"><span data-stu-id="093e8-139">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="093e8-140">Folder</span><span class="sxs-lookup"><span data-stu-id="093e8-140">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="093e8-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="093e8-141">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="093e8-142">Pour rechercher d’autres options pour le message de réponse de l’opération CopyFolder, explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="093e8-142">To find other options for the response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="093e8-143">Commencez par l’élément [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="093e8-143">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="copyfolder-error-response"></a><span data-ttu-id="093e8-144">Réponse d’erreur CopyFolder</span><span class="sxs-lookup"><span data-stu-id="093e8-144">CopyFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="093e8-145">Description</span><span class="sxs-lookup"><span data-stu-id="093e8-145">Description</span></span>

<span data-ttu-id="093e8-146">L’exemple suivant montre une réponse d’erreur à une demande CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="093e8-146">The following example shows an error response to a CopyFolder request.</span></span> <span data-ttu-id="093e8-147">L’erreur s’est produite car un dossier portant le même nom d’affichage existe déjà.</span><span class="sxs-lookup"><span data-stu-id="093e8-147">The error occurred because a folder with the same display name already exists.</span></span>
  
### <a name="code"></a><span data-ttu-id="093e8-148">Code</span><span class="sxs-lookup"><span data-stu-id="093e8-148">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyFolderResponseMessage ResponseClass="Error">
          <m:MessageText>The move or copy operation failed.</m:MessageText>
          <m:ResponseCode>ErrorMoveCopyFailed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CopyFolderResponseMessage>
      </m:ResponseMessages>
    </CopyFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="093e8-149">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="093e8-149">Error response elements</span></span>

<span data-ttu-id="093e8-150">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="093e8-150">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="093e8-151">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="093e8-151">CopyFolderResponse</span></span>](copyfolderresponse.md)
    
- [<span data-ttu-id="093e8-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="093e8-152">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="093e8-153">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="093e8-153">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
    
- [<span data-ttu-id="093e8-154">MessageText</span><span class="sxs-lookup"><span data-stu-id="093e8-154">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="093e8-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="093e8-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="093e8-156">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="093e8-156">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="093e8-157">Dossiers</span><span class="sxs-lookup"><span data-stu-id="093e8-157">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="093e8-158">Pour rechercher d’autres options pour le message d’erreur de l’opération CopyFolder, explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="093e8-158">To find other options for the error response message of the CopyFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="093e8-159">Commencez par l’élément [CopyFolderResponse](copyfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="093e8-159">Start at the [CopyFolderResponse](copyfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="093e8-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="093e8-160">See also</span></span>

- [<span data-ttu-id="093e8-161">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="093e8-161">MoveFolder operation</span></span>](movefolder-operation.md)
- [<span data-ttu-id="093e8-162">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="093e8-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

