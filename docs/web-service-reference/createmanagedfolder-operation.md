---
title: Opération CreateManagedFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateManagedFolder
api_type:
- schema
ms.assetid: 60a668a2-b4e9-4db9-ac76-9b181e47b302
description: L’opération CreateManagedFolder crée un dossier géré dans la banque d’informations Exchange.
ms.openlocfilehash: 2c2af53dc5dbe1e6fcbc7f3b1174a856e51e4905
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755735"
---
# <a name="createmanagedfolder-operation"></a><span data-ttu-id="0ebe9-103">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-103">CreateManagedFolder operation</span></span>

<span data-ttu-id="0ebe9-104">L’opération CreateManagedFolder crée un dossier géré dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-104">The CreateManagedFolder operation creates a managed folder in the Exchange store.</span></span>
  
## <a name="using-the-createmanagedfolder-operation"></a><span data-ttu-id="0ebe9-105">Utilisation de l’opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-105">Using the CreateManagedFolder Operation</span></span>

<span data-ttu-id="0ebe9-106">L’opération CreateManagedFolder ajoute un dossier personnalisé géré à la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-106">The CreateManagedFolder operation adds a managed custom folder to a user's mailbox.</span></span> <span data-ttu-id="0ebe9-107">Vous pouvez utiliser l’applet de commande Exchange Management Shell, **Get-ManagedFolder** pour rechercher les dossiers gérés disponibles à ajouter.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-107">You can use the Exchange Management Shell **Get-ManagedFolder** cmdlet to find available managed folders to add.</span></span> <span data-ttu-id="0ebe9-108">Bien que cette applet de commande renvoie les dossiers personnalisés gérés et les dossiers gérés par défaut uniquement gérés personnalisés dossiers peuvent être ajoutés.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-108">Although this cmdlet returns both managed custom folders and managed default folders, only managed custom folders can be added.</span></span> <span data-ttu-id="0ebe9-109">Dossiers personnalisés gérés sont identifiés par le type de dossier ManagedCustomFolder.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-109">Managed custom folders are identified by the ManagedCustomFolder folder type.</span></span> <span data-ttu-id="0ebe9-110">L’espace de noms System.DirectoryServices inclut également les types qui peuvent être utilisés pour découvrir les noms des dossiers gérés disponibles.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-110">The System.DirectoryServices namespace also includes types that can be used to discover the names of available managed folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0ebe9-111">Vous ne pouvez pas utiliser les Services Web Exchange pour rechercher les noms de dossiers gérés disponibles à ajouter à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-111">You cannot use Exchange Web Services to find the names of available managed folders to add to a mailbox.</span></span> 
  
<span data-ttu-id="0ebe9-112">Vous pouvez utiliser les opérations FindFolder et GetFolder pour accéder aux dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-112">You can use the FindFolder and GetFolder operations to access managed folders.</span></span> <span data-ttu-id="0ebe9-113">FindFolder est utilisé pour rechercher des dossiers dans un dossier parent spécifié.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-113">FindFolder is used to search for folders in a specified parent folder.</span></span> <span data-ttu-id="0ebe9-114">Cela peut être utilisé pour que les dossiers gérés peuvent être découverts dans un dossier avant la tentative d’ajout de qu'un dossier personnalisé dans le même répertoire géré par un double.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-114">This can be used so that managed folders can be discovered in a folder before trying to add a duplicate managed custom folder to the same directory.</span></span> <span data-ttu-id="0ebe9-115">GetFolder est utilisée après l’opération FindFolder pour obtenir plus d’informations sur un dossier personnalisé géré.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-115">GetFolder is used after the FindFolder operation to get more information about a managed custom folder.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ebe9-116">Remarques</span><span class="sxs-lookup"><span data-stu-id="0ebe9-116">Remarks</span></span>

