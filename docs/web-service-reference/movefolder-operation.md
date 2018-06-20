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
ms.openlocfilehash: 5da6929f11ce9ba74db190db6d799f25974d2192
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828490"
---
# <a name="movefolder-operation"></a><span data-ttu-id="8d6d1-103">Opération MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-103">MoveFolder operation</span></span>

<span data-ttu-id="8d6d1-104">L’opération MoveFolder déplace les dossiers d’un dossier spécifié et les place dans un autre dossier.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-104">The MoveFolder operation moves folders from a specified folder and puts them in another folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d6d1-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="8d6d1-105">Remarks</span></span>

<span data-ttu-id="8d6d1-106">L’opération MoveFolder est similaire à l’opération CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-106">The MoveFolder operation is similar to the CopyFolder operation.</span></span> <span data-ttu-id="8d6d1-107">Impossible de déplacer des dossiers uniques.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-107">You cannot move distinguished folders.</span></span> <span data-ttu-id="8d6d1-108">Vous pouvez déplacer plusieurs dossiers à la fois dans le dossier de destination.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-108">You can move multiple folders at one time to the destination folder.</span></span>
  
## <a name="movefolder-request-example"></a><span data-ttu-id="8d6d1-109">Exemple de requête MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-109">MoveFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="8d6d1-110">Description</span><span class="sxs-lookup"><span data-stu-id="8d6d1-110">Description</span></span>

<span data-ttu-id="8d6d1-111">L’exemple suivant d’une demande MoveFolder indique comment former une demande pour déplacer un dossier identifié par l' [ID FolderId](folderid.md) et placez le dossier dans le dossier de courrier indésirable unique.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-111">The following example of a MoveFolder request shows how to form a request to move a folder identified by the [FolderId](folderid.md) and put the folder in the Junk E-mail distinguished folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8d6d1-112">Code</span><span class="sxs-lookup"><span data-stu-id="8d6d1-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="8d6d1-113">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8d6d1-113">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="8d6d1-114">La valeur de l’attribut ID de l’élément [FolderId](folderid.md) a été raccourcie pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-114">The value of the ID attribute of the [FolderId](folderid.md) element has been shortened for readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="8d6d1-115">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="8d6d1-115">Request elements</span></span>

<span data-ttu-id="8d6d1-116">Cette demande MoveFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8d6d1-116">This MoveFolder request includes the following elements:</span></span>
  
- [<span data-ttu-id="8d6d1-117">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-117">MoveFolder</span></span>](movefolder.md)
    
- [<span data-ttu-id="8d6d1-118">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="8d6d1-118">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="8d6d1-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="8d6d1-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="8d6d1-120">FolderIds</span><span class="sxs-lookup"><span data-stu-id="8d6d1-120">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="8d6d1-121">FolderId</span><span class="sxs-lookup"><span data-stu-id="8d6d1-121">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="8d6d1-122">Voir le schéma pour les éléments supplémentaires que vous pouvez utiliser pour créer une demande MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-122">See the schema for additional elements that you can use to form a MoveFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8d6d1-123">L’emplacement par défaut du schéma est dans le répertoire virtuel EWS sur l’ordinateur sur lequel le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-123">The default location of the schema is in the EWS virtual directory on the computer that has the Client Access server role installed.</span></span> 
  
## <a name="successful-movefolder-response-example"></a><span data-ttu-id="8d6d1-124">Exemple de réponse MoveFolder réussie</span><span class="sxs-lookup"><span data-stu-id="8d6d1-124">Successful MoveFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="8d6d1-125">Description</span><span class="sxs-lookup"><span data-stu-id="8d6d1-125">Description</span></span>

<span data-ttu-id="8d6d1-126">L’exemple suivant montre une réponse positive à la demande MoveFolder.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-126">The following example shows a successful response to the MoveFolder request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8d6d1-127">Code</span><span class="sxs-lookup"><span data-stu-id="8d6d1-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="8d6d1-128">Commentaires</span><span class="sxs-lookup"><span data-stu-id="8d6d1-128">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="8d6d1-129">L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-129">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="8d6d1-130">L’ID FolderId qui est renvoyé dans la réponse représente le dossier qui a été déplacé vers le nouveau l’emplacement du dossier.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-130">The FolderId that is returned in the response represents the folder that was moved to the new the folder location.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="8d6d1-131">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="8d6d1-131">Response elements</span></span>

<span data-ttu-id="8d6d1-132">La réponse MoveFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8d6d1-132">The MoveFolder response includes the following elements:</span></span>
  
- [<span data-ttu-id="8d6d1-133">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8d6d1-133">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="8d6d1-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8d6d1-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8d6d1-135">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8d6d1-135">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="8d6d1-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8d6d1-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8d6d1-137">Dossiers</span><span class="sxs-lookup"><span data-stu-id="8d6d1-137">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="8d6d1-138">Folder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-138">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="8d6d1-139">FolderId</span><span class="sxs-lookup"><span data-stu-id="8d6d1-139">FolderId</span></span>](folderid.md)
    
## <a name="movefolder-error-response-example"></a><span data-ttu-id="8d6d1-140">Exemple de réponse d’erreur MoveFolder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-140">MoveFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="8d6d1-141">Description</span><span class="sxs-lookup"><span data-stu-id="8d6d1-141">Description</span></span>

<span data-ttu-id="8d6d1-142">L’exemple suivant montre une réponse d’erreur qui se produit lorsque vous tentez de déplacer un dossier unique.</span><span class="sxs-lookup"><span data-stu-id="8d6d1-142">The following example shows an error response that occurs when you try to move a distinguished folder.</span></span>
  
### <a name="code"></a><span data-ttu-id="8d6d1-143">Code</span><span class="sxs-lookup"><span data-stu-id="8d6d1-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <MoveFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="8d6d1-144">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="8d6d1-144">Error response elements</span></span>

<span data-ttu-id="8d6d1-145">La réponse d’erreur MoveFolder comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="8d6d1-145">The MoveFolder error response includes the following elements:</span></span>
  
- [<span data-ttu-id="8d6d1-146">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8d6d1-146">MoveFolderResponse</span></span>](movefolderresponse.md)
    
- [<span data-ttu-id="8d6d1-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8d6d1-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="8d6d1-148">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8d6d1-148">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
    
- [<span data-ttu-id="8d6d1-149">MessageText</span><span class="sxs-lookup"><span data-stu-id="8d6d1-149">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="8d6d1-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8d6d1-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="8d6d1-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8d6d1-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="8d6d1-152">Dossiers</span><span class="sxs-lookup"><span data-stu-id="8d6d1-152">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="8d6d1-153">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="8d6d1-153">See also</span></span>



[<span data-ttu-id="8d6d1-154">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="8d6d1-154">CopyFolder operation</span></span>](copyfolder-operation.md)

