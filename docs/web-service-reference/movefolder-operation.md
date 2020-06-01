---
title: Opération MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: c7233966-6c87-4a14-8156-b1610760176d
description: L’opération MoveFolder déplace les dossiers d’un dossier spécifié et les place dans un autre dossier.
ms.openlocfilehash: dc572130ca3b2f2b152abbb4a8b68cc6f67790e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460581"
---
# <a name="movefolder-operation"></a><span data-ttu-id="ec667-103">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ec667-103">MoveFolder operation</span></span>

<span data-ttu-id="ec667-104">L’opération MoveFolder déplace les dossiers d’un dossier spécifié et les place dans un autre dossier.</span><span class="sxs-lookup"><span data-stu-id="ec667-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec667-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec667-105">Remarks</span></span>

<span data-ttu-id="ec667-106">L’opération MoveFolder est similaire à l’opération CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="ec667-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="ec667-107">Vous ne pouvez pas déplacer des dossiers uniques.</span><span class="sxs-lookup"><span data-stu-id="ec667-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="ec667-108">Vous pouvez déplacer plusieurs dossiers à la fois vers le dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="ec667-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="ec667-109">Exemple de requête MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ec667-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ec667-110">Description</span><span class="sxs-lookup"><span data-stu-id="ec667-110">Description</span></span>

<span data-ttu-id="ec667-111">L’exemple de requête MoveFolder suivant montre comment créer une demande de déplacement d’un dossier identifié par le [FolderId](folderid.md) et placer le dossier dans le dossier unique du courrier indésirable.</span><span class="sxs-lookup"><span data-stu-id="ec667-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ec667-112">Code</span><span class="sxs-lookup"><span data-stu-id="ec667-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="junkemail"/>
      </ToFolderId>
      <FolderIds>
        <t:FolderId Id="AScAc"/>
      </FolderIds>
    </MoveFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ec667-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="ec667-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ec667-114">La valeur de l’attribut ID de l’élément [FolderId](folderid.md) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ec667-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ec667-115">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="ec667-115">Request elements</span></span>

<span data-ttu-id="ec667-116">Cette requête MoveFolder inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ec667-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="ec667-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ec667-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="ec667-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="ec667-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="ec667-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ec667-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ec667-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="ec667-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="ec667-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="ec667-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="ec667-122">Consultez le schéma pour les éléments supplémentaires que vous pouvez utiliser pour former une requête MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="ec667-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ec667-123">L’emplacement par défaut du schéma se trouve dans le répertoire virtuel EWS de l’ordinateur sur lequel le rôle serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ec667-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="ec667-124">Exemple de réponse MoveFolder réussi</span><span class="sxs-lookup"><span data-stu-id="ec667-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="ec667-125">Description</span><span class="sxs-lookup"><span data-stu-id="ec667-125">Description</span></span>

<span data-ttu-id="ec667-126">L’exemple suivant montre une réponse réussie à la demande MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="ec667-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ec667-127">Code</span><span class="sxs-lookup"><span data-stu-id="ec667-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AAAlAFV" ChangeKey="AQAAAB" />
            </t:Folder>
          </m:Folders>
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ec667-128">Commentaires</span><span class="sxs-lookup"><span data-stu-id="ec667-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ec667-129">L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ec667-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="ec667-130">Le FolderId renvoyé dans la réponse représente le dossier déplacé vers le nouvel emplacement du dossier.</span><span class="sxs-lookup"><span data-stu-id="ec667-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="ec667-131">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="ec667-131">Response elements</span></span>

<span data-ttu-id="ec667-132">La réponse MoveFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ec667-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="ec667-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ec667-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="ec667-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec667-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ec667-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec667-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="ec667-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ec667-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ec667-137">Dossiers</span><span class="sxs-lookup"><span data-stu-id="ec667-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ec667-138">Folder</span><span class="sxs-lookup"><span data-stu-id="ec667-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="ec667-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="ec667-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="ec667-140">Exemple de réponse d’erreur MoveFolder</span><span class="sxs-lookup"><span data-stu-id="ec667-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ec667-141">Description</span><span class="sxs-lookup"><span data-stu-id="ec667-141">Description</span></span>

<span data-ttu-id="ec667-142">L’exemple suivant montre une réponse d’erreur qui se produit lorsque vous essayez de déplacer un dossier unique.</span><span class="sxs-lookup"><span data-stu-id="ec667-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="ec667-143">Code</span><span class="sxs-lookup"><span data-stu-id="ec667-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot move distinguished folder.</m:MessageText>
          <m:ResponseCode>ErrorMoveDistinguishedFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:MoveFolderResponseMessage>
      </m:ResponseMessages>
    </MoveFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="ec667-144">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="ec667-144">Error response elements</span></span>

<span data-ttu-id="ec667-145">La réponse d’erreur MoveFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ec667-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="ec667-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ec667-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="ec667-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ec667-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ec667-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ec667-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="ec667-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="ec667-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ec667-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ec667-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ec667-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ec667-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ec667-152">Dossiers</span><span class="sxs-lookup"><span data-stu-id="ec667-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="ec667-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec667-153">See also</span></span>



[<span data-ttu-id="ec667-154">CopyFolder, opération</span><span class="sxs-lookup"><span data-stu-id="ec667-154">CopyFolder operation</span></span>](copyfolder-operation.md)

