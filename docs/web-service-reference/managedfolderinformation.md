---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: L’élément ManagedFolderInformation contient des informations sur un dossier personnalisé géré.
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828341"
---
# <a name="managedfolderinformation"></a><span data-ttu-id="467bc-103">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="467bc-103">ManagedFolderInformation</span></span>

<span data-ttu-id="467bc-104">L’élément **ManagedFolderInformation** contient des informations sur un dossier personnalisé géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-104">The **ManagedFolderInformation** element contains information about a managed custom folder.</span></span> 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 <span data-ttu-id="467bc-105">**ManagedFolderInformationType**</span><span class="sxs-lookup"><span data-stu-id="467bc-105">**ManagedFolderInformationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="467bc-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="467bc-106">Attributes and elements</span></span>

<span data-ttu-id="467bc-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="467bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="467bc-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="467bc-108">Attributes</span></span>

<span data-ttu-id="467bc-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="467bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="467bc-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="467bc-110">Child elements</span></span>

|<span data-ttu-id="467bc-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="467bc-111">**Element**</span></span>|<span data-ttu-id="467bc-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="467bc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="467bc-113">CanDelete</span><span class="sxs-lookup"><span data-stu-id="467bc-113">CanDelete</span></span>](candelete.md) <br/> |<span data-ttu-id="467bc-114">Indique si un dossier géré peut être supprimé par un client.</span><span class="sxs-lookup"><span data-stu-id="467bc-114">Indicates whether a managed folder can be deleted by a customer.</span></span>  <br/> |
|[<span data-ttu-id="467bc-115">CanRenameOrMove</span><span class="sxs-lookup"><span data-stu-id="467bc-115">CanRenameOrMove</span></span>](canrenameormove.md) <br/> |<span data-ttu-id="467bc-116">Indique si un dossier géré donné peut être renommé ou déplacé par le client.</span><span class="sxs-lookup"><span data-stu-id="467bc-116">Indicates whether a given managed folder can be renamed or moved by the customer.</span></span>  <br/> |
|[<span data-ttu-id="467bc-117">MustDisplayComment</span><span class="sxs-lookup"><span data-stu-id="467bc-117">MustDisplayComment</span></span>](mustdisplaycomment.md) <br/> |<span data-ttu-id="467bc-118">Indique si le commentaire de dossier géré doit être affiché.</span><span class="sxs-lookup"><span data-stu-id="467bc-118">Indicates whether the managed folder comment must be displayed.</span></span>  <br/> |
|[<span data-ttu-id="467bc-119">HasQuota</span><span class="sxs-lookup"><span data-stu-id="467bc-119">HasQuota</span></span>](hasquota.md) <br/> |<span data-ttu-id="467bc-120">Indique si le dossier géré a un quota.</span><span class="sxs-lookup"><span data-stu-id="467bc-120">Indicates whether the managed folder has a quota.</span></span>  <br/> |
|[<span data-ttu-id="467bc-121">IsManagedFoldersRoot</span><span class="sxs-lookup"><span data-stu-id="467bc-121">IsManagedFoldersRoot</span></span>](ismanagedfoldersroot.md) <br/> |<span data-ttu-id="467bc-122">Indique si le dossier géré est la racine de tous les dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="467bc-122">Indicates whether the managed folder is the root for all managed folders.</span></span>  <br/> |
|[<span data-ttu-id="467bc-123">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="467bc-123">ManagedFolderId</span></span>](managedfolderid.md) <br/> |<span data-ttu-id="467bc-124">Contient l’ID de dossier du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-124">Contains the folder ID of the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="467bc-125">Commentaire</span><span class="sxs-lookup"><span data-stu-id="467bc-125">Comment</span></span>](comment.md) <br/> |<span data-ttu-id="467bc-126">Contient le commentaire qui est associé à un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-126">Contains the comment that is associated with a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="467bc-127">StorageQuota</span><span class="sxs-lookup"><span data-stu-id="467bc-127">StorageQuota</span></span>](storagequota.md) <br/> |<span data-ttu-id="467bc-128">Décrit le quota de stockage pour le dossier géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-128">Describes the storage quota for the managed folder.</span></span>  <br/> |
|[<span data-ttu-id="467bc-129">FolderSize</span><span class="sxs-lookup"><span data-stu-id="467bc-129">FolderSize</span></span>](foldersize.md) <br/> |<span data-ttu-id="467bc-130">Décrit la taille totale de tout le contenu d’un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-130">Describes the total size of all the contents of a managed folder.</span></span>  <br/> |
|[<span data-ttu-id="467bc-131">Page d’accueil</span><span class="sxs-lookup"><span data-stu-id="467bc-131">HomePage</span></span>](homepage.md) <br/> |<span data-ttu-id="467bc-132">Spécifie l’URL qui sera la page d’accueil par défaut pour le dossier géré.</span><span class="sxs-lookup"><span data-stu-id="467bc-132">Specifies the URL that will be the default home page for the managed folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="467bc-133">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="467bc-133">Parent elements</span></span>

