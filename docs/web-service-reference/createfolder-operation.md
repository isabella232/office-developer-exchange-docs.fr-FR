---
title: CreateFolder Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateFolder
api_type:
- schema
ms.assetid: 6f6c334c-b190-4e55-8f0a-38f2a018d1b3
description: L’opération CreateFolder crée des dossiers, des dossiers de calendrier, les dossiers contacts, tâches de dossiers et recherche les dossiers.
ms.openlocfilehash: 97156d4a3747cacbdcf9563d21d93a0aa44c3358
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755700"
---
# <a name="createfolder-operation"></a><span data-ttu-id="eabd1-103">CreateFolder Operation</span><span class="sxs-lookup"><span data-stu-id="eabd1-103">CreateFolder operation</span></span>

<span data-ttu-id="eabd1-104">L’opération CreateFolder crée des dossiers, des dossiers de calendrier, les dossiers contacts, tâches de dossiers et recherche les dossiers.</span><span class="sxs-lookup"><span data-stu-id="eabd1-104">The CreateFolder operation creates folders, calendar folders, contacts folders, tasks folders, and search folders.</span></span>
  
## <a name="createfolder-request-example"></a><span data-ttu-id="eabd1-105">Exemple de requête CreateFolder</span><span class="sxs-lookup"><span data-stu-id="eabd1-105">CreateFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="eabd1-106">Description</span><span class="sxs-lookup"><span data-stu-id="eabd1-106">Description</span></span>

<span data-ttu-id="eabd1-107">L’exemple suivant d’une demande CreateFolder montre comment former une demande pour créer deux nouveaux dossiers dans la racine de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="eabd1-107">The following example of a CreateFolder request shows how to form a request to create two new folders in the mailbox root.</span></span>
  
### <a name="code"></a><span data-ttu-id="eabd1-108">Code</span><span class="sxs-lookup"><span data-stu-id="eabd1-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ParentFolderId>
        <t:DistinguishedFolderId Id="msgfolderroot"/>
      </ParentFolderId>
      <Folders>
        <t:Folder>
          <t:DisplayName>Folder1</t:DisplayName>
        </t:Folder>
        <t:Folder>
          <t:DisplayName>Folder2</t:DisplayName>
        </t:Folder>
      </Folders>
    </CreateFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="eabd1-109">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="eabd1-109">Request elements</span></span>

<span data-ttu-id="eabd1-110">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="eabd1-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="eabd1-111">CreateFolder</span><span class="sxs-lookup"><span data-stu-id="eabd1-111">CreateFolder</span></span>](createfolder.md)
    
- [<span data-ttu-id="eabd1-112">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="eabd1-112">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="eabd1-113">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="eabd1-113">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="eabd1-114">Dossiers</span><span class="sxs-lookup"><span data-stu-id="eabd1-114">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="eabd1-115">Folder</span><span class="sxs-lookup"><span data-stu-id="eabd1-115">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="eabd1-116">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="eabd1-116">DisplayName (string)</span></span>](displayname-string.md)
    
> [!NOTE]
> <span data-ttu-id="eabd1-117">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="eabd1-117">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="eabd1-118">Pour trouver d’autres options pour le message de demande de l’opération CreateFolder, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="eabd1-118">To find other options for the request message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eabd1-119">Commencer à l’élément [CreateFolder](createfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="eabd1-119">Start at the [CreateFolder](createfolder.md) element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="eabd1-120">Si vous créez un dossier de recherche avec une restriction à l’aide de la propriété **Calendrier : organisateur** , un appel de dossier suivantes get retournera la restriction avec la **message : à partir de** propriété à la place.</span><span class="sxs-lookup"><span data-stu-id="eabd1-120">If you create a search folder with a restriction by using the **calendar:Organizer** property, a subsequent get folder call will return the restriction with the **message:from** property in its place.</span></span> <span data-ttu-id="eabd1-121">Ces deux propriétés mappent à la même propriété MAPI sous-jacent.</span><span class="sxs-lookup"><span data-stu-id="eabd1-121">These two properties map to the same underlying MAPI property.</span></span> 
  
<span data-ttu-id="eabd1-122">L’opération CreateFolder prend en charge la création d’une classe de dossier personnalisé uniquement lorsque vous créez le dossier à l’aide d’un élément de type dossier générique et définissez l’élément de la **classe FolderClass** .</span><span class="sxs-lookup"><span data-stu-id="eabd1-122">The CreateFolder operation supports the creation of a custom folder class only when you create the folder by using a generic folder type element and set the **FolderClass** element.</span></span> 
  