<span data-ttu-id="0ebe9-117">Pour plus d’informations sur la façon de configurer la stratégie de gestion (MRM) des enregistrements de messagerie, voir [comment créer une stratégie de boîte aux lettres de dossier géré](http://go.microsoft.com/fwlink/?LinkId=100975).</span><span class="sxs-lookup"><span data-stu-id="0ebe9-117">For information about how to set up messaging records management (MRM) policy, see [How to Create a Managed Folder Mailbox Policy](http://go.microsoft.com/fwlink/?LinkId=100975).</span></span>
  
<span data-ttu-id="0ebe9-118">Pour plus d’informations sur la suppression des dossiers personnalisés gérés à partir d’une boîte aux lettres, voir [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).</span><span class="sxs-lookup"><span data-stu-id="0ebe9-118">For information about how to remove managed custom folders from a mailbox, see [Remove-ManagedFolder](http://go.microsoft.com/fwlink/?LinkId=100976).</span></span>
  
## <a name="createmanagedfolder-request-example"></a><span data-ttu-id="0ebe9-119">Exemple de requête CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-119">CreateManagedFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="0ebe9-120">Description</span><span class="sxs-lookup"><span data-stu-id="0ebe9-120">Description</span></span>

<span data-ttu-id="0ebe9-121">Une demande CreateManagedFolder l’exemple suivant montre comment ajouter un dossier géré nommé dossier géré de Test pour une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-121">The following example of a CreateManagedFolder request shows how to add a managed folder named Test Managed Folder to a mailbox.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0ebe9-122">Vous pouvez également utiliser l’accès délégué pour ajouter des dossiers personnalisés gérés.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-122">You can also use delegate access to add managed custom folders.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0ebe9-123">Code</span><span class="sxs-lookup"><span data-stu-id="0ebe9-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateManagedFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderNames>
        <t:FolderName>Test Managed Folder</t:FolderName>
      </FolderNames>
    </CreateManagedFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="0ebe9-124">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="0ebe9-124">Request elements</span></span>

<span data-ttu-id="0ebe9-125">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="0ebe9-125">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="0ebe9-126">CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-126">CreateManagedFolder</span></span>](createmanagedfolder.md)
    
- [<span data-ttu-id="0ebe9-127">Noms de dossier</span><span class="sxs-lookup"><span data-stu-id="0ebe9-127">FolderNames</span></span>](foldernames.md)
    
- [<span data-ttu-id="0ebe9-128">FolderName</span><span class="sxs-lookup"><span data-stu-id="0ebe9-128">FolderName</span></span>](foldername.md)
    
<span data-ttu-id="0ebe9-129">Pour trouver d’autres options pour le message de demande de l’opération CreateManagedFolder, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-129">To find other options for the request message of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0ebe9-130">Commencer à l’élément [CreateManagedFolder](createmanagedfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="0ebe9-130">Start at the [CreateManagedFolder](createmanagedfolder.md) element.</span></span> 
  
## <a name="successful-createmanagedfolder-response"></a><span data-ttu-id="0ebe9-131">Réponse CreateManagedFolder réussie</span><span class="sxs-lookup"><span data-stu-id="0ebe9-131">Successful CreateManagedFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="0ebe9-132">Description</span><span class="sxs-lookup"><span data-stu-id="0ebe9-132">Description</span></span>

<span data-ttu-id="0ebe9-133">L’exemple de code suivant montre une réponse positive à une demande CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-133">The following code example shows a successful response to a CreateManagedFolder request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="0ebe9-134">Les valeurs d’attribut **Id** et **ChangeKey** ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-134">The **Id** and **ChangeKey** attribute values have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="0ebe9-135">Code</span><span class="sxs-lookup"><span data-stu-id="0ebe9-135">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AS0AdX=" ChangeKey="AACADA=="/>
            </t:Folder>
          </m:Folders>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="0ebe9-136">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="0ebe9-136">Successful response elements</span></span>

<span data-ttu-id="0ebe9-137">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="0ebe9-137">The following elements are used in the response:</span></span> 
  
- [<span data-ttu-id="0ebe9-138">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0ebe9-138">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="0ebe9-139">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ebe9-139">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0ebe9-140">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ebe9-140">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="0ebe9-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ebe9-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ebe9-142">Dossiers</span><span class="sxs-lookup"><span data-stu-id="0ebe9-142">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="0ebe9-143">Folder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-143">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="0ebe9-144">FolderId</span><span class="sxs-lookup"><span data-stu-id="0ebe9-144">FolderId</span></span>](folderid.md)
    
<span data-ttu-id="0ebe9-145">Pour trouver d’autres options pour les messages de réponse de l’opération CreateManagedFolder, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-145">To find other options for the response messages of the CreateManagedFolder operation, explore the schema hierarchy.</span></span> <span data-ttu-id="0ebe9-146">Démarrez au niveau de l’élément [CreateManagedFolderResponse](createmanagedfolderresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="0ebe9-146">Start at the [CreateManagedFolderResponse](createmanagedfolderresponse.md) element.</span></span> 
  
## <a name="createmanagedfolder-error-response"></a><span data-ttu-id="0ebe9-147">Réponse d’erreur CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-147">CreateManagedFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="0ebe9-148">Description</span><span class="sxs-lookup"><span data-stu-id="0ebe9-148">Description</span></span>

<span data-ttu-id="0ebe9-149">L’exemple de code suivant montre une réponse d’erreur à une demande CreateManagedFolder.</span><span class="sxs-lookup"><span data-stu-id="0ebe9-149">The following code example shows an error response to a CreateManagedFolder request.</span></span>
  
### <a name="code"></a><span data-ttu-id="0ebe9-150">Code</span><span class="sxs-lookup"><span data-stu-id="0ebe9-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="598" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateManagedFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateManagedFolderResponseMessage ResponseClass="Error">
          <m:MessageText>A specified managed folder already exists in the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorManagedFolderAlreadyExists</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders/>
        </m:CreateManagedFolderResponseMessage>
      </m:ResponseMessages>
    </CreateManagedFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="0ebe9-151">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="0ebe9-151">Error response elements</span></span>

<span data-ttu-id="0ebe9-152">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="0ebe9-152">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="0ebe9-153">CreateManagedFolderResponse</span><span class="sxs-lookup"><span data-stu-id="0ebe9-153">CreateManagedFolderResponse</span></span>](createmanagedfolderresponse.md)
    
- [<span data-ttu-id="0ebe9-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0ebe9-154">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="0ebe9-155">CreateManagedFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0ebe9-155">CreateManagedFolderResponseMessage</span></span>](createmanagedfolderresponsemessage.md)
    
- [<span data-ttu-id="0ebe9-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ebe9-156">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0ebe9-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ebe9-157">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ebe9-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ebe9-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="0ebe9-159">Dossiers</span><span class="sxs-lookup"><span data-stu-id="0ebe9-159">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="see-also"></a><span data-ttu-id="0ebe9-160">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0ebe9-160">See also</span></span>



[<span data-ttu-id="0ebe9-161">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-161">GetFolder operation</span></span>](getfolder-operation.md)
  
[<span data-ttu-id="0ebe9-162">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="0ebe9-162">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="0ebe9-163">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="0ebe9-163">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)
  
[<span data-ttu-id="0ebe9-164">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="0ebe9-164">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