|<span data-ttu-id="467bc-134">**Élément**</span><span class="sxs-lookup"><span data-stu-id="467bc-134">**Element**</span></span>|<span data-ttu-id="467bc-135">**Description**</span><span class="sxs-lookup"><span data-stu-id="467bc-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="467bc-136">Folder</span><span class="sxs-lookup"><span data-stu-id="467bc-136">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="467bc-137">Représente un dossier dans la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="467bc-137">Represents a folder in the Exchange store.</span></span> <span data-ttu-id="467bc-138">Les dossiers personnalisés gérés peuvent être uniquement les sous-dossiers du dossier nommé **Dossiers gérés**.</span><span class="sxs-lookup"><span data-stu-id="467bc-138">Managed custom folders can only be subfolders of the folder named **Managed Folders**.</span></span>  <br/> |
|[<span data-ttu-id="467bc-139">CalendarFolder</span><span class="sxs-lookup"><span data-stu-id="467bc-139">CalendarFolder</span></span>](calendarfolder.md) <br/> |<span data-ttu-id="467bc-140">Non applicable.</span><span class="sxs-lookup"><span data-stu-id="467bc-140">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="467bc-141">ContactsFolder</span><span class="sxs-lookup"><span data-stu-id="467bc-141">ContactsFolder</span></span>](contactsfolder.md) <br/> |<span data-ttu-id="467bc-142">Non applicable.</span><span class="sxs-lookup"><span data-stu-id="467bc-142">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="467bc-143">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="467bc-143">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="467bc-144">Non applicable.</span><span class="sxs-lookup"><span data-stu-id="467bc-144">Not applicable.</span></span>  <br/> |
|[<span data-ttu-id="467bc-145">Dossier tâches</span><span class="sxs-lookup"><span data-stu-id="467bc-145">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="467bc-146">Non applicable.</span><span class="sxs-lookup"><span data-stu-id="467bc-146">Not applicable.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="467bc-147">Notes</span><span class="sxs-lookup"><span data-stu-id="467bc-147">Remarks</span></span>

<span data-ttu-id="467bc-148">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="467bc-148">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="467bc-149">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="467bc-149">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="467bc-150">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="467bc-150">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="467bc-151">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="467bc-151">Schema name</span></span>  <br/> |<span data-ttu-id="467bc-152">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="467bc-152">Types schema</span></span>  <br/> |
|<span data-ttu-id="467bc-153">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="467bc-153">Validation file</span></span>  <br/> |<span data-ttu-id="467bc-154">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="467bc-154">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="467bc-155">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="467bc-155">Can be empty</span></span>  <br/> |<span data-ttu-id="467bc-156">False</span><span class="sxs-lookup"><span data-stu-id="467bc-156">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="467bc-157">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="467bc-157">See also</span></span>



[<span data-ttu-id="467bc-158">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="467bc-158">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="467bc-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="467bc-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="467bc-160">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="467bc-160">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