## <a name="successful-createfolder-response-example"></a><span data-ttu-id="eabd1-123">Exemple de réponse CreateFolder réussie</span><span class="sxs-lookup"><span data-stu-id="eabd1-123">Successful CreateFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="eabd1-124">Description</span><span class="sxs-lookup"><span data-stu-id="eabd1-124">Description</span></span>

<span data-ttu-id="eabd1-125">L’exemple suivant montre une réponse positive à la demande CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="eabd1-125">The following example shows a successful response to the CreateFolder request.</span></span> <span data-ttu-id="eabd1-126">Dans cet exemple, la réponse renvoie les identificateurs des nouveaux dossiers.</span><span class="sxs-lookup"><span data-stu-id="eabd1-126">In this example, the response returns the identifiers of the new folders.</span></span>
  
> [!NOTE]
> <span data-ttu-id="eabd1-127">L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="eabd1-127">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="eabd1-128">Code</span><span class="sxs-lookup"><span data-stu-id="eabd1-128">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
        <m:CreateFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS4AUn==" />
            </t:Folder>
          </m:Folders>
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="eabd1-129">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="eabd1-129">Successful response elements</span></span>

<span data-ttu-id="eabd1-130">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="eabd1-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="eabd1-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eabd1-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eabd1-132">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="eabd1-132">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="eabd1-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eabd1-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eabd1-134">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eabd1-134">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="eabd1-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eabd1-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eabd1-136">Dossiers</span><span class="sxs-lookup"><span data-stu-id="eabd1-136">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="eabd1-137">Folder</span><span class="sxs-lookup"><span data-stu-id="eabd1-137">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="eabd1-138">FolderId</span><span class="sxs-lookup"><span data-stu-id="eabd1-138">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="eabd1-139">Pour trouver d’autres options pour le message de réponse de l’opération CreateFolder, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="eabd1-139">To find other options for the response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eabd1-140">Démarrez au niveau de l’élément [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="eabd1-140">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="createfolder-error-response"></a><span data-ttu-id="eabd1-141">Réponse d’erreur CreateFolder</span><span class="sxs-lookup"><span data-stu-id="eabd1-141">CreateFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="eabd1-142">Description</span><span class="sxs-lookup"><span data-stu-id="eabd1-142">Description</span></span>

<span data-ttu-id="eabd1-143">L’exemple suivant montre une réponse d’erreur à une demande de CreateFolder.</span><span class="sxs-lookup"><span data-stu-id="eabd1-143">The following example shows an error response to a CreateFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="eabd1-144">Code</span><span class="sxs-lookup"><span data-stu-id="eabd1-144">Code</span></span>

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
    <CreateFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A folder with the specified name already exists.</m:MessageText>
          <m:ResponseCode>ErrorFolderExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:CreateFolderResponseMessage>
      </m:ResponseMessages>
    </CreateFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="eabd1-145">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="eabd1-145">Error response elements</span></span>

<span data-ttu-id="eabd1-146">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="eabd1-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="eabd1-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eabd1-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eabd1-148">CreateFolderResponse</span><span class="sxs-lookup"><span data-stu-id="eabd1-148">CreateFolderResponse</span></span>](createfolderresponse.md)
    
- [<span data-ttu-id="eabd1-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eabd1-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="eabd1-150">CreateFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eabd1-150">CreateFolderResponseMessage</span></span>](createfolderresponsemessage.md)
    
- [<span data-ttu-id="eabd1-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="eabd1-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="eabd1-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eabd1-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eabd1-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="eabd1-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="eabd1-154">Dossiers</span><span class="sxs-lookup"><span data-stu-id="eabd1-154">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="eabd1-155">Pour trouver d’autres options pour le message de réponse de l’opération CreateFolder, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="eabd1-155">To find other options for the error response message of the CreateFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="eabd1-156">Démarrez au niveau de l’élément [CreateFolderResponse](createfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="eabd1-156">Start at the [CreateFolderResponse](createfolderresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="eabd1-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eabd1-157">See also</span></span>



[<span data-ttu-id="eabd1-158">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="eabd1-158">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="eabd1-159">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="eabd1-159">FindFolder operation</span></span>](findfolder-operation.md)
  
 <span data-ttu-id="eabd1-160">**CreateFolderType**</span><span class="sxs-lookup"><span data-stu-id="eabd1-160">**CreateFolderType**</span></span>


- [<span data-ttu-id="eabd1-161">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="eabd1-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="eabd1-162">Création de dossiers (Exchange Web Services)</span><span class="sxs-lookup"><span data-stu-id="eabd1-162">Creating Folders (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

